# Comparing `tmp/sunsolve-0.0.1.tar.gz` & `tmp/sunsolve-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsolve-0.0.1.tar", max compression
+gzip compressed data, was "sunsolve-0.0.4.tar", max compression
```

## Comparing `sunsolve-0.0.1.tar` & `sunsolve-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     2871 2023-05-18 11:00:32.940447 sunsolve-0.0.1/README.md
--rw-r--r--   0        0        0     2167 2023-05-18 11:00:32.940447 sunsolve-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 11:00:32.940447 sunsolve-0.0.1/src/sunsolve/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 11:00:32.940447 sunsolve-0.0.1/src/sunsolve/py.typed
--rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 sunsolve-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2727 2023-05-18 17:27:23.424403 sunsolve-0.0.4/README.md
+-rw-r--r--   0        0        0     2167 2023-05-18 17:27:23.424403 sunsolve-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 17:27:23.424403 sunsolve-0.0.4/src/sunsolve/__init__.py
+-rw-r--r--   0        0        0     4300 2023-05-18 17:27:23.424403 sunsolve-0.0.4/src/sunsolve/fitness_function.py
+-rw-r--r--   0        0        0        0 2023-05-18 17:27:23.428403 sunsolve-0.0.4/src/sunsolve/genetic_algorithm.py
+-rw-r--r--   0        0        0      721 2023-05-18 17:27:23.428403 sunsolve-0.0.4/src/sunsolve/plotter.py
+-rw-r--r--   0        0        0     1266 2023-05-18 17:27:23.428403 sunsolve-0.0.4/src/sunsolve/solver.py
+-rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 sunsolve-0.0.4/PKG-INFO
```

### Comparing `sunsolve-0.0.1/README.md` & `sunsolve-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -84,9 +84,7 @@
 Or if you want e.g. want to run all checks manually for all files:
 
 ```sh
 pre-commit run --all-files
 ```
 
 ---
-
-This project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.
```

### Comparing `sunsolve-0.0.1/pyproject.toml` & `sunsolve-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sunsolve"
-version = "0.0.1"
+version = "0.0.4"
 description = "A python package for solving the inverse problem of matching LEDs to the sun’s spectrum"
 authors = [
     "nkalis <n.kalis98@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `sunsolve-0.0.1/PKG-INFO` & `sunsolve-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsolve
-Version: 0.0.1
+Version: 0.0.4
 Summary: A python package for solving the inverse problem of matching LEDs to the sun’s spectrum
 Home-page: https://nkalis.github.io/sunsolve
 License: MIT
 Author: nkalis
 Author-email: n.kalis98@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -114,9 +114,7 @@
 
 ```sh
 pre-commit run --all-files
 ```
 
 ---
 
-This project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.
-
```

