# Comparing `tmp/mawk-0.1.2.tar.gz` & `tmp/mawk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mawk-0.1.2.tar", max compression
+gzip compressed data, was "mawk-0.1.3.tar", max compression
```

## Comparing `mawk-0.1.2.tar` & `mawk-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-13 19:24:00.617990 mawk-0.1.2/LICENSE
--rw-r--r--   0        0        0     2266 2023-05-13 19:24:00.617990 mawk-0.1.2/README.md
--rw-r--r--   0        0        0     3349 2023-05-13 19:24:00.617990 mawk-0.1.2/mawk.py
--rw-r--r--   0        0        0      543 2023-05-13 19:24:00.617990 mawk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2935 1970-01-01 00:00:00.000000 mawk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 23:10:37.697187 mawk-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2380 2023-05-17 23:10:37.701187 mawk-0.1.3/README.md
+-rw-r--r--   0        0        0     3349 2023-05-17 23:10:37.701187 mawk-0.1.3/mawk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 23:10:37.701187 mawk-0.1.3/mawk/py.typed
+-rw-r--r--   0        0        0      543 2023-05-17 23:10:37.701187 mawk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 mawk-0.1.3/PKG-INFO
```

### Comparing `mawk-0.1.2/LICENSE` & `mawk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mawk-0.1.2/README.md` & `mawk-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # μ-awk
 This is a tiny Python implementation of a line processor with Awk-like semantics. You write a set of regex-based rules. The program loops through the lines of some input file, running the matching functions on lines that match.
 
 This package is too small by any margin to qualify for the status of "package", but I keep finding myself copy-pasting this code,making small improvements every time otherwise.
 
 ## Install
-It is considered best practice to use a virtual environment (I recommend using [`poetry`](https://python-poetry.org/)).
+It is considered best practice to use a virtual environment. I recommend using [`poetry`](https://python-poetry.org/). If you do use Poetry, you can add it to your project by running:
+
+```
+poetry add mawk
+```
+
+Otherwise, using `pip`:
 
 ```
 pip install mawk
 ```
 
 ## Tutorial
 A μ-awk routine is a set of methods that are triggered on regexes. The routine will recieve the `re.Match` object and is expected to return one of three things:
```

### Comparing `mawk-0.1.2/mawk.py` & `mawk-0.1.3/mawk/__init__.py`

 * *Files identical despite different names*

### Comparing `mawk-0.1.2/pyproject.toml` & `mawk-0.1.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mawk"
-version = "0.1.2"
+version = "0.1.3"
 description = "A minimalist implementation of an Awk-like model in Python"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2"
 readme = "README.md"
 repository = "https://github.com/jhidding/mawk"
 
 [tool.poetry.dependencies]
```

### Comparing `mawk-0.1.2/PKG-INFO` & `mawk-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mawk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A minimalist implementation of an Awk-like model in Python
 Home-page: https://github.com/jhidding/mawk
 License: Apache 2
 Author: Johan Hidding
 Author-email: j.hidding@esciencecenter.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,21 @@
 
 # μ-awk
 This is a tiny Python implementation of a line processor with Awk-like semantics. You write a set of regex-based rules. The program loops through the lines of some input file, running the matching functions on lines that match.
 
 This package is too small by any margin to qualify for the status of "package", but I keep finding myself copy-pasting this code,making small improvements every time otherwise.
 
 ## Install
-It is considered best practice to use a virtual environment (I recommend using [`poetry`](https://python-poetry.org/)).
+It is considered best practice to use a virtual environment. I recommend using [`poetry`](https://python-poetry.org/). If you do use Poetry, you can add it to your project by running:
+
+```
+poetry add mawk
+```
+
+Otherwise, using `pip`:
 
 ```
 pip install mawk
 ```
 
 ## Tutorial
 A μ-awk routine is a set of methods that are triggered on regexes. The routine will recieve the `re.Match` object and is expected to return one of three things:
```

