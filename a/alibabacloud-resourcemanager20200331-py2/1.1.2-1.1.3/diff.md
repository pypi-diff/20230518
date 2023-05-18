# Comparing `tmp/alibabacloud_resourcemanager20200331_py2-1.1.2.tar.gz` & `tmp/alibabacloud_resourcemanager20200331_py2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcemanager20200331_py2-1.1.2.tar", last modified: Wed Feb 22 02:22:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcemanager20200331_py2-1.1.3.tar", last modified: Thu May 18 08:58:34 2023, max compression
```

## Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2.tar` & `alibabacloud_resourcemanager20200331_py2-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      457 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2544 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1152 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   110325 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331/client.py
--rw-r--r--   0 root         (0) root         (0)   510943 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2544 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-22 02:22:41.000000 alibabacloud_resourcemanager20200331_py2-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:58:34.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-18 08:58:34.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:58:34.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164634 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331/client.py
+-rw-r--r--   0 root         (0) root         (0)   594770 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 08:58:34.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 08:58:34.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-05-18 08:58:33.000000 alibabacloud_resourcemanager20200331_py2-1.1.3/setup.py
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/LICENSE` & `alibabacloud_resourcemanager20200331_py2-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/PKG-INFO` & `alibabacloud_resourcemanager20200331_py2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcemanager20200331_py2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/README-CN.md` & `alibabacloud_resourcemanager20200331_py2-1.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/README.md` & `alibabacloud_resourcemanager20200331_py2-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO` & `alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcemanager20200331-py2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud ResourceManager (20200331) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt` & `alibabacloud_resourcemanager20200331_py2-1.1.3/alibabacloud_resourcemanager20200331_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcemanager20200331_py2-1.1.2/setup.py` & `alibabacloud_resourcemanager20200331_py2-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcemanager20200331_py2.
 
-Created on 22/02/2023
+Created on 18/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcemanager20200331"
 NAME = "alibabacloud_resourcemanager20200331_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceManager (20200331) SDK Library for Python2"
```

