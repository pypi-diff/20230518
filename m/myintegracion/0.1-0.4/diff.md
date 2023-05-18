# Comparing `tmp/myintegracion-0.1.tar.gz` & `tmp/myintegracion-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myintegracion-0.1.tar", last modified: Thu May 18 18:21:58 2023, max compression
+gzip compressed data, was "myintegracion-0.4.tar", last modified: Thu May 18 18:09:46 2023, max compression
```

## Comparing `myintegracion-0.1.tar` & `myintegracion-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:21:58.767887 myintegracion-0.1/
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 myintegracion-0.1/LICENSE
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2196 2023-05-18 18:21:58.767887 myintegracion-0.1/PKG-INFO
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1675 2023-05-16 14:58:20.000000 myintegracion-0.1/README.md
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:21:58.763887 myintegracion-0.1/myintegracion/
--rw-r--r--   0 usuario   (1001) usuario   (1001)      249 2023-05-18 18:20:49.000000 myintegracion-0.1/myintegracion/__init__.py
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:21:58.767887 myintegracion-0.1/myintegracion.egg-info/
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2196 2023-05-18 18:21:58.000000 myintegracion-0.1/myintegracion.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1001) usuario   (1001)      293 2023-05-18 18:21:58.000000 myintegracion-0.1/myintegracion.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-18 18:21:58.000000 myintegracion-0.1/myintegracion.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-18 18:21:58.000000 myintegracion-0.1/myintegracion.egg-info/entry_points.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-18 18:21:58.000000 myintegracion-0.1/myintegracion.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       14 2023-05-18 18:21:58.000000 myintegracion-0.1/myintegracion.egg-info/top_level.txt
--rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 myintegracion-0.1/pyproject.toml
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-18 18:21:58.767887 myintegracion-0.1/setup.cfg
--rw-r--r--   0 usuario   (1001) usuario   (1001)     2260 2023-05-18 18:21:29.000000 myintegracion-0.1/setup.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:09:46.823890 myintegracion-0.4/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 myintegracion-0.4/LICENSE
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     2196 2023-05-18 18:09:46.823890 myintegracion-0.4/PKG-INFO
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     1675 2023-05-16 14:58:20.000000 myintegracion-0.4/README.md
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:09:46.823890 myintegracion-0.4/myintegracion/
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      500 2023-05-16 14:58:43.000000 myintegracion-0.4/myintegracion/__init__.py
+drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:09:46.823890 myintegracion-0.4/myintegracion.egg-info/
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)     2196 2023-05-18 18:09:46.000000 myintegracion-0.4/myintegracion.egg-info/PKG-INFO
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)      293 2023-05-18 18:09:46.000000 myintegracion-0.4/myintegracion.egg-info/SOURCES.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-18 18:09:46.000000 myintegracion-0.4/myintegracion.egg-info/dependency_links.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-18 18:09:46.000000 myintegracion-0.4/myintegracion.egg-info/entry_points.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-18 18:09:46.000000 myintegracion-0.4/myintegracion.egg-info/requires.txt
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       14 2023-05-18 18:09:46.000000 myintegracion-0.4/myintegracion.egg-info/top_level.txt
+-rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 myintegracion-0.4/pyproject.toml
+-rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-18 18:09:46.823890 myintegracion-0.4/setup.cfg
+-rw-r--r--   0 usuario   (1001) usuario   (1001)     2260 2023-05-18 18:01:14.000000 myintegracion-0.4/setup.py
```

### Comparing `myintegracion-0.1/LICENSE` & `myintegracion-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myintegracion-0.1/PKG-INFO` & `myintegracion-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myintegracion
-Version: 0.1
+Version: 0.4
 Summary: integracion numerica de ecuaciones diferenciales
 Home-page: https://pypi.org/project/myintegracion
 Author: emanuel
 Author-email: emanuelnorenag@gmail.com
 License: MIT
 Keywords: integegracion ecuaciones diferenciales relatividad
 Platform: UNKNOWN
```

### Comparing `myintegracion-0.1/README.md` & `myintegracion-0.4/README.md`

 * *Files identical despite different names*

### Comparing `myintegracion-0.1/myintegracion.egg-info/PKG-INFO` & `myintegracion-0.4/myintegracion.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myintegracion
-Version: 0.1
+Version: 0.4
 Summary: integracion numerica de ecuaciones diferenciales
 Home-page: https://pypi.org/project/myintegracion
 Author: emanuel
 Author-email: emanuelnorenag@gmail.com
 License: MIT
 Keywords: integegracion ecuaciones diferenciales relatividad
 Platform: UNKNOWN
```

### Comparing `myintegracion-0.1/setup.py` & `myintegracion-0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.1',
+    version='0.4',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

