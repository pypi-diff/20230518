# Comparing `tmp/antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4.tar.gz` & `tmp/antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4.tar", last modified: Mon May 15 06:16:51 2023, max compression
+gzip compressed data, was "dist/antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5.tar", last modified: Thu May 18 09:00:29 2023, max compression
```

## Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4.tar` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17762 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/client.py
--rw-r--r--   0 root         (0) root         (0)    10929 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-15 06:16:51.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28014 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/client.py
+-rw-r--r--   0 root         (0) root         (0)    28837 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_sdk_ak_50c620ebd72240219637191db5c3441d/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-18 09:00:29.000000 antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/setup.py
```

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/LICENSE` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/PKG-INFO` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_50c620ebd72240219637191db5c3441d
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ant Chain Ak_50c620ebd72240219637191db5c3441d SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/README-CN.md` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/README.md` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/PKG-INFO` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-50c620ebd72240219637191db5c3441d
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ant Chain Ak_50c620ebd72240219637191db5c3441d SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/SOURCES.txt` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/antchain_ak_50c620ebd72240219637191db5c3441d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.4/setup.py` & `antchain_ak_50c620ebd72240219637191db5c3441d-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_50c620ebd72240219637191db5c3441d.
 
-Created on 15/05/2023
+Created on 18/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_50c620ebd72240219637191db5c3441d"
 NAME = "antchain_ak_50c620ebd72240219637191db5c3441d" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_50c620ebd72240219637191db5c3441d SDK Library for Python"
```

