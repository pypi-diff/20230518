# Comparing `tmp/usseg-0.1.0a1.tar.gz` & `tmp/usseg-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usseg-0.1.0a1.tar", max compression
+gzip compressed data, was "usseg-0.2.0a1.tar", max compression
```

## Comparing `usseg-0.1.0a1.tar` & `usseg-0.2.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2831 2023-05-17 14:48:09.714561 usseg-0.1.0a1/README.md
--rw-r--r--   0        0        0      665 2023-05-18 10:16:50.439804 usseg-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0    53504 2023-05-17 12:58:04.630200 usseg-0.1.0a1/usseg/General_functions.py
--rw-r--r--   0        0        0     4115 2023-05-17 14:37:14.323870 usseg-0.1.0a1/usseg/Organise_files.py
--rw-r--r--   0        0        0    11405 2023-05-17 19:40:16.094684 usseg-0.1.0a1/usseg/Refined_anon_2_html.py
--rw-r--r--   0        0        0      303 2023-05-17 12:40:36.083145 usseg-0.1.0a1/usseg/__init__.py
--rw-r--r--   0        0        0      857 2023-05-18 10:07:46.451007 usseg-0.1.0a1/usseg/main.py
--rw-r--r--   0        0        0     4914 2023-05-17 14:12:40.206489 usseg-0.1.0a1/usseg/visualisation_html.py
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 usseg-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-05-17 14:48:09.714561 usseg-0.2.0a1/README.md
+-rw-r--r--   0        0        0      665 2023-05-18 10:18:19.531200 usseg-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0    53504 2023-05-17 12:58:04.630200 usseg-0.2.0a1/usseg/General_functions.py
+-rw-r--r--   0        0        0     4115 2023-05-17 14:37:14.323870 usseg-0.2.0a1/usseg/Organise_files.py
+-rw-r--r--   0        0        0    11405 2023-05-17 19:40:16.094684 usseg-0.2.0a1/usseg/Refined_anon_2_html.py
+-rw-r--r--   0        0        0      303 2023-05-17 12:40:36.083145 usseg-0.2.0a1/usseg/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-18 10:07:46.451007 usseg-0.2.0a1/usseg/main.py
+-rw-r--r--   0        0        0     4914 2023-05-17 14:12:40.206489 usseg-0.2.0a1/usseg/visualisation_html.py
+-rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 usseg-0.2.0a1/PKG-INFO
```

### Comparing `usseg-0.1.0a1/README.md` & `usseg-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `usseg-0.1.0a1/pyproject.toml` & `usseg-0.2.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usseg"
-version = "0.1.0a1"
+version = "0.2.0a1"
 description = "Tools to segment doppler ultrasound signals from scan images."
 authors = ["Dale Kernot <874043@swansea.ac.uk>"]
 license = "GPL-v3-or-later"
 readme = "README.md"
 packages = [{include = "usseg"}]
 
 [tool.poetry.dependencies]
```

### Comparing `usseg-0.1.0a1/usseg/General_functions.py` & `usseg-0.2.0a1/usseg/General_functions.py`

 * *Files identical despite different names*

### Comparing `usseg-0.1.0a1/usseg/Organise_files.py` & `usseg-0.2.0a1/usseg/Organise_files.py`

 * *Files identical despite different names*

### Comparing `usseg-0.1.0a1/usseg/Refined_anon_2_html.py` & `usseg-0.2.0a1/usseg/Refined_anon_2_html.py`

 * *Files identical despite different names*

### Comparing `usseg-0.1.0a1/usseg/main.py` & `usseg-0.2.0a1/usseg/main.py`

 * *Files identical despite different names*

### Comparing `usseg-0.1.0a1/usseg/visualisation_html.py` & `usseg-0.2.0a1/usseg/visualisation_html.py`

 * *Files identical despite different names*

### Comparing `usseg-0.1.0a1/PKG-INFO` & `usseg-0.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usseg
-Version: 0.1.0a1
+Version: 0.2.0a1
 Summary: Tools to segment doppler ultrasound signals from scan images.
 License: GPL-v3-or-later
 Author: Dale Kernot
 Author-email: 874043@swansea.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

