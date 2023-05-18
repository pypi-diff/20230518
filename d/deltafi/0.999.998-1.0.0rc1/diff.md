# Comparing `tmp/deltafi-0.999.998.tar.gz` & `tmp/deltafi-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-0.999.998.tar", max compression
+gzip compressed data, was "deltafi-1.0.0rc1.tar", max compression
```

## Comparing `deltafi-0.999.998.tar` & `deltafi-1.0.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-0.999.998/README.md
--rw-r--r--   0        0        0      706 2023-04-10 13:34:58.932322 deltafi-0.999.998/deltafi/__init__.py
--rw-r--r--   0        0        0     7326 2023-05-17 20:43:32.059753 deltafi-0.999.998/deltafi/action.py
--rw-r--r--   0        0        0     1981 2023-04-10 13:34:58.932322 deltafi-0.999.998/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      985 2023-05-17 20:43:32.059753 deltafi-0.999.998/deltafi/actiontype.py
--rw-r--r--   0        0        0    11019 2023-05-17 20:43:32.060753 deltafi-0.999.998/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-0.999.998/deltafi/exception.py
--rw-r--r--   0        0        0     6284 2023-05-17 20:43:32.060753 deltafi-0.999.998/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-0.999.998/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-0.999.998/deltafi/metric.py
--rw-r--r--   0        0        0     8553 2023-05-08 15:00:28.699314 deltafi-0.999.998/deltafi/plugin.py
--rw-r--r--   0        0        0     9972 2023-05-17 20:43:32.061753 deltafi-0.999.998/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-0.999.998/deltafi/storage.py
--rw-r--r--   0        0        0     1281 2023-05-18 05:03:49.571172 deltafi-0.999.998/pyproject.toml
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 deltafi-0.999.998/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:32:51.621370 deltafi-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      706 2023-04-10 13:32:51.622370 deltafi-1.0.0rc1/deltafi/__init__.py
+-rw-r--r--   0        0        0     7326 2023-05-16 13:45:16.568554 deltafi-1.0.0rc1/deltafi/action.py
+-rw-r--r--   0        0        0     1981 2023-04-10 13:32:51.622370 deltafi-1.0.0rc1/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      985 2023-05-16 13:45:16.569555 deltafi-1.0.0rc1/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11019 2023-05-17 20:40:37.760691 deltafi-1.0.0rc1/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-26 13:21:52.730906 deltafi-1.0.0rc1/deltafi/exception.py
+-rw-r--r--   0        0        0     6284 2023-05-16 13:45:16.569555 deltafi-1.0.0rc1/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:32:51.623371 deltafi-1.0.0rc1/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:32:51.623371 deltafi-1.0.0rc1/deltafi/metric.py
+-rw-r--r--   0        0        0     8553 2023-05-08 14:58:59.555208 deltafi-1.0.0rc1/deltafi/plugin.py
+-rw-r--r--   0        0        0     9972 2023-05-17 20:40:37.760691 deltafi-1.0.0rc1/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:40:37.760691 deltafi-1.0.0rc1/deltafi/storage.py
+-rw-r--r--   0        0        0     1281 2023-05-18 01:53:26.403686 deltafi-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-1.0.0rc1/PKG-INFO
```

### Comparing `deltafi-0.999.998/deltafi/__init__.py` & `deltafi-1.0.0rc1/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/action.py` & `deltafi-1.0.0rc1/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/actioneventqueue.py` & `deltafi-1.0.0rc1/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/actiontype.py` & `deltafi-1.0.0rc1/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/domain.py` & `deltafi-1.0.0rc1/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/exception.py` & `deltafi-1.0.0rc1/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/input.py` & `deltafi-1.0.0rc1/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/logger.py` & `deltafi-1.0.0rc1/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/metric.py` & `deltafi-1.0.0rc1/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/plugin.py` & `deltafi-1.0.0rc1/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/result.py` & `deltafi-1.0.0rc1/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/deltafi/storage.py` & `deltafi-1.0.0rc1/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.999.998/pyproject.toml` & `deltafi-1.0.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "0.999.998"
+version = "1.0.0-RC1"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-0.999.998/PKG-INFO` & `deltafi-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 0.999.998
+Version: 1.0.0rc1
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

