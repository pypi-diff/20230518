# Comparing `tmp/mimodulito-0.2.tar.gz` & `tmp/mimodulito-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimodulito-0.2.tar", last modified: Thu May 18 18:22:04 2023, max compression
+gzip compressed data, was "mimodulito-0.3.tar", last modified: Thu May 18 18:26:30 2023, max compression
```

## Comparing `mimodulito-0.2.tar` & `mimodulito-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 18:22:04.736888 mimodulito-0.2/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1134 2023-05-16 14:58:24.000000 mimodulito-0.2/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1824 2023-05-18 18:22:04.736888 mimodulito-0.2/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1370 2023-05-18 18:20:45.000000 mimodulito-0.2/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 18:22:04.736888 mimodulito-0.2/mimodulito/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       29 2023-05-18 17:56:54.000000 mimodulito-0.2/mimodulito/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 18:22:04.736888 mimodulito-0.2/mimodulito.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1824 2023-05-18 18:22:04.000000 mimodulito-0.2/mimodulito.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      272 2023-05-18 18:22:04.000000 mimodulito-0.2/mimodulito.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-05-18 18:22:04.000000 mimodulito-0.2/mimodulito.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2023-05-18 18:22:04.000000 mimodulito-0.2/mimodulito.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-05-18 18:22:04.000000 mimodulito-0.2/mimodulito.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-05-18 18:22:04.000000 mimodulito-0.2/mimodulito.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      117 2023-05-18 17:58:56.000000 mimodulito-0.2/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-05-18 18:22:04.736888 mimodulito-0.2/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2175 2023-05-18 18:21:45.000000 mimodulito-0.2/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 18:26:30.067295 mimodulito-0.3/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1134 2023-05-16 14:58:24.000000 mimodulito-0.3/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1817 2023-05-18 18:26:30.063295 mimodulito-0.3/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1363 2023-05-18 18:25:55.000000 mimodulito-0.3/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 18:26:30.063295 mimodulito-0.3/mimodulito/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       29 2023-05-18 17:56:54.000000 mimodulito-0.3/mimodulito/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 18:26:30.063295 mimodulito-0.3/mimodulito.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1817 2023-05-18 18:26:30.000000 mimodulito-0.3/mimodulito.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      272 2023-05-18 18:26:30.000000 mimodulito-0.3/mimodulito.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-05-18 18:26:30.000000 mimodulito-0.3/mimodulito.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2023-05-18 18:26:30.000000 mimodulito-0.3/mimodulito.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-05-18 18:26:30.000000 mimodulito-0.3/mimodulito.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-05-18 18:26:30.000000 mimodulito-0.3/mimodulito.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      117 2023-05-18 17:58:56.000000 mimodulito-0.3/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-05-18 18:26:30.067295 mimodulito-0.3/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2175 2023-05-18 18:26:12.000000 mimodulito-0.3/setup.py
```

### Comparing `mimodulito-0.2/LICENSE` & `mimodulito-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mimodulito-0.2/PKG-INFO` & `mimodulito-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimodulito
-Version: 0.2
+Version: 0.3
 Summary: Calculate modulus
 Home-page: https://pypi.org/project/mimodulito
 Author: Daniel Niño Villegas
 Author-email: daniel.ninov@udea.edu.co
 License: MIT
 Keywords: Modulo
 Platform: UNKNOWN
@@ -35,30 +35,28 @@
 ```
 pip install mimodulito
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ pymiau
+pip install -i https://test.pypi.org/simple/ mimodulito
 ```
 
 ## Quick start
 
 To import the package, run the next command:
 
 ```
-import midoulito
+import mimodulito
 ```
 
 ## Code examples
 
-Provide some detailed examples for more advanced users.
-
-For instance:
+Lets calculate the operation 3%2 usind the `mod` function:
 
 ```
 import mimodulito
 print(mimodulito.mod(3,2))
 ```
 
 ## What's new
```

### Comparing `mimodulito-0.2/README.md` & `mimodulito-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,28 @@
 ```
 pip install mimodulito
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ pymiau
+pip install -i https://test.pypi.org/simple/ mimodulito
 ```
 
 ## Quick start
 
 To import the package, run the next command:
 
 ```
-import midoulito
+import mimodulito
 ```
 
 ## Code examples
 
-Provide some detailed examples for more advanced users.
-
-For instance:
+Lets calculate the operation 3%2 usind the `mod` function:
 
 ```
 import mimodulito
 print(mimodulito.mod(3,2))
 ```
 
 ## What's new
```

### Comparing `mimodulito-0.2/mimodulito.egg-info/PKG-INFO` & `mimodulito-0.3/mimodulito.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimodulito
-Version: 0.2
+Version: 0.3
 Summary: Calculate modulus
 Home-page: https://pypi.org/project/mimodulito
 Author: Daniel Niño Villegas
 Author-email: daniel.ninov@udea.edu.co
 License: MIT
 Keywords: Modulo
 Platform: UNKNOWN
@@ -35,30 +35,28 @@
 ```
 pip install mimodulito
 ```
 
 You can also test the unstable version of the package with:
 
 ```
-pip install -i https://test.pypi.org/simple/ pymiau
+pip install -i https://test.pypi.org/simple/ mimodulito
 ```
 
 ## Quick start
 
 To import the package, run the next command:
 
 ```
-import midoulito
+import mimodulito
 ```
 
 ## Code examples
 
-Provide some detailed examples for more advanced users.
-
-For instance:
+Lets calculate the operation 3%2 usind the `mod` function:
 
 ```
 import mimodulito
 print(mimodulito.mod(3,2))
 ```
 
 ## What's new
```

### Comparing `mimodulito-0.2/setup.py` & `mimodulito-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.2',
+    version='0.3',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

