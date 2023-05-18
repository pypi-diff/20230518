# Comparing `tmp/dodi-2.0.1.tar.gz` & `tmp/dodi-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dodi-2.0.1.tar", last modified: Wed Mar 29 14:50:18 2023, max compression
+gzip compressed data, was "dist/dodi-2.0.2.tar", last modified: Thu May 18 16:34:35 2023, max compression
```

## Comparing `dodi-2.0.1.tar` & `dodi-2.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-03-29 14:50:18.000000 dodi-2.0.1/
--rw-r--r--   0 alex       (502) staff       (20)     6488 2023-03-29 14:50:18.000000 dodi-2.0.1/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)       50 2022-04-08 13:51:07.000000 dodi-2.0.1/MANIFEST.in
--rw-r--r--   0 alex       (502) staff       (20)     5093 2022-08-26 21:26:17.000000 dodi-2.0.1/README.md
--rw-r--r--   0 alex       (502) staff       (20)      805 2023-03-29 14:39:43.000000 dodi-2.0.1/setup.py
--rw-r--r--   0 alex       (502) staff       (20)        5 2023-03-29 14:45:19.000000 dodi-2.0.1/VERSION
--rw-r--r--   0 alex       (502) staff       (20)      420 2023-03-29 14:46:21.000000 dodi-2.0.1/RELEASE_NOTES.md
--rw-r--r--   0 alex       (502) staff       (20)       38 2023-03-29 14:50:18.000000 dodi-2.0.1/setup.cfg
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-03-29 14:50:18.000000 dodi-2.0.1/src/
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi/
--rw-r--r--   0 alex       (502) staff       (20)     1876 2022-04-12 16:28:48.000000 dodi-2.0.1/src/dodi/validator.py
--rw-r--r--   0 alex       (502) staff       (20)     2065 2022-04-13 19:35:23.000000 dodi-2.0.1/src/dodi/_etag_responder.py
--rw-r--r--   0 alex       (502) staff       (20)       96 2022-04-11 21:52:49.000000 dodi-2.0.1/src/dodi/__init__.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi/__pycache__/
--rw-r--r--   0 alex       (502) staff       (20)      327 2022-04-08 21:19:37.000000 dodi-2.0.1/src/dodi/__pycache__/_exceptions.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     2944 2022-08-26 21:27:42.000000 dodi-2.0.1/src/dodi/__pycache__/_views.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     3595 2022-04-13 17:53:40.000000 dodi-2.0.1/src/dodi/__pycache__/_operations.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     2295 2022-04-13 19:35:25.000000 dodi-2.0.1/src/dodi/__pycache__/_etag_responder.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     3722 2022-04-08 21:34:36.000000 dodi-2.0.1/src/dodi/__pycache__/_transform.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     1689 2022-08-26 21:26:43.000000 dodi-2.0.1/src/dodi/__pycache__/_utils.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      271 2022-04-11 21:52:50.000000 dodi-2.0.1/src/dodi/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     4658 2022-04-13 19:26:03.000000 dodi-2.0.1/src/dodi/__pycache__/transform.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     2289 2022-04-12 16:42:31.000000 dodi-2.0.1/src/dodi/__pycache__/validator.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      321 2022-08-26 21:26:43.000000 dodi-2.0.1/src/dodi/__pycache__/urls.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     5093 2022-08-26 21:26:17.000000 dodi-2.0.1/src/dodi/README.md
--rw-r--r--   0 alex       (502) staff       (20)     3302 2022-08-26 21:27:40.000000 dodi-2.0.1/src/dodi/_views.py
--rw-r--r--   0 alex       (502) staff       (20)        5 2023-03-29 14:45:19.000000 dodi-2.0.1/src/dodi/VERSION
--rw-r--r--   0 alex       (502) staff       (20)     4914 2022-04-13 19:26:01.000000 dodi-2.0.1/src/dodi/transform.py
--rw-r--r--   0 alex       (502) staff       (20)      420 2023-03-29 14:46:21.000000 dodi-2.0.1/src/dodi/RELEASE_NOTES.md
--rw-r--r--   0 alex       (502) staff       (20)      148 2022-08-26 21:25:00.000000 dodi-2.0.1/src/dodi/urls.py
--rw-r--r--   0 alex       (502) staff       (20)     6252 2022-04-13 17:53:39.000000 dodi-2.0.1/src/dodi/_operations.py
--rw-r--r--   0 alex       (502) staff       (20)     1247 2022-08-26 21:25:34.000000 dodi-2.0.1/src/dodi/_utils.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi.egg-info/
--rw-r--r--   0 alex       (502) staff       (20)     6488 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)      907 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (502) staff       (20)       63 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi.egg-info/requires.txt
--rw-r--r--   0 alex       (502) staff       (20)        5 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi.egg-info/top_level.txt
--rw-r--r--   0 alex       (502) staff       (20)        1 2023-03-29 14:50:18.000000 dodi-2.0.1/src/dodi.egg-info/dependency_links.txt
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-18 16:34:35.000000 dodi-2.0.2/
+-rw-r--r--   0 alex       (502) staff       (20)     6488 2023-05-18 16:34:35.000000 dodi-2.0.2/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)       50 2022-04-08 13:51:07.000000 dodi-2.0.2/MANIFEST.in
+-rw-r--r--   0 alex       (502) staff       (20)     5093 2022-08-26 21:26:17.000000 dodi-2.0.2/README.md
+-rw-r--r--   0 alex       (502) staff       (20)      807 2023-05-18 16:28:52.000000 dodi-2.0.2/setup.py
+-rw-r--r--   0 alex       (502) staff       (20)        5 2023-05-18 16:33:52.000000 dodi-2.0.2/VERSION
+-rw-r--r--   0 alex       (502) staff       (20)      459 2023-05-18 16:34:24.000000 dodi-2.0.2/RELEASE_NOTES.md
+-rw-r--r--   0 alex       (502) staff       (20)       38 2023-05-18 16:34:35.000000 dodi-2.0.2/setup.cfg
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-18 16:34:35.000000 dodi-2.0.2/src/
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi/
+-rw-r--r--   0 alex       (502) staff       (20)     1876 2022-04-12 16:28:48.000000 dodi-2.0.2/src/dodi/validator.py
+-rw-r--r--   0 alex       (502) staff       (20)     2065 2022-04-13 19:35:23.000000 dodi-2.0.2/src/dodi/_etag_responder.py
+-rw-r--r--   0 alex       (502) staff       (20)       96 2022-04-11 21:52:49.000000 dodi-2.0.2/src/dodi/__init__.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi/__pycache__/
+-rw-r--r--   0 alex       (502) staff       (20)      327 2022-04-08 21:19:37.000000 dodi-2.0.2/src/dodi/__pycache__/_exceptions.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     2944 2022-08-26 21:27:42.000000 dodi-2.0.2/src/dodi/__pycache__/_views.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     3595 2022-04-13 17:53:40.000000 dodi-2.0.2/src/dodi/__pycache__/_operations.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     2295 2022-04-13 19:35:25.000000 dodi-2.0.2/src/dodi/__pycache__/_etag_responder.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     3722 2022-04-08 21:34:36.000000 dodi-2.0.2/src/dodi/__pycache__/_transform.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     1689 2022-08-26 21:26:43.000000 dodi-2.0.2/src/dodi/__pycache__/_utils.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      271 2022-04-11 21:52:50.000000 dodi-2.0.2/src/dodi/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     4658 2022-04-13 19:26:03.000000 dodi-2.0.2/src/dodi/__pycache__/transform.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     2289 2022-04-12 16:42:31.000000 dodi-2.0.2/src/dodi/__pycache__/validator.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      321 2022-08-26 21:26:43.000000 dodi-2.0.2/src/dodi/__pycache__/urls.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     5093 2022-08-26 21:26:17.000000 dodi-2.0.2/src/dodi/README.md
+-rw-r--r--   0 alex       (502) staff       (20)     3302 2022-08-26 21:27:40.000000 dodi-2.0.2/src/dodi/_views.py
+-rw-r--r--   0 alex       (502) staff       (20)        5 2023-05-18 16:33:52.000000 dodi-2.0.2/src/dodi/VERSION
+-rw-r--r--   0 alex       (502) staff       (20)     4914 2022-04-13 19:26:01.000000 dodi-2.0.2/src/dodi/transform.py
+-rw-r--r--   0 alex       (502) staff       (20)      459 2023-05-18 16:34:24.000000 dodi-2.0.2/src/dodi/RELEASE_NOTES.md
+-rw-r--r--   0 alex       (502) staff       (20)      148 2022-08-26 21:25:00.000000 dodi-2.0.2/src/dodi/urls.py
+-rw-r--r--   0 alex       (502) staff       (20)     6252 2022-04-13 17:53:39.000000 dodi-2.0.2/src/dodi/_operations.py
+-rw-r--r--   0 alex       (502) staff       (20)     1247 2022-08-26 21:25:34.000000 dodi-2.0.2/src/dodi/_utils.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi.egg-info/
+-rw-r--r--   0 alex       (502) staff       (20)     6488 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)      907 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (502) staff       (20)       65 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi.egg-info/requires.txt
+-rw-r--r--   0 alex       (502) staff       (20)        5 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi.egg-info/top_level.txt
+-rw-r--r--   0 alex       (502) staff       (20)        1 2023-05-18 16:34:35.000000 dodi-2.0.2/src/dodi.egg-info/dependency_links.txt
```

### Comparing `dodi-2.0.1/PKG-INFO` & `dodi-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodi
-Version: 2.0.1
+Version: 2.0.2
 Summary: Django On-Demand Images
 Home-page: UNKNOWN
 Author: Alex Fischer
 Author-email: alex@quadrant.net
 License: UNKNOWN
 Description: # DODI: Django On-Demand Images
```

### Comparing `dodi-2.0.1/README.md` & `dodi-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/setup.py` & `dodi-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=["Django>=2.2<4", "Pillow>=7.0.0,!=7.2.*,!=8.0.*,!=8.1.*,!=8.2.*,<9"],
+    install_requires=["Django>=2.2,<4", "Pillow>=7.0.0,!=7.2.*,!=8.0.*,!=8.1.*,!=8.2.*,<10"],
 )
```

### Comparing `dodi-2.0.1/src/dodi/validator.py` & `dodi-2.0.2/src/dodi/validator.py`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/_etag_responder.py` & `dodi-2.0.2/src/dodi/_etag_responder.py`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/_views.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/_views.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/_operations.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/_operations.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/_etag_responder.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/_etag_responder.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/_transform.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/_transform.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/_utils.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/_utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/transform.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/transform.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/__pycache__/validator.cpython-36.pyc` & `dodi-2.0.2/src/dodi/__pycache__/validator.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/README.md` & `dodi-2.0.2/src/dodi/README.md`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/_views.py` & `dodi-2.0.2/src/dodi/_views.py`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/transform.py` & `dodi-2.0.2/src/dodi/transform.py`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/_operations.py` & `dodi-2.0.2/src/dodi/_operations.py`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi/_utils.py` & `dodi-2.0.2/src/dodi/_utils.py`

 * *Files identical despite different names*

### Comparing `dodi-2.0.1/src/dodi.egg-info/PKG-INFO` & `dodi-2.0.2/src/dodi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dodi
-Version: 2.0.1
+Version: 2.0.2
 Summary: Django On-Demand Images
 Home-page: UNKNOWN
 Author: Alex Fischer
 Author-email: alex@quadrant.net
 License: UNKNOWN
 Description: # DODI: Django On-Demand Images
```

### Comparing `dodi-2.0.1/src/dodi.egg-info/SOURCES.txt` & `dodi-2.0.2/src/dodi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

