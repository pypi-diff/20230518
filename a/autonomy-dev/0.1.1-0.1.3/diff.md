# Comparing `tmp/autonomy_dev-0.1.1.tar.gz` & `tmp/autonomy_dev-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.1.tar", max compression
+gzip compressed data, was "autonomy_dev-0.1.3.tar", max compression
```

## Comparing `autonomy_dev-0.1.1.tar` & `autonomy_dev-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      578 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/LICENSE
--rw-r--r--   0        0        0       58 2023-05-11 10:50:35.015487 autonomy_dev-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/__init__.py
--rw-r--r--   0        0        0     3151 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/cli.py
--rw-r--r--   0        0        0     2732 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/cli_executor.py
--rw-r--r--   0        0        0      301 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/constants.py
--rw-r--r--   0        0        0      529 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      464 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/test.py
--rw-r--r--   0        0        0     1083 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/auto_dev/utils.py
--rw-r--r--   0        0        0     2484 2023-05-11 10:48:11.285003 autonomy_dev-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1187 2023-05-11 10:31:40.571881 autonomy_dev-0.1.1/tests/test_cli.py
--rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 autonomy_dev-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/LICENSE
+-rw-r--r--   0        0        0      117 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/__init__.py
+-rw-r--r--   0        0        0     3151 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/cli.py
+-rw-r--r--   0        0        0     2732 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0      301 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/constants.py
+-rw-r--r--   0        0        0      529 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      464 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/lint.py
+-rw-r--r--   0        0        0      438 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/test.py
+-rw-r--r--   0        0        0     1083 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/auto_dev/utils.py
+-rw-r--r--   0        0        0     2516 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1187 2023-05-18 10:13:29.042774 autonomy_dev-0.1.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 autonomy_dev-0.1.3/PKG-INFO
```

### Comparing `autonomy_dev-0.1.1/LICENSE` & `autonomy_dev-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.1/auto_dev/cli.py` & `autonomy_dev-0.1.3/auto_dev/cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.1/auto_dev/cli_executor.py` & `autonomy_dev-0.1.3/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.1/auto_dev/data/pylama.ini` & `autonomy_dev-0.1.3/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.1/auto_dev/utils.py` & `autonomy_dev-0.1.3/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.1/pyproject.toml` & `autonomy_dev-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.1"
+version = "0.1.3"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -44,25 +44,27 @@
 bump2version = "^1.0.1"
 yamllint = "^1.27.1"
 GitPython = "^3.1.27"
 pylama = {extras = ["all"], version = "^8.4.1"}
 rich-click = "^1.5.2"
 install = "^1.3.5"
 mkdocstrings-python = "^0.10.0"
+pylint = "^2.17.4"
 
 [tool.poetry.dev-dependencies]
 
 
 [tool.poetry.extras]
-test = [
+all = [
     "pytest",
     "black",
     "isort",
     "mypy",
     "pylama",
+    "pylint",
     "pytest-cov"
     ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml", "bump2version"]
 
 doc = [
     "mkdocs",
```

### Comparing `autonomy_dev-0.1.1/tests/test_cli.py` & `autonomy_dev-0.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.1/PKG-INFO` & `autonomy_dev-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.1
+Version: 0.1.3
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,38 +17,45 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
-Provides-Extra: test
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
-Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "test"
+Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "all"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: click (==8.0.2)
 Requires-Dist: install (>=1.3.5,<2.0.0)
-Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "test"
+Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "all"
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.6.1,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.4.0,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
 Requires-Dist: mkdocstrings-python (>=0.10.0,<0.11.0)
-Requires-Dist: mypy (>=0.971,<0.972) ; extra == "test"
+Requires-Dist: mypy (>=0.971,<0.972) ; extra == "all"
 Requires-Dist: pip (>=22.2.2,<23.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.20.0,<3.0.0) ; extra == "dev"
-Requires-Dist: pylama[all] (>=8.4.1,<9.0.0) ; extra == "test"
-Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
+Requires-Dist: pylama[all] (>=8.4.1,<9.0.0) ; extra == "all"
+Requires-Dist: pylint (>=2.17.4,<3.0.0) ; extra == "all"
+Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "all"
 Requires-Dist: rich-click (>=1.5.2,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.25.1,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=4.0.1,<5.0.0) ; extra == "dev"
 Requires-Dist: yamllint (>=1.27.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Autonomy Dev
 
 Tooling to speed up autonomy development.
 
+# Installation
+
+```bash
+pip install autonomy-dev[all]
+```
+
```

