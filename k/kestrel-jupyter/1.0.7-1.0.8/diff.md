# Comparing `tmp/kestrel-jupyter-1.0.7.tar.gz` & `tmp/kestrel-jupyter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-jupyter-1.0.7.tar", last modified: Thu Dec  8 23:29:40 2022, max compression
+gzip compressed data, was "kestrel-jupyter-1.0.8.tar", last modified: Thu May 18 02:01:24 2023, max compression
```

## Comparing `kestrel-jupyter-1.0.7.tar` & `kestrel-jupyter-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:40.236251 kestrel-jupyter-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/src/kestrel_ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_ipython/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2022-12-08 23:29:40.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-08 23:29:40.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 23:29:40.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-08 23:29:40.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-08 23:29:40.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:40.240251 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/codemirror/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/codemirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/codemirror/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2022-12-08 23:29:20.000000 kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_ipython/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 02:01:24.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:24.291581 kestrel-jupyter-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/tests/test_kernel_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-18 02:00:59.000000 kestrel-jupyter-1.0.8/tests/test_notebook_syntax_gen.py
```

### Comparing `kestrel-jupyter-1.0.7/LICENSE` & `kestrel-jupyter-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.7/PKG-INFO` & `kestrel-jupyter-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kestrel-jupyter
-Version: 1.0.7
+Version: 1.0.8
 Summary: Kestrel Jupyter Kernel
 Home-page: https://github.com/IBM/kestrel-jupyter
 License: Apache 2.0 License
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 Kestrel Jupyter Notebook Kernel
 ===============================
```

### Comparing `kestrel-jupyter-1.0.7/README.rst` & `kestrel-jupyter-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.7/setup.cfg` & `kestrel-jupyter-1.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-jupyter
-version = 1.0.7
+version = 1.0.8
 description = Kestrel Jupyter Kernel
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -15,17 +15,17 @@
 	Operating System :: OS Independent
 	License :: OSI Approved :: Apache Software License
 
 [options]
 packages = find:
 package_dir = 
 	=src
-python_requires = >= 3.7
+python_requires = >= 3.8
 install_requires = 
-	kestrel-lang>=1.5.3
+	kestrel-lang>=1.6.0
 	jupyterlab-server==2.15.2
 	jupyterlab
 	jupyter_client
 tests_require = 
 	pytest
 
 [options.packages.find]
```

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_ipython/magic.py` & `kestrel-jupyter-1.0.8/src/kestrel_ipython/magic.py`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/PKG-INFO` & `kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kestrel-jupyter
-Version: 1.0.7
+Version: 1.0.8
 Summary: Kestrel Jupyter Kernel
 Home-page: https://github.com/IBM/kestrel-jupyter
 License: Apache 2.0 License
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 Kestrel Jupyter Notebook Kernel
 ===============================
```

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_jupyter.egg-info/SOURCES.txt` & `kestrel-jupyter-1.0.8/src/kestrel_jupyter.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 src/kestrel_jupyter_kernel/__init__.py
 src/kestrel_jupyter_kernel/__main__.py
 src/kestrel_jupyter_kernel/config.py
 src/kestrel_jupyter_kernel/kernel.py
 src/kestrel_jupyter_kernel/setup.py
 src/kestrel_jupyter_kernel/codemirror/__init__.py
 src/kestrel_jupyter_kernel/codemirror/kestrel_template.js
-src/kestrel_jupyter_kernel/codemirror/setup.py
+src/kestrel_jupyter_kernel/codemirror/setup.py
+tests/test_kernel_install.py
+tests/test_notebook_syntax_gen.py
```

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js` & `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/kestrel_template.js`

 * *Files identical despite different names*

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/codemirror/setup.py` & `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/codemirror/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import nbclassic
 import notebook
 import pkgutil
 import kestrel
 
 
 def update_codemirror_mode():
-
     for codemirror_file_path in _get_codemirror_file_paths():
         src_current = ""
         if os.path.isfile(codemirror_file_path):
             try:
                 with open(codemirror_file_path) as fp:
                     src_current = fp.read()
             except PermissionError:
```

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/kernel.py` & `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/kernel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from ipykernel.kernelbase import Kernel
-import os
 import logging
 
 from kestrel.codegen.display import DisplayWarning
 from kestrel.session import Session
-from kestrel_jupyter_kernel.config import LOG_FILE_NAME
 
 
 _logger = logging.getLogger(__name__)
 
 
 class KestrelKernel(Kernel):
     implementation = "kestrel"
@@ -18,32 +16,27 @@
     # https://jupyter-client.readthedocs.io/en/stable/messaging.html#msging-kernel-info
     language_info = {"name": "kestrel", "file_extension": ".hf"}
     banner = "Kestrel"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.kestrel_session = Session()
-        _set_logging(
-            self.kestrel_session.debug_mode,
-            os.path.join(self.kestrel_session.runtime_directory, LOG_FILE_NAME),
-        )
 
     def do_complete(self, code, cursor_pos):
         return {
             "matches": self.kestrel_session.do_complete(code, cursor_pos),
             "cursor_end": cursor_pos,
             "cursor_start": cursor_pos,
             "metadata": {},
             "status": "ok",
         }
 
     def do_execute(
         self, code, silent, store_history=True, user_expressions=None, allow_stdin=False
     ):
-
         errmsg = None
 
         if not silent:
             try:
                 outputs = self.kestrel_session.execute(code)
                 warning = "\n".join(
                     [
@@ -72,16 +65,7 @@
 
         return {
             "status": "ok",
             "execution_count": self.execution_count,
             "payload": [],
             "user_expressions": {},
         }
-
-
-def _set_logging(debug_flag, log_file_path):
-    logging.basicConfig(
-        format="%(asctime)s %(levelname)s %(name)s %(message)s",
-        datefmt="%H:%M:%S",
-        level=logging.DEBUG if debug_flag else logging.INFO,
-        handlers=[logging.FileHandler(log_file_path)],
-    )
```

### Comparing `kestrel-jupyter-1.0.7/src/kestrel_jupyter_kernel/setup.py` & `kestrel-jupyter-1.0.8/src/kestrel_jupyter_kernel/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             json.dump(_KERNEL_SPEC, kf)
 
         m = KernelSpecManager()
         m.install_kernel_spec(kernel_dirname, "kestrel", user=True)
 
 
 if __name__ == "__main__":
-
     print("Setup Kestrel Jupyter Kernel")
     print("  Install new Jupyter kernel ...", end=" ")
     install_kernelspec()
     print("done")
 
     # generate and install kestrel codemirrmor mode
     print("  Compute and install syntax highlighting ...", end=" ")
```

