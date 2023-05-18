# Comparing `tmp/pythonsqliextensionsV2-1.0.0.tar.gz` & `tmp/pythonsqliextensionsV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqliextensionsV2-1.0.0.tar", last modified: Thu May 18 16:59:56 2023, max compression
+gzip compressed data, was "pythonsqliextensionsV2-1.1.0.tar", last modified: Thu May 18 17:02:04 2023, max compression
```

## Comparing `pythonsqliextensionsV2-1.0.0.tar` & `pythonsqliextensionsV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:59:56.324224 pythonsqliextensionsV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-18 16:59:56.324224 pythonsqliextensionsV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:59:56.324224 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 16:59:56.000000 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:59:56.324224 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-18 16:59:56.000000 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-18 16:59:56.000000 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:59:56.000000 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 16:59:56.000000 pythonsqliextensionsV2-1.0.0/pythonsqliextensionsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 16:59:56.324224 pythonsqliextensionsV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-18 16:59:56.000000 pythonsqliextensionsV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:02:04.074674 pythonsqliextensionsV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-18 17:02:04.074674 pythonsqliextensionsV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:02:04.074674 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-05-18 17:02:03.000000 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 17:02:04.074674 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-18 17:02:04.000000 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-18 17:02:04.000000 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 17:02:04.000000 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 17:02:04.000000 pythonsqliextensionsV2-1.1.0/pythonsqliextensionsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 17:02:04.074674 pythonsqliextensionsV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-18 17:02:03.000000 pythonsqliextensionsV2-1.1.0/setup.py
```

### Comparing `pythonsqliextensionsV2-1.0.0/setup.py` & `pythonsqliextensionsV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythonsqliextensionsV2",
     version=VERSION,
```

