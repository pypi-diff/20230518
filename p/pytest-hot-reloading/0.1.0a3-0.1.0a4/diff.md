# Comparing `tmp/pytest_hot_reloading-0.1.0a3.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a3.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a4.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a3.tar` & `pytest_hot_reloading-0.1.0a4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     2442 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/README.md
--rw-r--r--   0        0        0      654 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     1846 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0     4556 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     7672 2023-05-17 20:02:44.967686 pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-18 21:22:49.726174 pytest_hot_reloading-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     2442 2023-05-18 21:22:49.726174 pytest_hot_reloading-0.1.0a4/README.md
+-rw-r--r--   0        0        0      676 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     1969 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0     7638 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     8221 2023-05-18 21:22:49.730174 pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a4/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a3/LICENSE` & `pytest_hot_reloading-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a3/README.md` & `pytest_hot_reloading-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a3/pyproject.toml` & `pytest_hot_reloading-0.1.0a4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 line-length = 98
 
 [tool.black]
 line-length = 98
 
 [tool.poetry]
 name = "pytest-hot-reloading"
-version = "0.1.0-alpha.3"
+version = "0.1.0-alpha.4"
 description = ""
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 packages = [{ include = "pytest_hot_reloading" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jurigged = "^0.5.5"
+cachetools = "^5.3.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 ruff = "^0.0.261"
 black = "^23.3.0"
 pytest = "^7.2.2"
 megamock = "^0.1.0b3"
```

### Comparing `pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import socket
 import sys
+import time
 import xmlrpc.client
 
-from pytest_hot_reloading.daemon import PytestDaemon
-
 
 class PytestClient:
     _socket: socket.socket | None
     _daemon_host: str
     _daemon_port: int
     _pytest_name: str
 
@@ -21,15 +20,17 @@
 
     def run(self, args: list[str]) -> str:
         self._start_daemon_if_needed()
 
         server_url = f"http://{self._daemon_host}:{self._daemon_port}"
         server = xmlrpc.client.ServerProxy(server_url)
 
+        start = time.time()
         result = server.run_pytest(args)
+        print(f"Daemon took {(time.time() - start):.3f} seconds to reply")
 
         stdout = result["stdout"].data.decode("utf-8")
         stderr = result["stderr"].data.decode("utf-8")
 
         print(stdout, file=sys.stdout)
         print(stderr, file=sys.stderr)
 
@@ -51,11 +52,13 @@
             self._socket.close()
         except ConnectionRefusedError:
             # the daemon is not running
             # start the daemon
             self._start_daemon()
 
     def _start_daemon(self) -> None:
+        from pytest_hot_reloading.daemon import PytestDaemon
+
         # start the daemon
         PytestDaemon.start(
             host=self._daemon_host, port=self._daemon_port, pytest_name=self._pytest_name
         )
```

### Comparing `pytest_hot_reloading-0.1.0a3/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a4/pytest_hot_reloading/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """
 Pytest Hot Reloading plugin
 """
-import ast
-import fnmatch
+from __future__ import annotations
+
 import os
-import re
 import sys
-from typing import Callable
-
-import jurigged
-import jurigged.codetools as jurigged_codetools
-from pytest import Config, Item, Session
+from typing import TYPE_CHECKING, Callable
 
 from pytest_hot_reloading.client import PytestClient
-from pytest_hot_reloading.daemon import PytestDaemon
 
 # this is modified by the daemon so that the pytest_collection hooks does not run
 i_am_server = False
 
 seen_paths = set()
 
+if TYPE_CHECKING:
+    from pytest import Config, Item, Session
+
 
 def pytest_addoption(parser) -> None:
     group = parser.getgroup("daemon")
     group.addoption(
         "--daemon",
         action="store_true",
         default=False,
@@ -71,83 +68,96 @@
     """
     # early escapes
     if config.option.collectonly:
         return
     if i_am_server:
         return
     _plugin_logic(config)
+    # dont do any more work. Don't let pytest continue
+    return 0  # status code 0
 
 
-def _jurigged_logger(x: str) -> None:
-    """
-    Jurigged behavior is to both print and log.
-
-    By default this creates duplicated output.
-
-    Pass in a no-op logger to prevent this.
-    """
-
-
-OrigFunctionDefinition = jurigged_codetools.FunctionDefinition
-
-
-class NewFunctionDefinition(OrigFunctionDefinition):
-    def reevaluate(self, new_node, glb):
-        new_node = self.apply_assertion_rewrite(new_node, glb)
-        return super().reevaluate(new_node, glb)
-
-    def apply_assertion_rewrite(self, ast_func, glb):
-        from _pytest.assertion.rewrite import AssertionRewriter
-
-        nodes: list[ast.AST] = [ast_func]
-        while nodes:
-            node = nodes.pop()
-            for name, field in ast.iter_fields(node):
-                if isinstance(field, list):
-                    new: list[ast.AST] = []
-                    for i, child in enumerate(field):
-                        if isinstance(child, ast.Assert):
-                            # Transform assert.
-                            new.extend(
-                                AssertionRewriter(glb["__file__"], None, None).visit(child)
-                            )
-                        else:
-                            new.append(child)
-                            if isinstance(child, ast.AST):
-                                nodes.append(child)
-                    setattr(node, name, new)
-                elif (
-                    isinstance(field, ast.AST)
-                    # Don't recurse into expressions as they can't contain
-                    # asserts.
-                    and not isinstance(field, ast.expr)
-                ):
-                    nodes.append(field)
-        return ast_func
+def monkey_patch_jurigged_function_definition():
+    import jurigged.codetools as jurigged_codetools
 
+    OrigFunctionDefinition = jurigged_codetools.FunctionDefinition
 
-# monkey patch in new definition
-jurigged_codetools.FunctionDefinition = NewFunctionDefinition
+    import ast
+
+    class NewFunctionDefinition(OrigFunctionDefinition):
+        def reevaluate(self, new_node, glb):
+            new_node = self.apply_assertion_rewrite(new_node, glb)
+            return super().reevaluate(new_node, glb)
+
+        def apply_assertion_rewrite(self, ast_func, glb):
+            from _pytest.assertion.rewrite import AssertionRewriter
+
+            nodes: list[ast.AST] = [ast_func]
+            while nodes:
+                node = nodes.pop()
+                for name, field in ast.iter_fields(node):
+                    if isinstance(field, list):
+                        new: list[ast.AST] = []
+                        for i, child in enumerate(field):
+                            if isinstance(child, ast.Assert):
+                                # Transform assert.
+                                new.extend(
+                                    AssertionRewriter(glb["__file__"], None, None).visit(child)
+                                )
+                            else:
+                                new.append(child)
+                                if isinstance(child, ast.AST):
+                                    nodes.append(child)
+                        setattr(node, name, new)
+                    elif (
+                        isinstance(field, ast.AST)
+                        # Don't recurse into expressions as they can't contain
+                        # asserts.
+                        and not isinstance(field, ast.expr)
+                    ):
+                        nodes.append(field)
+            return ast_func
+
+    # monkey patch in new definition
+    jurigged_codetools.FunctionDefinition = NewFunctionDefinition
+
+
+def setup_jurigged(config: Config):
+    def _jurigged_logger(x: str) -> None:
+        """
+        Jurigged behavior is to both print and log.
+
+        By default this creates duplicated output.
+
+        Pass in a no-op logger to prevent this.
+        """
+
+    import jurigged
+
+    pattern = _get_pattern_filters(config)
+    # TODO: intelligently use poll versus watchman (https://github.com/JamesHutchison/pytest-hot-reloading/issues/16)
+    jurigged.watch(pattern=pattern, logger=_jurigged_logger, poll=True)
 
 
 def _plugin_logic(config: Config) -> None:
     """
     The core plugin logic. This is where it splits based on whether we are the server or client.
 
     In either case, the pytest logic will not continue after this.
     """
     # if daemon is passed, then we are the daemon / server
     # if daemon is not passed, then we are the client
     daemon_port = int(config.option.daemon_port)
     if config.option.daemon:
         # pytest prints out "collecting ...". The leading \r prevents that
         print("\rStarting daemon...")
-        pattern = _get_pattern_filters(config)
-        # TODO: intelligently use poll versus watchman
-        jurigged.watch(pattern=pattern, logger=_jurigged_logger, poll=True)
+        setup_jurigged(config)
+
+        from pytest_hot_reloading.daemon import PytestDaemon
+
         daemon = PytestDaemon(daemon_port=daemon_port)
 
         daemon.run_forever()
     else:
         pytest_name = config.option.pytest_name
         client = PytestClient(daemon_port=daemon_port, pytest_name=pytest_name)
         # find the index of the first value that is not None
@@ -164,17 +174,14 @@
             print(sys.argv)
             raise Exception(
                 "Could not find pytest name in args. "
                 "Check the configured name versus the actual name."
             )
         client.run(sys.argv[pytest_name_index + 1 :])
 
-        # dont do any more work. Don't let pytest continue
-        os._exit(0)
-
 
 def _get_pattern_filters(config: Config) -> str | Callable[[str], bool]:
     """
     Jurigged takes in a pattern argument. The argument is either a glob string
     or a function that returns True if the path passed into it should be watched.
 
     This creates a function filter that will return True if the path matches.
@@ -183,14 +190,17 @@
     and creates a function that will return True if the path matches the watch globs.
 
     The seen_paths set is used to prevent duplicate paths from being watched and also
     acts as a short circuit for paths that have already been seen.
     """
     global seen_paths
 
+    import fnmatch
+    import re
+
     def normalize(glob: str) -> str:
         if glob.startswith("~"):
             glob = os.path.expanduser(glob)
         elif not glob.startswith("/"):
             glob = os.path.abspath(glob)
         if os.path.isdir(glob):
             glob = os.path.join(glob, "*")
@@ -223,14 +233,18 @@
 
 
 def pytest_collection_modifyitems(session: Session, config: Config, items: list[Item]) -> None:
     """
     This hooks is called by pytest after the collection phase.
 
     This adds tests to the watch list automatically.
+
+    The client should never get this far. This should only be
+    used by the daemon.
     """
     global seen_paths
+    import jurigged
 
     for item in items:
         if item.path and item.path not in seen_paths:
             jurigged.watch(pattern=str(item.path))
             seen_paths.add(item.path)
```

### Comparing `pytest_hot_reloading-0.1.0a3/PKG-INFO` & `pytest_hot_reloading-0.1.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: 
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: jurigged (>=0.5.5,<0.6.0)
 Description-Content-Type: text/markdown
 
 # A PyTest Hot Reloading Plugin
 A hot reloading pytest daemon, implemented as a plugin.
 
 This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
```

