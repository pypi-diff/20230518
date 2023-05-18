# Comparing `tmp/mimultiplicacion-0.3.tar.gz` & `tmp/mimultiplicacion-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimultiplicacion-0.3.tar", last modified: Thu May 18 18:18:31 2023, max compression
+gzip compressed data, was "mimultiplicacion-0.4.tar", last modified: Thu May 18 18:22:18 2023, max compression
```

## Comparing `mimultiplicacion-0.3.tar` & `mimultiplicacion-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:18:31.033275 mimultiplicacion-0.3/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 mimultiplicacion-0.3/LICENSE
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2229 2023-05-18 18:18:31.033275 mimultiplicacion-0.3/PKG-INFO
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1758 2023-05-18 18:16:42.000000 mimultiplicacion-0.3/README.md
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:18:31.033275 mimultiplicacion-0.3/mimultiplicacion/
--rw-r--r--   0 juanita   (1000) juanita   (1000)      247 2023-05-18 18:16:22.000000 mimultiplicacion-0.3/mimultiplicacion/__init__.py
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:18:31.033275 mimultiplicacion-0.3/mimultiplicacion.egg-info/
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2229 2023-05-18 18:18:31.000000 mimultiplicacion-0.3/mimultiplicacion.egg-info/PKG-INFO
--rw-rw-r--   0 juanita   (1000) juanita   (1000)      314 2023-05-18 18:18:31.000000 mimultiplicacion-0.3/mimultiplicacion.egg-info/SOURCES.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-05-18 18:18:31.000000 mimultiplicacion-0.3/mimultiplicacion.egg-info/dependency_links.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       59 2023-05-18 18:18:31.000000 mimultiplicacion-0.3/mimultiplicacion.egg-info/entry_points.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 18:18:31.000000 mimultiplicacion-0.3/mimultiplicacion.egg-info/requires.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 18:18:31.000000 mimultiplicacion-0.3/mimultiplicacion.egg-info/top_level.txt
--rw-r--r--   0 juanita   (1000) juanita   (1000)      131 2023-05-16 14:58:32.000000 mimultiplicacion-0.3/pyproject.toml
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-05-18 18:18:31.033275 mimultiplicacion-0.3/setup.cfg
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2202 2023-05-18 18:18:26.000000 mimultiplicacion-0.3/setup.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:22:18.004629 mimultiplicacion-0.4/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 mimultiplicacion-0.4/LICENSE
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2262 2023-05-18 18:22:18.004629 mimultiplicacion-0.4/PKG-INFO
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1791 2023-05-18 18:21:48.000000 mimultiplicacion-0.4/README.md
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:22:18.004629 mimultiplicacion-0.4/mimultiplicacion/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      247 2023-05-18 18:16:22.000000 mimultiplicacion-0.4/mimultiplicacion/__init__.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:22:18.004629 mimultiplicacion-0.4/mimultiplicacion.egg-info/
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2262 2023-05-18 18:22:17.000000 mimultiplicacion-0.4/mimultiplicacion.egg-info/PKG-INFO
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)      314 2023-05-18 18:22:17.000000 mimultiplicacion-0.4/mimultiplicacion.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-05-18 18:22:17.000000 mimultiplicacion-0.4/mimultiplicacion.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       59 2023-05-18 18:22:17.000000 mimultiplicacion-0.4/mimultiplicacion.egg-info/entry_points.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 18:22:17.000000 mimultiplicacion-0.4/mimultiplicacion.egg-info/requires.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 18:22:17.000000 mimultiplicacion-0.4/mimultiplicacion.egg-info/top_level.txt
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      131 2023-05-16 14:58:32.000000 mimultiplicacion-0.4/pyproject.toml
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-05-18 18:22:18.004629 mimultiplicacion-0.4/setup.cfg
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2202 2023-05-18 18:22:10.000000 mimultiplicacion-0.4/setup.py
```

### Comparing `mimultiplicacion-0.3/LICENSE` & `mimultiplicacion-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mimultiplicacion-0.3/PKG-INFO` & `mimultiplicacion-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimultiplicacion
-Version: 0.3
+Version: 0.4
 Summary: Make a multiplicacion
 Home-page: https://pypi.org/project/mimultiplicacion
 Author: Juani
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: multiplication maths
 Platform: UNKNOWN
@@ -61,30 +61,30 @@
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau(n=2))
+import mimultiplicacion
+print(pymiau.multuplica_dos_numeros(a=3, b=4))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
 Version 0.3:
 
 - Function `saludo_inicial` was implemented.
 - Function `multiplica_dos_numeros` was implemented.
 
-Version 0.1:
+Version 0.3:
 
-- First version of the package.
+- Third version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `mimultiplicacion-0.3/README.md` & `mimultiplicacion-0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,28 +45,28 @@
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau(n=2))
+import mimultiplicacion
+print(pymiau.multuplica_dos_numeros(a=3, b=4))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
 Version 0.3:
 
 - Function `saludo_inicial` was implemented.
 - Function `multiplica_dos_numeros` was implemented.
 
-Version 0.1:
+Version 0.3:
 
-- First version of the package.
+- Third version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `mimultiplicacion-0.3/mimultiplicacion.egg-info/PKG-INFO` & `mimultiplicacion-0.4/mimultiplicacion.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimultiplicacion
-Version: 0.3
+Version: 0.4
 Summary: Make a multiplicacion
 Home-page: https://pypi.org/project/mimultiplicacion
 Author: Juani
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: multiplication maths
 Platform: UNKNOWN
@@ -61,30 +61,30 @@
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import pymiau
-print(pymiau.miau(n=2))
+import mimultiplicacion
+print(pymiau.multuplica_dos_numeros(a=3, b=4))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
 Version 0.3:
 
 - Function `saludo_inicial` was implemented.
 - Function `multiplica_dos_numeros` was implemented.
 
-Version 0.1:
+Version 0.3:
 
-- First version of the package.
+- Third version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `mimultiplicacion-0.3/setup.py` & `mimultiplicacion-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.3',
+    version='0.4',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

