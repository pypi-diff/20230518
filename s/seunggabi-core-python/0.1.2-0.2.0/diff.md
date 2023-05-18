# Comparing `tmp/seunggabi_core_python-0.1.2.tar.gz` & `tmp/seunggabi_core_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seunggabi_core_python-0.1.2.tar", last modified: Mon May 15 15:03:28 2023, max compression
+gzip compressed data, was "seunggabi_core_python-0.2.0.tar", last modified: Thu May 18 14:05:14 2023, max compression
```

## Comparing `seunggabi_core_python-0.1.2.tar` & `seunggabi_core_python-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 15:03:28.771450 seunggabi_core_python-0.1.2/
--rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.1.2/LICENSE
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-15 15:03:28.771334 seunggabi_core_python-0.1.2/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      332 2023-05-15 13:55:58.000000 seunggabi_core_python-0.1.2/README.md
--rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-05-15 15:03:28.771479 seunggabi_core_python-0.1.2/setup.cfg
--rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.1.2/setup.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 15:03:28.770039 seunggabi_core_python-0.1.2/seunggabi_core_python/
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-15 15:03:25.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/const.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 15:03:28.770756 seunggabi_core_python-0.1.2/seunggabi_core_python/exception/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/exception/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)       95 2023-05-15 12:54:12.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/exception/bad_request.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 15:03:28.771177 seunggabi_core_python-0.1.2/seunggabi_core_python/util/
--rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/util/__init__.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      767 2023-05-15 15:02:45.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/util/config_util.py
--rw-r--r--   0 seunggabi   (501) staff       (20)      142 2023-05-13 14:44:24.000000 seunggabi_core_python-0.1.2/seunggabi_core_python/util/json_util.py
-drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-15 15:03:28.770492 seunggabi_core_python-0.1.2/seunggabi_core_python.egg-info/
--rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-15 15:03:28.000000 seunggabi_core_python-0.1.2/seunggabi_core_python.egg-info/PKG-INFO
--rw-r--r--   0 seunggabi   (501) staff       (20)      483 2023-05-15 15:03:28.000000 seunggabi_core_python-0.1.2/seunggabi_core_python.egg-info/SOURCES.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-05-15 15:03:28.000000 seunggabi_core_python-0.1.2/seunggabi_core_python.egg-info/dependency_links.txt
--rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-15 15:03:28.000000 seunggabi_core_python-0.1.2/seunggabi_core_python.egg-info/top_level.txt
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.066094 seunggabi_core_python-0.2.0/
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1070 2023-05-13 14:31:33.000000 seunggabi_core_python-0.2.0/LICENSE
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-18 14:05:14.065955 seunggabi_core_python-0.2.0/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      362 2023-05-18 14:04:41.000000 seunggabi_core_python-0.2.0/README.md
+-rw-r--r--   0 seunggabi   (501) staff       (20)       38 2023-05-18 14:05:14.066124 seunggabi_core_python-0.2.0/setup.cfg
+-rw-r--r--   0 seunggabi   (501) staff       (20)      746 2023-05-15 13:20:26.000000 seunggabi_core_python-0.2.0/setup.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.064212 seunggabi_core_python-0.2.0/seunggabi_core_python/
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-18 14:05:01.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       48 2023-05-15 13:10:17.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/const.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.065029 seunggabi_core_python-0.2.0/seunggabi_core_python/exception/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-15 12:46:34.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/exception/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)       95 2023-05-15 12:54:12.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/exception/bad_request.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.065738 seunggabi_core_python-0.2.0/seunggabi_core_python/util/
+-rw-r--r--   0 seunggabi   (501) staff       (20)        0 2023-05-13 15:22:13.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/__init__.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)     1001 2023-05-17 20:21:40.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/arg_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      781 2023-05-15 15:07:17.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/config_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      149 2023-05-15 15:07:03.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/json_util.py
+-rw-r--r--   0 seunggabi   (501) staff       (20)      193 2023-05-18 13:38:22.000000 seunggabi_core_python-0.2.0/seunggabi_core_python/util/request_util.py
+drwxr-xr-x   0 seunggabi   (501) staff       (20)        0 2023-05-18 14:05:14.064698 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/
+-rw-r--r--   0 seunggabi   (501) staff       (20)      573 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/PKG-INFO
+-rw-r--r--   0 seunggabi   (501) staff       (20)      565 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/SOURCES.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)        1 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/dependency_links.txt
+-rw-r--r--   0 seunggabi   (501) staff       (20)       22 2023-05-18 14:05:14.000000 seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/top_level.txt
```

### Comparing `seunggabi_core_python-0.1.2/LICENSE` & `seunggabi_core_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.1.2/PKG-INFO` & `seunggabi_core_python-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seunggabi_core_python
-Version: 0.1.2
+Version: 0.2.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seunggabi_core_python-0.1.2/setup.py` & `seunggabi_core_python-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `seunggabi_core_python-0.1.2/seunggabi_core_python/util/config_util.py` & `seunggabi_core_python-0.2.0/seunggabi_core_python/util/config_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 from configparser import ConfigParser
 
 from seunggabi_core_python.const import DEFAULT, CREDENTIALS
 from seunggabi_core_python.exception.bad_request import BadRequest
 
 
-def home():
+def home() -> str:
     return os.path.expanduser("~")
 
 
 def path(
     group: str = None,
     context: str = None,
-):
+) -> str:
     return f".{group}/{context}"
 
 
 def get(
     group: str = None,
     context: str = None,
     profile: str = None,
```

### Comparing `seunggabi_core_python-0.1.2/seunggabi_core_python.egg-info/PKG-INFO` & `seunggabi_core_python-0.2.0/seunggabi_core_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seunggabi-core-python
-Version: 0.1.2
+Version: 0.2.0
 Summary: A collection of core Python modules
 Home-page: https://github.com/seunggabi/core_python
 Author: seunggabi
 Author-email: seunggabi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

