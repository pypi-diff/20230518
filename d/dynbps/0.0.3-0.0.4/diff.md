# Comparing `tmp/dynbps-0.0.3.tar.gz` & `tmp/dynbps-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.3.tar", last modified: Tue May 16 23:07:54 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.4.tar", last modified: Wed May 17 12:34:58 2023, max compression
```

## Comparing `dynbps-0.0.3.tar` & `dynbps-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 23:07:54.732763 dynbps-0.0.3/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.3/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.3/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 23:07:54.732203 dynbps-0.0.3/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      275 2023-05-16 22:34:41.000000 dynbps-0.0.3/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 23:07:54.720860 dynbps-0.0.3/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     9023 2023-05-16 23:06:13.000000 dynbps-0.0.3/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-16 23:06:13.000000 dynbps-0.0.3/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-16 23:06:13.000000 dynbps-0.0.3/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 23:07:54.731301 dynbps-0.0.3/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.3/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-16 23:05:52.000000 dynbps-0.0.3/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-16 23:07:54.732927 dynbps-0.0.3/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.3/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 12:34:58.282989 dynbps-0.0.4/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.4/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.4/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 12:34:58.281868 dynbps-0.0.4/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      284 2023-05-17 12:25:45.000000 dynbps-0.0.4/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 12:34:58.269639 dynbps-0.0.4/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     9023 2023-05-17 12:25:54.000000 dynbps-0.0.4/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-17 12:25:54.000000 dynbps-0.0.4/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-17 12:25:54.000000 dynbps-0.0.4/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 12:34:58.279010 dynbps-0.0.4/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.4/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-17 12:25:30.000000 dynbps-0.0.4/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-17 12:34:58.283156 dynbps-0.0.4/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.4/setup.py
```

### Comparing `dynbps-0.0.3/LICENSE` & `dynbps-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.3/PKG-INFO` & `dynbps-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,12 +31,14 @@
 
 ``` sh
 pip install dynbps
 ```
 
 ## How to use
 
-Fill me in please! Don’t forget code examples:
+This is a test to make sure everything still works
 
 ``` python
 1+1
 ```
+
+    2
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dynbps-0.0.3/dynbps/BPS.py` & `dynbps-0.0.4/dynbps/BPS.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.3/dynbps/_modidx.py` & `dynbps-0.0.4/dynbps/_modidx.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.3/dynbps.egg-info/PKG-INFO` & `dynbps-0.0.4/dynbps.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,12 +31,14 @@
 
 ``` sh
 pip install dynbps
 ```
 
 ## How to use
 
-Fill me in please! Don’t forget code examples:
+This is a test to make sure everything still works
 
 ``` python
 1+1
 ```
+
+    2
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dynbps-0.0.3/settings.ini` & `dynbps-0.0.4/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dynbps
 lib_name = dynbps
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dynbps
 nbs_path = nbs
 recursive = True
```

### Comparing `dynbps-0.0.3/setup.py` & `dynbps-0.0.4/setup.py`

 * *Files identical despite different names*

