# Comparing `tmp/aioairzone-cloud-0.0.2.tar.gz` & `tmp/aioairzone-cloud-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.0.2.tar", last modified: Wed Apr 27 17:58:56 2022, max compression
+gzip compressed data, was "aioairzone-cloud-0.0.3.tar", last modified: Thu May 18 08:21:47 2023, max compression
```

## Comparing `aioairzone-cloud-0.0.2.tar` & `aioairzone-cloud-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2022-04-27 17:58:56.332653 aioairzone-cloud-0.0.2/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.2/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.2/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1237 2022-04-27 17:58:56.332653 aioairzone-cloud-0.0.2/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      319 2022-04-06 08:44:13.000000 aioairzone-cloud-0.0.2/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2022-04-27 17:58:56.328653 aioairzone-cloud-0.0.2/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    12864 2022-04-27 17:54:29.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4225 2022-04-06 19:26:33.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2890 2022-04-06 19:36:15.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      624 2022-04-06 08:18:59.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1168 2022-04-06 10:44:53.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3775 2022-04-06 08:42:41.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    17976 2022-04-06 19:27:54.000000 aioairzone-cloud-0.0.2/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2022-04-27 17:58:56.332653 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1237 2022-04-27 17:58:56.000000 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      587 2022-04-27 17:58:56.000000 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2022-04-27 17:58:56.000000 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2022-04-27 17:58:56.000000 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-04-27 17:58:56.000000 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2022-04-27 17:58:56.000000 aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.2/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2022-04-27 17:58:56.332653 aioairzone-cloud-0.0.2/setup.cfg
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1186 2022-04-27 17:55:32.000000 aioairzone-cloud-0.0.2/setup.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.3/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.3/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.3/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    12864 2022-04-27 17:54:29.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4225 2022-04-06 19:26:33.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2890 2022-04-06 19:36:15.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      624 2022-04-06 08:18:59.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1168 2022-04-06 10:44:53.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3775 2022-04-06 08:42:41.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    17976 2022-04-06 19:27:54.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-18 08:20:12.000000 aioairzone-cloud-0.0.3/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.3/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/setup.cfg
```

### Comparing `aioairzone-cloud-0.0.2/LICENSE` & `aioairzone-cloud-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/PKG-INFO` & `aioairzone-cloud-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to control Airzone Cloud devices
-Home-page: https://github.com/Noltari/aioairzone-cloud
-Author: Álvaro Fernández Rojas
-Author-email: noltari@gmail.com
+Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
-Download-URL: https://github.com/Noltari/aioairzone-cloud
-Description: # aioairzone-cloud
-        Python library to control Airzone Cloud devices.
-        
-        ## Requirements
-        - Python >= 3.8
-        
-        ## Install
-        ```bash
-        pip install aioairzone-cloud
-        ```
-        
-        ## Install from Source
-        Run the following command inside this folder
-        ```bash
-        pip install --upgrade .
-        ```
-        
-        ## Examples
-        Examples can be found in the `examples` folder
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
+Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
+Keywords: airzone,cloud,hvac,home
+Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aioairzone-cloud
+Python library to control Airzone Cloud devices.
+
+## Requirements
+- Python >= 3.10
+
+## Install
+```bash
+pip install aioairzone-cloud
+```
+
+## Install from Source
+Run the following command inside this folder
+```bash
+pip install --upgrade .
+```
+
+## Examples
+Examples can be found in the `examples` folder
```

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/cloudapi.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/common.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/const.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/device.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.0.3/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to control Airzone Cloud devices
-Home-page: https://github.com/Noltari/aioairzone-cloud
-Author: Álvaro Fernández Rojas
-Author-email: noltari@gmail.com
+Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
-Download-URL: https://github.com/Noltari/aioairzone-cloud
-Description: # aioairzone-cloud
-        Python library to control Airzone Cloud devices.
-        
-        ## Requirements
-        - Python >= 3.8
-        
-        ## Install
-        ```bash
-        pip install aioairzone-cloud
-        ```
-        
-        ## Install from Source
-        Run the following command inside this folder
-        ```bash
-        pip install --upgrade .
-        ```
-        
-        ## Examples
-        Examples can be found in the `examples` folder
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
+Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
+Keywords: airzone,cloud,hvac,home
+Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aioairzone-cloud
+Python library to control Airzone Cloud devices.
+
+## Requirements
+- Python >= 3.10
+
+## Install
+```bash
+pip install aioairzone-cloud
+```
+
+## Install from Source
+Run the following command inside this folder
+```bash
+pip install --upgrade .
+```
+
+## Examples
+Examples can be found in the `examples` folder
```

### Comparing `aioairzone-cloud-0.0.2/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
-setup.py
 aioairzone_cloud/__init__.py
 aioairzone_cloud/cloudapi.py
 aioairzone_cloud/common.py
 aioairzone_cloud/const.py
 aioairzone_cloud/device.py
 aioairzone_cloud/exceptions.py
 aioairzone_cloud/installation.py
```

