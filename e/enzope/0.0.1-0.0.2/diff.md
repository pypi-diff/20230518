# Comparing `tmp/enzope-0.0.1.tar.gz` & `tmp/enzope-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enzope-0.0.1.tar", last modified: Thu May 18 18:38:48 2023, max compression
+gzip compressed data, was "enzope-0.0.2.tar", last modified: Thu May 18 18:57:22 2023, max compression
```

## Comparing `enzope-0.0.1.tar` & `enzope-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1072 2023-05-18 18:19:34.000000 enzope-0.0.1/LICENSE
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      629 2023-05-18 18:38:48.468856 enzope-0.0.1/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      720 2023-05-18 18:18:01.000000 enzope-0.0.1/pyproject.toml
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       38 2023-05-18 18:38:48.468856 enzope-0.0.1/setup.cfg
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:36:25.000000 enzope-0.0.1/src/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/enzope.egg-info/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      629 2023-05-18 18:38:48.000000 enzope-0.0.1/src/enzope.egg-info/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      417 2023-05-18 18:38:48.000000 enzope-0.0.1/src/enzope.egg-info/SOURCES.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-05-18 18:38:48.000000 enzope-0.0.1/src/enzope.egg-info/dependency_links.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       43 2023-05-18 18:38:48.000000 enzope-0.0.1/src/enzope.egg-info/top_level.txt
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/graphs/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-12 15:11:48.000000 enzope-0.0.1/src/graphs/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6766 2023-05-12 15:20:06.000000 enzope-0.0.1/src/graphs/custom_gtg.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     4532 2023-05-15 13:39:45.000000 enzope-0.0.1/src/graphs/graph_class.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/kernels/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.1/src/kernels/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1368 2023-05-15 19:19:28.000000 enzope-0.0.1/src/kernels/k_ys.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      434 2023-05-13 20:26:31.000000 enzope-0.0.1/src/kernels/locks.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/model/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:36:37.000000 enzope-0.0.1/src/model/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6442 2023-05-15 16:53:38.000000 enzope-0.0.1/src/model/model_gpu.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/trades/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.1/src/trades/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/src/utils/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:24.000000 enzope-0.0.1/src/utils/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:38:48.468856 enzope-0.0.1/tests/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       37 2023-05-15 13:42:25.000000 enzope-0.0.1/tests/test.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1072 2023-05-18 18:19:34.000000 enzope-0.0.2/LICENSE
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      629 2023-05-18 18:57:22.172868 enzope-0.0.2/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      720 2023-05-18 18:55:58.000000 enzope-0.0.2/pyproject.toml
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       38 2023-05-18 18:57:22.172868 enzope-0.0.2/setup.cfg
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:36:25.000000 enzope-0.0.2/src/__init__.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/enzope.egg-info/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      629 2023-05-18 18:57:22.000000 enzope-0.0.2/src/enzope.egg-info/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      417 2023-05-18 18:57:22.000000 enzope-0.0.2/src/enzope.egg-info/SOURCES.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-05-18 18:57:22.000000 enzope-0.0.2/src/enzope.egg-info/dependency_links.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       43 2023-05-18 18:57:22.000000 enzope-0.0.2/src/enzope.egg-info/top_level.txt
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/graphs/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-12 15:11:48.000000 enzope-0.0.2/src/graphs/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6766 2023-05-12 15:20:06.000000 enzope-0.0.2/src/graphs/custom_gtg.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     4532 2023-05-15 13:39:45.000000 enzope-0.0.2/src/graphs/graph_class.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/kernels/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.2/src/kernels/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1368 2023-05-15 19:19:28.000000 enzope-0.0.2/src/kernels/k_ys.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      434 2023-05-13 20:26:31.000000 enzope-0.0.2/src/kernels/locks.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/model/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:36:37.000000 enzope-0.0.2/src/model/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6442 2023-05-15 16:53:38.000000 enzope-0.0.2/src/model/model_gpu.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/trades/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.2/src/trades/__init__.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/src/utils/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:24.000000 enzope-0.0.2/src/utils/__init__.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-05-18 18:57:22.172868 enzope-0.0.2/tests/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       37 2023-05-15 13:42:25.000000 enzope-0.0.2/tests/test.py
```

### Comparing `enzope-0.0.1/LICENSE` & `enzope-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enzope-0.0.1/PKG-INFO` & `enzope-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enzope
-Version: 0.0.1
+Version: 0.0.2
 Summary: Agent based modelling in complex networks
 Author-email: Lautaro Giordano <giordanolautaro@gmail.com>
 Project-URL: Homepage, https://github.com/lautarogiordano/enzope
 Project-URL: Bug Tracker, https://github.com/lautarogiordano/enzope/issues
 Keywords: Agent based modelling,complex networks,Yard Sale algorithm,random networks,econophysics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enzope-0.0.1/pyproject.toml` & `enzope-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "enzope"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lautaro Giordano", email="giordanolautaro@gmail.com" },
 ]
 description = "Agent based modelling in complex networks"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `enzope-0.0.1/src/enzope.egg-info/PKG-INFO` & `enzope-0.0.2/src/enzope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enzope
-Version: 0.0.1
+Version: 0.0.2
 Summary: Agent based modelling in complex networks
 Author-email: Lautaro Giordano <giordanolautaro@gmail.com>
 Project-URL: Homepage, https://github.com/lautarogiordano/enzope
 Project-URL: Bug Tracker, https://github.com/lautarogiordano/enzope/issues
 Keywords: Agent based modelling,complex networks,Yard Sale algorithm,random networks,econophysics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enzope-0.0.1/src/graphs/custom_gtg.py` & `enzope-0.0.2/src/graphs/custom_gtg.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.1/src/graphs/graph_class.py` & `enzope-0.0.2/src/graphs/graph_class.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.1/src/kernels/k_ys.py` & `enzope-0.0.2/src/kernels/k_ys.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.1/src/model/model_gpu.py` & `enzope-0.0.2/src/model/model_gpu.py`

 * *Files identical despite different names*

