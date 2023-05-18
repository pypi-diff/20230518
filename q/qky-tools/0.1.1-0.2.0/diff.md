# Comparing `tmp/qky-tools-0.1.1.tar.gz` & `tmp/qky-tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qky-tools-0.1.1.tar", last modified: Thu May 18 01:20:45 2023, max compression
+gzip compressed data, was "qky-tools-0.2.0.tar", last modified: Thu May 18 01:22:35 2023, max compression
```

## Comparing `qky-tools-0.1.1.tar` & `qky-tools-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:20:45.464656 qky-tools-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-05-18 00:09:54.000000 qky-tools-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      690 2023-05-18 01:20:45.462661 qky-tools-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-18 00:10:33.000000 qky-tools-0.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 01:20:45.435738 qky-tools-0.1.1/db/
--rw-rw-rw-   0        0        0     5338 2023-05-18 00:24:47.000000 qky-tools-0.1.1/db/MySQL.py
--rw-rw-rw-   0        0        0        0 2023-05-18 00:18:21.000000 qky-tools-0.1.1/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:20:45.453685 qky-tools-0.1.1/qky_tools.egg-info/
--rw-rw-rw-   0        0        0      690 2023-05-18 01:20:45.000000 qky-tools-0.1.1/qky_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-18 01:20:45.000000 qky-tools-0.1.1/qky_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:20:45.000000 qky-tools-0.1.1/qky_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 01:20:45.000000 qky-tools-0.1.1/qky_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 01:20:45.000000 qky-tools-0.1.1/qky_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 01:20:45.458671 qky-tools-0.1.1/req/
--rw-rw-rw-   0        0        0        0 2023-05-18 00:54:44.000000 qky-tools-0.1.1/req/__init__.py
--rw-rw-rw-   0        0        0     3250 2023-05-18 01:19:46.000000 qky-tools-0.1.1/req/cacheReq.py
--rw-rw-rw-   0        0        0      191 2023-05-18 01:01:36.000000 qky-tools-0.1.1/req/proxy.py
--rw-rw-rw-   0        0        0       42 2023-05-18 01:20:45.464656 qky-tools-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3932 2023-05-18 01:20:42.000000 qky-tools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:22:35.525253 qky-tools-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-18 00:09:54.000000 qky-tools-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      690 2023-05-18 01:22:35.525253 qky-tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:10:33.000000 qky-tools-0.2.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 01:22:35.509295 qky-tools-0.2.0/db/
+-rw-rw-rw-   0        0        0     5338 2023-05-18 00:24:47.000000 qky-tools-0.2.0/db/MySQL.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:18:21.000000 qky-tools-0.2.0/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:22:35.520267 qky-tools-0.2.0/qky_tools.egg-info/
+-rw-rw-rw-   0        0        0      690 2023-05-18 01:22:35.000000 qky-tools-0.2.0/qky_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-18 01:22:35.000000 qky-tools-0.2.0/qky_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:22:35.000000 qky-tools-0.2.0/qky_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 01:22:35.000000 qky-tools-0.2.0/qky_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 01:22:35.000000 qky-tools-0.2.0/qky_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 01:22:35.523258 qky-tools-0.2.0/req/
+-rw-rw-rw-   0        0        0        0 2023-05-18 00:54:44.000000 qky-tools-0.2.0/req/__init__.py
+-rw-rw-rw-   0        0        0     3250 2023-05-18 01:19:46.000000 qky-tools-0.2.0/req/cacheReq.py
+-rw-rw-rw-   0        0        0      191 2023-05-18 01:01:36.000000 qky-tools-0.2.0/req/proxy.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:22:35.526250 qky-tools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3932 2023-05-18 01:22:03.000000 qky-tools-0.2.0/setup.py
```

### Comparing `qky-tools-0.1.1/LICENSE.txt` & `qky-tools-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qky-tools-0.1.1/PKG-INFO` & `qky-tools-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qky-tools
-Version: 0.1.1
+Version: 0.2.0
 Summary: python tools collection
 Home-page: https://github.com/qiaokuoyuan/py-tools
 Author: qiaokuoyuan
 Author-email: 457361577@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qky-tools-0.1.1/db/MySQL.py` & `qky-tools-0.2.0/db/MySQL.py`

 * *Files identical despite different names*

### Comparing `qky-tools-0.1.1/qky_tools.egg-info/PKG-INFO` & `qky-tools-0.2.0/qky_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qky-tools
-Version: 0.1.1
+Version: 0.2.0
 Summary: python tools collection
 Home-page: https://github.com/qiaokuoyuan/py-tools
 Author: qiaokuoyuan
 Author-email: 457361577@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qky-tools-0.1.1/req/cacheReq.py` & `qky-tools-0.2.0/req/cacheReq.py`

 * *Files identical despite different names*

### Comparing `qky-tools-0.1.1/setup.py` & `qky-tools-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'qky-tools'
 DESCRIPTION = 'python tools collection'
 URL = 'https://github.com/qiaokuoyuan/py-tools'
 EMAIL = '457361577@qq.com'
 AUTHOR = 'qiaokuoyuan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     'pymysql', 'nanoid'
 ]
```

