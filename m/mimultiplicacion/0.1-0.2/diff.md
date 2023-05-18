# Comparing `tmp/mimultiplicacion-0.1.tar.gz` & `tmp/mimultiplicacion-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimultiplicacion-0.1.tar", last modified: Thu May 18 17:54:30 2023, max compression
+gzip compressed data, was "mimultiplicacion-0.2.tar", last modified: Thu May 18 18:04:17 2023, max compression
```

## Comparing `mimultiplicacion-0.1.tar` & `mimultiplicacion-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 17:54:30.820006 mimultiplicacion-0.1/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 mimultiplicacion-0.1/LICENSE
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2146 2023-05-18 17:54:30.820006 mimultiplicacion-0.1/PKG-INFO
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1675 2023-05-16 14:58:20.000000 mimultiplicacion-0.1/README.md
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 17:54:30.820006 mimultiplicacion-0.1/mimultiplicacion/
--rw-r--r--   0 juanita   (1000) juanita   (1000)      158 2023-05-16 18:56:03.000000 mimultiplicacion-0.1/mimultiplicacion/__init__.py
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 17:54:30.820006 mimultiplicacion-0.1/mimultiplicacion.egg-info/
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2146 2023-05-18 17:54:30.000000 mimultiplicacion-0.1/mimultiplicacion.egg-info/PKG-INFO
--rw-rw-r--   0 juanita   (1000) juanita   (1000)      314 2023-05-18 17:54:30.000000 mimultiplicacion-0.1/mimultiplicacion.egg-info/SOURCES.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-05-18 17:54:30.000000 mimultiplicacion-0.1/mimultiplicacion.egg-info/dependency_links.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       59 2023-05-18 17:54:30.000000 mimultiplicacion-0.1/mimultiplicacion.egg-info/entry_points.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 17:54:30.000000 mimultiplicacion-0.1/mimultiplicacion.egg-info/requires.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 17:54:30.000000 mimultiplicacion-0.1/mimultiplicacion.egg-info/top_level.txt
--rw-r--r--   0 juanita   (1000) juanita   (1000)      131 2023-05-16 14:58:32.000000 mimultiplicacion-0.1/pyproject.toml
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-05-18 17:54:30.820006 mimultiplicacion-0.1/setup.cfg
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2202 2023-05-18 17:51:59.000000 mimultiplicacion-0.1/setup.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:04:17.236659 mimultiplicacion-0.2/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 mimultiplicacion-0.2/LICENSE
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2192 2023-05-18 18:04:17.236659 mimultiplicacion-0.2/PKG-INFO
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1721 2023-05-18 18:00:52.000000 mimultiplicacion-0.2/README.md
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:04:17.236659 mimultiplicacion-0.2/mimultiplicacion/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      158 2023-05-16 18:56:03.000000 mimultiplicacion-0.2/mimultiplicacion/__init__.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-05-18 18:04:17.236659 mimultiplicacion-0.2/mimultiplicacion.egg-info/
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2192 2023-05-18 18:04:17.000000 mimultiplicacion-0.2/mimultiplicacion.egg-info/PKG-INFO
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)      314 2023-05-18 18:04:17.000000 mimultiplicacion-0.2/mimultiplicacion.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-05-18 18:04:17.000000 mimultiplicacion-0.2/mimultiplicacion.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       59 2023-05-18 18:04:17.000000 mimultiplicacion-0.2/mimultiplicacion.egg-info/entry_points.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 18:04:17.000000 mimultiplicacion-0.2/mimultiplicacion.egg-info/requires.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       17 2023-05-18 18:04:17.000000 mimultiplicacion-0.2/mimultiplicacion.egg-info/top_level.txt
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      131 2023-05-16 14:58:32.000000 mimultiplicacion-0.2/pyproject.toml
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-05-18 18:04:17.236659 mimultiplicacion-0.2/setup.cfg
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2202 2023-05-18 18:03:29.000000 mimultiplicacion-0.2/setup.py
```

### Comparing `mimultiplicacion-0.1/LICENSE` & `mimultiplicacion-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mimultiplicacion-0.1/PKG-INFO` & `mimultiplicacion-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimultiplicacion
-Version: 0.1
+Version: 0.2
 Summary: Make a multiplicacion
 Home-page: https://pypi.org/project/mimultiplicacion
 Author: Juani
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: multiplication maths
 Platform: UNKNOWN
@@ -14,24 +14,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMiau
 ## Use a short explanatory subtitle like, Make a Miau and a Guau
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
-[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
+[![version](https://img.shields.io/pypi/v/mimultiplicacion?color=blue)](https://pypi.org/project/mimultiplicacion/)
+[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/mimultiplicacion/)
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
-<p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
+<p align="center"><img src="https://img.freepik.com/premium-vector/multiplication-table-with-cats_118813-3728.jpg?w=740" alt="Logo""/></p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
@@ -83,7 +83,8 @@
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
 
+
```

### Comparing `mimultiplicacion-0.1/README.md` & `mimultiplicacion-0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # PyMiau
 ## Use a short explanatory subtitle like, Make a Miau and a Guau
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
-[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
+[![version](https://img.shields.io/pypi/v/mimultiplicacion?color=blue)](https://pypi.org/project/mimultiplicacion/)
+[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/mimultiplicacion/)
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
-<p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
+<p align="center"><img src="https://img.freepik.com/premium-vector/multiplication-table-with-cats_118813-3728.jpg?w=740" alt="Logo""/></p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
@@ -65,8 +65,8 @@
 
 Version 0.1:
 
 - First version of the package.
 
 ------------
 
-This package has been designed and written by Fulanit@ de Tal (C) 2023
+This package has been designed and written by Fulanit@ de Tal (C) 2023
```

### Comparing `mimultiplicacion-0.1/mimultiplicacion.egg-info/PKG-INFO` & `mimultiplicacion-0.2/mimultiplicacion.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimultiplicacion
-Version: 0.1
+Version: 0.2
 Summary: Make a multiplicacion
 Home-page: https://pypi.org/project/mimultiplicacion
 Author: Juani
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: multiplication maths
 Platform: UNKNOWN
@@ -14,24 +14,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyMiau
 ## Use a short explanatory subtitle like, Make a Miau and a Guau
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/pymiau/)
-[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/pymiau/)
+[![version](https://img.shields.io/pypi/v/mimultiplicacion?color=blue)](https://pypi.org/project/mimultiplicacion/)
+[![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/mimultiplicacion/)
 
 Always start the README explaining clearly what your package do.  If
 you can include here some beautiful image to call the attention of the
 potential user do it!
 
 This is an example:
 
-<p align="center"><img src="https://drive.google.com/uc?export=view&id=1XWnQLEt_oBJjVzMLFVGEAm_uh4zmiYvC" alt="Logo""/></p>
+<p align="center"><img src="https://img.freepik.com/premium-vector/multiplication-table-with-cats_118813-3728.jpg?w=740" alt="Logo""/></p>
 
 ## Download and install
 
 Describe here how the package can be downloaded and install it in
 different arquitectures.
 
 If you are using `PyPI` installation it's as simple as:
@@ -83,7 +83,8 @@
 
 - First version of the package.
 
 ------------
 
 This package has been designed and written by Fulanit@ de Tal (C) 2023
 
+
```

### Comparing `mimultiplicacion-0.1/setup.py` & `mimultiplicacion-0.2/setup.py`

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
-    version='0.1',
+    version='0.2',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

