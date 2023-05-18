# Comparing `tmp/skytek-utils-0.2.0.tar.gz` & `tmp/skytek-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek-utils-0.2.0.tar", last modified: Tue May  9 19:05:07 2023, max compression
+gzip compressed data, was "skytek-utils-0.3.0.tar", last modified: Thu May 18 11:35:23 2023, max compression
```

## Comparing `skytek-utils-0.2.0.tar` & `skytek-utils-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.791386 skytek-utils-0.2.0/skytek_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:04:57.000000 skytek-utils-0.2.0/skytek_utils/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/skytek_utils/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/skytek_utils/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/skytek_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 19:05:07.000000 skytek-utils-0.2.0/skytek_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:05:07.795386 skytek-utils-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-09 19:04:49.000000 skytek-utils-0.2.0/tests/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.444766 skytek-utils-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-18 11:35:23.444766 skytek-utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 11:35:23.444766 skytek-utils-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.440766 skytek-utils-0.3.0/skytek_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 11:35:16.000000 skytek-utils-0.3.0/skytek_utils/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.440766 skytek-utils-0.3.0/skytek_utils/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.440766 skytek-utils-0.3.0/skytek_utils/interconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.444766 skytek-utils-0.3.0/skytek_utils/interconnect/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/interconnect/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/skytek_utils/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.440766 skytek-utils-0.3.0/skytek_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-18 11:35:23.000000 skytek-utils-0.3.0/skytek_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-18 11:35:23.000000 skytek-utils-0.3.0/skytek_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:35:23.000000 skytek-utils-0.3.0/skytek_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 11:35:23.000000 skytek-utils-0.3.0/skytek_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 11:35:23.000000 skytek-utils-0.3.0/skytek_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 11:35:23.444766 skytek-utils-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-18 11:35:14.000000 skytek-utils-0.3.0/tests/test_iter.py
```

### Comparing `skytek-utils-0.2.0/LICENSE` & `skytek-utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.2.0/PKG-INFO` & `skytek-utils-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.2.0/setup.py` & `skytek-utils-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.2.0/skytek_utils/celery.py` & `skytek-utils-0.3.0/skytek_utils/celery.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.2.0/skytek_utils/datetime.py` & `skytek-utils-0.3.0/skytek_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.2.0/skytek_utils/json_stream.py` & `skytek-utils-0.3.0/skytek_utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.2.0/skytek_utils/monitoring.py` & `skytek-utils-0.3.0/skytek_utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `skytek-utils-0.2.0/skytek_utils.egg-info/PKG-INFO` & `skytek-utils-0.3.0/skytek_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: skytek-utils - a set of small util functions
 Home-page: http://github.com/Skytek/skytek-utils
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek-utils-0.2.0/skytek_utils.egg-info/SOURCES.txt` & `skytek-utils-0.3.0/skytek_utils.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,8 +15,16 @@
 skytek_utils.egg-info/SOURCES.txt
 skytek_utils.egg-info/dependency_links.txt
 skytek_utils.egg-info/not-zip-safe
 skytek_utils.egg-info/top_level.txt
 skytek_utils/django/__init__.py
 skytek_utils/django/forms.py
 skytek_utils/django/models.py
+skytek_utils/interconnect/__init__.py
+skytek_utils/interconnect/api/__init__.py
+skytek_utils/interconnect/api/authentication.py
+skytek_utils/interconnect/api/client.py
+skytek_utils/interconnect/api/jwt.py
+skytek_utils/interconnect/api/mixins.py
+skytek_utils/interconnect/api/permissions.py
+skytek_utils/interconnect/api/user.py
 tests/test_iter.py
```

### Comparing `skytek-utils-0.2.0/tests/test_iter.py` & `skytek-utils-0.3.0/tests/test_iter.py`

 * *Files identical despite different names*

