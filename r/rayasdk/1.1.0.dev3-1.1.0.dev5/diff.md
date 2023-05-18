# Comparing `tmp/rayasdk-1.1.0.dev3.tar.gz` & `tmp/rayasdk-1.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.0.dev3.tar", last modified: Thu May 18 03:49:44 2023, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev5.tar", last modified: Thu May 18 04:41:17 2023, max compression
```

## Comparing `rayasdk-1.1.0.dev3.tar` & `rayasdk-1.1.0.dev5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev3/README.md
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/__init__.py
--rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5154 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5150 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/connect.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6198 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk/container_handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev3/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5576 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2568 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/initializer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1342 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/killer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1513 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      819 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/messages.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     5993 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev3/rayasdk/runner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4396 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/scanner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1749 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev3/rayasdk/simulator.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2667 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk/template/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev3/rayasdk/template/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev3/rayasdk/template/app.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev3/rayasdk/template/launch.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev3/rayasdk/template/manifest.json
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3252 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/utils.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    11007 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev3/rayasdk/vcs.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/rayasdk.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      115 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-18 03:49:44.000000 rayasdk-1.1.0.dev3/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-18 03:49:44.264396 rayasdk-1.1.0.dev3/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1253 2023-05-18 03:47:17.000000 rayasdk-1.1.0.dev3/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6219 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev5/README.md
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/rayasdk/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/__init__.py
+-rwxrwxr-x   0 camilo    (1000) camilo    (1000)     5154 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev5/rayasdk/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5150 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/connect.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6198 2023-05-18 04:14:54.000000 rayasdk-1.1.0.dev5/rayasdk/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/rayasdk/container_handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev5/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5576 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev5/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2568 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/initializer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1342 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/killer.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1513 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev5/rayasdk/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      819 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/messages.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     5993 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev5/rayasdk/runner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4396 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/scanner.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1749 2023-05-11 21:39:47.000000 rayasdk-1.1.0.dev5/rayasdk/simulator.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2667 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/rayasdk/template/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev5/rayasdk/template/__main__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      551 2023-05-11 21:25:17.000000 rayasdk-1.1.0.dev5/rayasdk/template/app.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-04-17 17:27:42.000000 rayasdk-1.1.0.dev5/rayasdk/template/launch.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2023-02-22 08:37:00.000000 rayasdk-1.1.0.dev5/rayasdk/template/manifest.json
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3252 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev5/rayasdk/utils.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    11007 2023-05-17 15:09:08.000000 rayasdk-1.1.0.dev5/rayasdk/vcs.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/rayasdk.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6569 2023-05-18 04:41:17.000000 rayasdk-1.1.0.dev5/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      683 2023-05-18 04:41:17.000000 rayasdk-1.1.0.dev5/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 04:41:17.000000 rayasdk-1.1.0.dev5/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2023-05-18 04:41:17.000000 rayasdk-1.1.0.dev5/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      115 2023-05-18 04:41:17.000000 rayasdk-1.1.0.dev5/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2023-05-18 04:41:17.000000 rayasdk-1.1.0.dev5/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2023-05-18 04:41:17.973898 rayasdk-1.1.0.dev5/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1253 2023-05-18 04:17:06.000000 rayasdk-1.1.0.dev5/setup.py
```

### Comparing `rayasdk-1.1.0.dev3/PKG-INFO` & `rayasdk-1.1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev3
+Version: 1.1.0.dev5
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev3/README.md` & `rayasdk-1.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/__init__.py` & `rayasdk-1.1.0.dev5/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/__main__.py` & `rayasdk-1.1.0.dev5/rayasdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/connect.py` & `rayasdk-1.1.0.dev5/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/constants.py` & `rayasdk-1.1.0.dev5/rayasdk/constants.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/container_handlers/docker_handler.py` & `rayasdk-1.1.0.dev5/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/initializer.py` & `rayasdk-1.1.0.dev5/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/killer.py` & `rayasdk-1.1.0.dev5/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/logger.py` & `rayasdk-1.1.0.dev5/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/messages.py` & `rayasdk-1.1.0.dev5/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/runner.py` & `rayasdk-1.1.0.dev5/rayasdk/runner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/scanner.py` & `rayasdk-1.1.0.dev5/rayasdk/scanner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/simulator.py` & `rayasdk-1.1.0.dev5/rayasdk/simulator.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/sshKeyGen.py` & `rayasdk-1.1.0.dev5/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/template/app.py` & `rayasdk-1.1.0.dev5/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/utils.py` & `rayasdk-1.1.0.dev5/rayasdk/utils.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk/vcs.py` & `rayasdk-1.1.0.dev5/rayasdk/vcs.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.0.dev5/rayasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.0.dev3
+Version: 1.1.0.dev5
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
 Platform: UNKNOWN
```

### Comparing `rayasdk-1.1.0.dev3/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev5/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev3/setup.py` & `rayasdk-1.1.0.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pip_tools import get_last_release_version, get_last_prerelease_version
 
-VERSION = '1.1.0.dev3'
+VERSION = '1.1.0.dev5'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 if 'dev' in VERSION:
     RAYA_VERSION = get_last_prerelease_version('raya')
 else:
```

