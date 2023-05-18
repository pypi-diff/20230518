# Comparing `tmp/smartlogger-0.0.1.dev2.tar.gz` & `tmp/smartlogger-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartlogger-0.0.1.dev2.tar", last modified: Thu May 18 10:34:37 2023, max compression
+gzip compressed data, was "smartlogger-0.0.1.dev3.tar", last modified: Thu May 18 10:40:21 2023, max compression
```

## Comparing `smartlogger-0.0.1.dev2.tar` & `smartlogger-0.0.1.dev3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:34:37.509545 smartlogger-0.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 10:34:37.509545 smartlogger-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 10:34:20.000000 smartlogger-0.0.1.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 10:34:37.509545 smartlogger-0.0.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-18 10:34:20.000000 smartlogger-0.0.1.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:34:37.509545 smartlogger-0.0.1.dev2/smartlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 10:34:37.000000 smartlogger-0.0.1.dev2/smartlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-18 10:34:37.000000 smartlogger-0.0.1.dev2/smartlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:34:37.000000 smartlogger-0.0.1.dev2/smartlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 10:34:37.000000 smartlogger-0.0.1.dev2/smartlogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 10:34:37.000000 smartlogger-0.0.1.dev2/smartlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:34:37.000000 smartlogger-0.0.1.dev2/smartlogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:40:21.764284 smartlogger-0.0.1.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 10:40:21.764284 smartlogger-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 10:40:08.000000 smartlogger-0.0.1.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 10:40:21.764284 smartlogger-0.0.1.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-18 10:40:08.000000 smartlogger-0.0.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:40:21.764284 smartlogger-0.0.1.dev3/smartlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 10:40:21.000000 smartlogger-0.0.1.dev3/smartlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-18 10:40:21.000000 smartlogger-0.0.1.dev3/smartlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:40:21.000000 smartlogger-0.0.1.dev3/smartlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 10:40:21.000000 smartlogger-0.0.1.dev3/smartlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 10:40:21.000000 smartlogger-0.0.1.dev3/smartlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:40:21.000000 smartlogger-0.0.1.dev3/smartlogger.egg-info/top_level.txt
```

### Comparing `smartlogger-0.0.1.dev2/PKG-INFO` & `smartlogger-0.0.1.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlogger
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartlogger-0.0.1.dev2/README.md` & `smartlogger-0.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `smartlogger-0.0.1.dev2/setup.py` & `smartlogger-0.0.1.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartlogger"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev2"
+VERSION = "0.0.1.dev3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "liteindex"
 ]
```

### Comparing `smartlogger-0.0.1.dev2/smartlogger.egg-info/PKG-INFO` & `smartlogger-0.0.1.dev3/smartlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlogger
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

