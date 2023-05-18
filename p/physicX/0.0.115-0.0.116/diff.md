# Comparing `tmp/physicX-0.0.115.tar.gz` & `tmp/physicX-0.0.116.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicX-0.0.115.tar", last modified: Wed Apr 19 22:45:09 2023, max compression
+gzip compressed data, was "physicX-0.0.116.tar", last modified: Thu May 18 08:30:50 2023, max compression
```

## Comparing `physicX-0.0.115.tar` & `physicX-0.0.116.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      826 2023-04-19 22:45:09.101896 physicX-0.0.115/PKG-INFO
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      260 2023-04-14 12:09:52.000000 physicX-0.0.115/README.md
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      771 2023-04-19 22:44:38.000000 physicX-0.0.115/pyproject.toml
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-04-19 22:02:53.000000 physicX-0.0.115/requirements.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       38 2023-04-19 22:45:09.101896 physicX-0.0.115/setup.cfg
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/src/
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/src/physicX/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       50 2023-04-14 12:09:52.000000 physicX-0.0.115/src/physicX/__init__.py
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      402 2023-04-19 22:37:55.000000 physicX-0.0.115/src/physicX/constants.py
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-04-19 22:45:09.101896 physicX-0.0.115/src/physicX.egg-info/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      826 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/PKG-INFO
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      264 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/SOURCES.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)        1 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/dependency_links.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/requires.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)        8 2023-04-19 22:45:09.000000 physicX-0.0.115/src/physicX.egg-info/top_level.txt
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-05-18 08:30:50.443793 physicX-0.0.116/
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      829 2023-05-18 08:30:50.443793 physicX-0.0.116/PKG-INFO
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      263 2023-05-18 08:28:16.000000 physicX-0.0.116/README.md
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      771 2023-05-18 08:28:16.000000 physicX-0.0.116/pyproject.toml
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-05-18 08:28:16.000000 physicX-0.0.116/requirements.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       38 2023-05-18 08:30:50.443793 physicX-0.0.116/setup.cfg
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-05-18 08:30:50.443793 physicX-0.0.116/src/
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-05-18 08:30:50.443793 physicX-0.0.116/src/physicX/
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       50 2023-05-18 08:28:16.000000 physicX-0.0.116/src/physicX/__init__.py
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      369 2023-05-18 08:28:16.000000 physicX-0.0.116/src/physicX/constants.py
+drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-05-18 08:30:50.443793 physicX-0.0.116/src/physicX.egg-info/
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      829 2023-05-18 08:30:50.000000 physicX-0.0.116/src/physicX.egg-info/PKG-INFO
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)      264 2023-05-18 08:30:50.000000 physicX-0.0.116/src/physicX.egg-info/SOURCES.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)        1 2023-05-18 08:30:50.000000 physicX-0.0.116/src/physicX.egg-info/dependency_links.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-05-18 08:30:50.000000 physicX-0.0.116/src/physicX.egg-info/requires.txt
+-rw-r--r--   0 cunknown  (1000) cunknown  (1000)        8 2023-05-18 08:30:50.000000 physicX-0.0.116/src/physicX.egg-info/top_level.txt
```

### Comparing `physicX-0.0.115/PKG-INFO` & `physicX-0.0.116/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.115
+Version: 0.0.116
 Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Other OS
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PhysicX library for python
+  
 This project with LICENSE GNU-GPLv3, in fact created for developers , physicist , mathematicians and this project
 <pre>pre-released</pre>
 github:https://github.com/anonymous14725/physicX <br/>
 pypi:https://pypi.org/project/physicX
```

### Comparing `physicX-0.0.115/pyproject.toml` & `physicX-0.0.116/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["setuptools>=61.0","numpy>=1.19.2"]
+requires = ["setuptools>=61.0","numpy>=1.24.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "physicX"
-version = "0.0.115"
+version = "0.0.116"
 authors = [
   { name="anonymous14725", email="anonymous14725@yahoo.com" },
 ]
 description = "mathematics and physics library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `physicX-0.0.115/src/physicX.egg-info/PKG-INFO` & `physicX-0.0.116/src/physicX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.115
+Version: 0.0.116
 Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Other OS
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PhysicX library for python
+  
 This project with LICENSE GNU-GPLv3, in fact created for developers , physicist , mathematicians and this project
 <pre>pre-released</pre>
 github:https://github.com/anonymous14725/physicX <br/>
 pypi:https://pypi.org/project/physicX
```

