# Comparing `tmp/wyzard-0.1b1.tar.gz` & `tmp/wyzard-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyzard-0.1b1.tar", last modified: Thu May 18 05:45:49 2023, max compression
+gzip compressed data, was "wyzard-1.0.tar", last modified: Thu May 18 06:10:14 2023, max compression
```

## Comparing `wyzard-0.1b1.tar` & `wyzard-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:45:49.728765 wyzard-0.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 05:45:37.000000 wyzard-0.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-18 05:45:49.724765 wyzard-0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-18 05:45:37.000000 wyzard-0.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 05:45:49.728765 wyzard-0.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-18 05:45:37.000000 wyzard-0.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:45:49.724765 wyzard-0.1b1/wyzard/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-18 05:45:37.000000 wyzard-0.1b1/wyzard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 05:45:37.000000 wyzard-0.1b1/wyzard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-18 05:45:37.000000 wyzard-0.1b1/wyzard/gpt_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-18 05:45:37.000000 wyzard-0.1b1/wyzard/image_captioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-18 05:45:37.000000 wyzard-0.1b1/wyzard/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 05:45:37.000000 wyzard-0.1b1/wyzard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:45:49.724765 wyzard-0.1b1/wyzard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-18 05:45:49.000000 wyzard-0.1b1/wyzard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-18 05:45:49.000000 wyzard-0.1b1/wyzard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:45:49.000000 wyzard-0.1b1/wyzard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 05:45:49.000000 wyzard-0.1b1/wyzard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 05:45:49.000000 wyzard-0.1b1/wyzard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:14.182495 wyzard-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 06:10:02.000000 wyzard-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-18 06:10:14.182495 wyzard-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-18 06:10:02.000000 wyzard-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:10:14.182495 wyzard-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-18 06:10:02.000000 wyzard-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:14.182495 wyzard-1.0/wyzard/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 06:10:02.000000 wyzard-1.0/wyzard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 06:10:02.000000 wyzard-1.0/wyzard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-18 06:10:02.000000 wyzard-1.0/wyzard/gpt_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-18 06:10:02.000000 wyzard-1.0/wyzard/image_captioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-18 06:10:02.000000 wyzard-1.0/wyzard/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-18 06:10:02.000000 wyzard-1.0/wyzard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:14.182495 wyzard-1.0/wyzard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-18 06:10:14.000000 wyzard-1.0/wyzard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-18 06:10:14.000000 wyzard-1.0/wyzard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:10:14.000000 wyzard-1.0/wyzard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 06:10:14.000000 wyzard-1.0/wyzard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 06:10:14.000000 wyzard-1.0/wyzard.egg-info/top_level.txt
```

### Comparing `wyzard-0.1b1/LICENSE` & `wyzard-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/PKG-INFO` & `wyzard-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyzard
-Version: 0.1b1
+Version: 1.0
 Summary: Run various transformers models from one packages.
 Home-page: https://github.com/LyQuid12/Wyzard
 Author: LyQuid
 Author-email: lyquidpersonal@gmail.com
 License: MIT License
 Project-URL: Source Code, https://github.com/LyQuid12/Wyzard
 Project-URL: Discord, https://discord.gg/qpT2AeYZRN
```

### Comparing `wyzard-0.1b1/README.md` & `wyzard-1.0/README.md`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/setup.py` & `wyzard-1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/wyzard/exceptions.py` & `wyzard-1.0/wyzard/exceptions.py`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/wyzard/gpt_detector.py` & `wyzard-1.0/wyzard/gpt_detector.py`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/wyzard/image_captioning.py` & `wyzard-1.0/wyzard/image_captioning.py`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/wyzard/object_detection.py` & `wyzard-1.0/wyzard/object_detection.py`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/wyzard/utils.py` & `wyzard-1.0/wyzard/utils.py`

 * *Files identical despite different names*

### Comparing `wyzard-0.1b1/wyzard.egg-info/PKG-INFO` & `wyzard-1.0/wyzard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyzard
-Version: 0.1b1
+Version: 1.0
 Summary: Run various transformers models from one packages.
 Home-page: https://github.com/LyQuid12/Wyzard
 Author: LyQuid
 Author-email: lyquidpersonal@gmail.com
 License: MIT License
 Project-URL: Source Code, https://github.com/LyQuid12/Wyzard
 Project-URL: Discord, https://discord.gg/qpT2AeYZRN
```

