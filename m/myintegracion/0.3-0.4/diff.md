# Comparing `tmp/myintegracion-0.3.tar.gz` & `tmp/myintegracion-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myintegracion-0.3.tar", last modified: Thu May 18 18:47:00 2023, max compression
+gzip compressed data, was "myintegracion-0.4.tar", last modified: Thu May 18 18:09:46 2023, max compression
```

## Comparing `myintegracion-0.3.tar` & `myintegracion-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:47:00.711881 myintegracion-0.3/
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1134 2023-05-16 14:58:24.000000 myintegracion-0.3/LICENSE
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2339 2023-05-18 18:47:00.711881 myintegracion-0.3/PKG-INFO
--rw-r--r--   0 usuario   (1001) usuario   (1001)     1818 2023-05-18 18:46:13.000000 myintegracion-0.3/README.md
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:47:00.711881 myintegracion-0.3/myintegracion/
--rw-r--r--   0 usuario   (1001) usuario   (1001)      249 2023-05-18 18:20:49.000000 myintegracion-0.3/myintegracion/__init__.py
-drwxrwxr-x   0 usuario   (1001) usuario   (1001)        0 2023-05-18 18:47:00.711881 myintegracion-0.3/myintegracion.egg-info/
--rw-rw-r--   0 usuario   (1001) usuario   (1001)     2339 2023-05-18 18:47:00.000000 myintegracion-0.3/myintegracion.egg-info/PKG-INFO
--rw-rw-r--   0 usuario   (1001) usuario   (1001)      293 2023-05-18 18:47:00.000000 myintegracion-0.3/myintegracion.egg-info/SOURCES.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)        1 2023-05-18 18:47:00.000000 myintegracion-0.3/myintegracion.egg-info/dependency_links.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       50 2023-05-18 18:47:00.000000 myintegracion-0.3/myintegracion.egg-info/entry_points.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       30 2023-05-18 18:47:00.000000 myintegracion-0.3/myintegracion.egg-info/requires.txt
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       14 2023-05-18 18:47:00.000000 myintegracion-0.3/myintegracion.egg-info/top_level.txt
--rw-r--r--   0 usuario   (1001) usuario   (1001)      131 2023-05-16 14:58:32.000000 myintegracion-0.3/pyproject.toml
--rw-rw-r--   0 usuario   (1001) usuario   (1001)       38 2023-05-18 18:47:00.711881 myintegracion-0.3/setup.cfg
--rw-r--r--   0 usuario   (1001) usuario   (1001)     2260 2023-05-18 18:46:33.000000 myintegracion-0.3/setup.py
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

### Comparing `myintegracion-0.3/LICENSE` & `myintegracion-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myintegracion-0.3/PKG-INFO` & `myintegracion-0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myintegracion
-Version: 0.3
+Version: 0.4
 Summary: integracion numerica de ecuaciones diferenciales
 Home-page: https://pypi.org/project/myintegracion
 Author: emanuel
 Author-email: emanuelnorenag@gmail.com
 License: MIT
 Keywords: integegracion ecuaciones diferenciales relatividad
 Platform: UNKNOWN
@@ -24,68 +24,66 @@
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
 <p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
-<p align="center"><img src="https://saberimagenes.com/wp-content/uploads/2018/12/Universo15.jpg" alt="Logo""/></p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
-pip install myintegracion
+pip install pymiau
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ myintegracion
+pip install -i https://test.pypi.org/simple/ pymiau
 ```
 
 ## Quick start
 
 In this section you should provide the most simple instructions to use
 your package.
 
 For instance:
 
 ```
-import myintegracion as int
-print(myintegracion.integracion())
+import pymiau
+print(pymiau.miau())
 ```
 
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import myintegracion
-print(myintegracion.integracion(f,a,b))
+import pymiau
+print(pymiau.miau(n=2))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
-Version 0.1:
-
-- Function `integracion was` implemented.
+Version 0.2:
 
+- Function `guau` was implemented.
+- New parameters added to the `miau` routine.
 
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
 
-
```

### Comparing `myintegracion-0.3/myintegracion.egg-info/PKG-INFO` & `myintegracion-0.4/myintegracion.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myintegracion
-Version: 0.3
+Version: 0.4
 Summary: integracion numerica de ecuaciones diferenciales
 Home-page: https://pypi.org/project/myintegracion
 Author: emanuel
 Author-email: emanuelnorenag@gmail.com
 License: MIT
 Keywords: integegracion ecuaciones diferenciales relatividad
 Platform: UNKNOWN
@@ -24,68 +24,66 @@
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
 <p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
-<p align="center"><img src="https://saberimagenes.com/wp-content/uploads/2018/12/Universo15.jpg" alt="Logo""/></p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
-pip install myintegracion
+pip install pymiau
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ myintegracion
+pip install -i https://test.pypi.org/simple/ pymiau
 ```
 
 ## Quick start
 
 In this section you should provide the most simple instructions to use
 your package.
 
 For instance:
 
 ```
-import myintegracion as int
-print(myintegracion.integracion())
+import pymiau
+print(pymiau.miau())
 ```
 
 ## Code examples
 
 Provide some detailed examples for more advanced users.
 
 For instance:
 
 ```
-import myintegracion
-print(myintegracion.integracion(f,a,b))
+import pymiau
+print(pymiau.miau(n=2))
 ```
 
 ## What's new
 
 If your package will be frequently updated with new features include a
 section describing the new features added to it:
 
-Version 0.1:
-
-- Function `integracion was` implemented.
+Version 0.2:
 
+- Function `guau` was implemented.
+- New parameters added to the `miau` routine.
 
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
 
-
```

### Comparing `myintegracion-0.3/setup.py` & `myintegracion-0.4/setup.py`

 * *Files 2% similar despite different names*

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

