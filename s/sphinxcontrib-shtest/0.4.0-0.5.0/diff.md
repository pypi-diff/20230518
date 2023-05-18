# Comparing `tmp/sphinxcontrib-shtest-0.4.0.tar.gz` & `tmp/sphinxcontrib-shtest-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-shtest-0.4.0.tar", last modified: Wed Apr  5 03:41:48 2023, max compression
+gzip compressed data, was "sphinxcontrib-shtest-0.5.0.tar", last modified: Thu May 18 18:53:32 2023, max compression
```

## Comparing `sphinxcontrib-shtest-0.4.0.tar` & `sphinxcontrib-shtest-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-05 03:41:31.000000 sphinxcontrib-shtest-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-05 03:41:31.000000 sphinxcontrib-shtest-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/sphinxcontrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/sphinxcontrib/shtest/
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-04-05 03:41:31.000000 sphinxcontrib-shtest-0.4.0/sphinxcontrib/shtest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-05 03:41:48.000000 sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-05 03:41:48.000000 sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 03:41:48.000000 sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 03:41:48.000000 sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 03:41:48.000000 sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:41:48.756884 sphinxcontrib-shtest-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-05 03:41:31.000000 sphinxcontrib-shtest-0.4.0/tests/test_shtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-18 18:53:07.000000 sphinxcontrib-shtest-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-18 18:53:07.000000 sphinxcontrib-shtest-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/sphinxcontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/sphinxcontrib/shtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-18 18:53:07.000000 sphinxcontrib-shtest-0.5.0/sphinxcontrib/shtest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-18 18:53:32.000000 sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-18 18:53:32.000000 sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:53:32.000000 sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 18:53:32.000000 sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 18:53:32.000000 sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:53:32.717645 sphinxcontrib-shtest-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-18 18:53:07.000000 sphinxcontrib-shtest-0.5.0/tests/test_shtest.py
```

### Comparing `sphinxcontrib-shtest-0.4.0/PKG-INFO` & `sphinxcontrib-shtest-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-shtest
-Version: 0.4.0
+Version: 0.5.0
 Home-page: https://github.com/tillahoffmann/sphinxcontrib-shtest
 Description-Content-Type: text/x-rst
 
 🧪 shtest
 =========
 
 .. image:: https://github.com/tillahoffmann/sphinxcontrib-shtest/actions/workflows/main.yaml/badge.svg
@@ -69,8 +69,8 @@
     $ echo hello > world.txt
 
 .. ls -l
 
 Installation
 ------------
 
-Run :code:`pip install sphinxcontrib-shtest` to install the package and add :code:`"sphinxcontrib-shtest"` to your :code:`extensions` list in :code:`conf.py` (see `here <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-extensions>`__ for details). Then execute :code:`sphinx-build -b shtest /path/to/source/directory /path/to/output/directory`.
+Run :code:`pip install sphinxcontrib-shtest` to install the package and add :code:`"sphinxcontrib.shtest"` to your :code:`extensions` list in :code:`conf.py` (see `here <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-extensions>`__ for details). Then execute :code:`sphinx-build -b shtest /path/to/source/directory /path/to/output/directory`.
```

### Comparing `sphinxcontrib-shtest-0.4.0/README.rst` & `sphinxcontrib-shtest-0.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     $ echo hello > world.txt
 
 .. sh:: ls -l
 
 Installation
 ------------
 
-Run :code:`pip install sphinxcontrib-shtest` to install the package and add :code:`"sphinxcontrib-shtest"` to your :code:`extensions` list in :code:`conf.py` (see `here <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-extensions>`__ for details). Then execute :code:`sphinx-build -b shtest /path/to/source/directory /path/to/output/directory`.
+Run :code:`pip install sphinxcontrib-shtest` to install the package and add :code:`"sphinxcontrib.shtest"` to your :code:`extensions` list in :code:`conf.py` (see `here <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-extensions>`__ for details). Then execute :code:`sphinx-build -b shtest /path/to/source/directory /path/to/output/directory`.
```

### Comparing `sphinxcontrib-shtest-0.4.0/setup.py` & `sphinxcontrib-shtest-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fp.read()
 long_description = long_description \
     .replace(".. shtest::", ".. code-block::\n") \
     .replace(".. sh::", "..")
 
 setup(
     name="sphinxcontrib-shtest",
-    version="0.4.0",
+    version="0.5.0",
     packages=find_namespace_packages(),
     install_requires=[
         "sphinx",
     ],
     long_description_content_type="text/x-rst",
     long_description=long_description,
     url="https://github.com/tillahoffmann/sphinxcontrib-shtest",
```

### Comparing `sphinxcontrib-shtest-0.4.0/sphinxcontrib/shtest/__init__.py` & `sphinxcontrib-shtest-0.5.0/sphinxcontrib/shtest/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,31 +162,35 @@
     Displays shell command output in the documentation.
     """
     required_arguments = 1
     optional_arguments = float("inf")
     has_content = False
     option_spec = {
         "stderr": directives.flag,
+        "hide-cmd": directives.flag,
         "cwd": str,
     }
 
     def run(self) -> List[Node]:
         # Run the command and display the output.
         parent = Path(self.state.document["source"]).parent
         cwd = (parent / cwd) if (cwd := self.options.get("cwd")) else parent
         stderr = "stderr" in self.options
+        args = " ".join(self.arguments)
         kwargs = {
-            "args": " ".join(self.arguments),
+            "args": args,
             "shell": True,
             "text": True,
             "stderr" if stderr else "stdout": subprocess.PIPE,
         }
         process = subprocess.run(**kwargs)
         content = process.stderr if stderr else process.stdout
-        node = literal_block(content, content)
+        if "hide-cmd" not in self.options:
+            content = f"$ {args}\n{content}"
+        node = literal_block(content, content, language="bash")
         return [node]
 
 
 class ShTestBuilder(Builder):
     """
     Runs shell command test snippets in the documentation.
     """
```

### Comparing `sphinxcontrib-shtest-0.4.0/sphinxcontrib_shtest.egg-info/PKG-INFO` & `sphinxcontrib-shtest-0.5.0/sphinxcontrib_shtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-shtest
-Version: 0.4.0
+Version: 0.5.0
 Home-page: https://github.com/tillahoffmann/sphinxcontrib-shtest
 Description-Content-Type: text/x-rst
 
 🧪 shtest
 =========
 
 .. image:: https://github.com/tillahoffmann/sphinxcontrib-shtest/actions/workflows/main.yaml/badge.svg
@@ -69,8 +69,8 @@
     $ echo hello > world.txt
 
 .. ls -l
 
 Installation
 ------------
 
-Run :code:`pip install sphinxcontrib-shtest` to install the package and add :code:`"sphinxcontrib-shtest"` to your :code:`extensions` list in :code:`conf.py` (see `here <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-extensions>`__ for details). Then execute :code:`sphinx-build -b shtest /path/to/source/directory /path/to/output/directory`.
+Run :code:`pip install sphinxcontrib-shtest` to install the package and add :code:`"sphinxcontrib.shtest"` to your :code:`extensions` list in :code:`conf.py` (see `here <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-extensions>`__ for details). Then execute :code:`sphinx-build -b shtest /path/to/source/directory /path/to/output/directory`.
```

### Comparing `sphinxcontrib-shtest-0.4.0/tests/test_shtest.py` & `sphinxcontrib-shtest-0.5.0/tests/test_shtest.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,30 +24,46 @@
 
 
 def test_strip_colors() -> None:
     colored = f"{colorama.Fore.GREEN}hello {colorama.Fore.RED}world{colorama.Fore.RESET}"
     assert strip_colors(colored) == "hello world"
 
 
-@pytest.mark.parametrize("document, match", [
+@pytest.mark.parametrize("document_name, match", [
     ("true", None),
     ("false", "Expected return code: 0"),
     ("false-1-tempdir", None),
     ("multiple", None),
     ("no-command", "Expected a command starting with"),
     ("tempdir-and-cwd", "`cwd` and `tempdir` cannot"),
     ("cwd", None),
     ("sh", None),
 ])
-def test_directive_build(tmp_path: Path, document: str, match: Optional[str]) -> None:
-    # Copy data to a temporary directory.
+@pytest.mark.parametrize("builder", ["html", "shtest"])
+def test_directive_build(tmp_path: Path, document_name: str, match: Optional[str], builder: str) \
+        -> None:
+    # Copy data to a temporary directory and add a header.
     (tmp_path / "conf.py").write_text("extensions = ['sphinxcontrib.shtest']")
-    document = (Path(__file__).parent / "rst" / document).with_suffix(".rst")
-    shutil.copy(document, tmp_path / "index.rst")
+    document = (Path(__file__).parent / "rst" / document_name).with_suffix(".rst")
+
+    text = document.read_text()
+    (tmp_path / "index.rst").write_text("\n".join([
+        document_name,
+        "=" * len(document_name),
+        "",
+        text
+    ]))
 
     # Run the builder.
-    app = Sphinx(tmp_path, tmp_path, tmp_path / "_build", tmp_path / "_toctree", "shtest")
-    if match:
+    outdir = tmp_path / "_build"
+    app = Sphinx(tmp_path, tmp_path, outdir, tmp_path / "doctreedir", builder)
+    if match and builder == "shtest":
         with pytest.raises(ShTestError, match=match):
             app.build()
     else:
         app.build()
+        if builder == "html":
+            # Copy the result to the output directory for inspection.
+            html = Path(__file__).parent / "html"
+            html.mkdir(exist_ok=True)
+            html = (html / document_name).with_suffix(".html")
+            shutil.copy(outdir / "index.html", html)
```

