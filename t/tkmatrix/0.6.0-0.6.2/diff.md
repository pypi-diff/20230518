# Comparing `tmp/tkmatrix-0.6.0.tar.gz` & `tmp/tkmatrix-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.6.0.tar", last modified: Wed Mar  8 16:25:57 2023, max compression
+gzip compressed data, was "tkmatrix-0.6.2.tar", last modified: Thu May 18 17:17:21 2023, max compression
```

## Comparing `tkmatrix-0.6.0.tar` & `tkmatrix-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:25:57.856563 tkmatrix-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-08 16:25:57.856563 tkmatrix-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 16:25:57.856563 tkmatrix-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:25:57.852563 tkmatrix-0.6.0/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:25:57.852563 tkmatrix-0.6.0/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:25:57.856563 tkmatrix-0.6.0/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-03-08 16:25:49.000000 tkmatrix-0.6.0/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:25:57.852563 tkmatrix-0.6.0/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-08 16:25:57.000000 tkmatrix-0.6.0/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-08 16:25:57.000000 tkmatrix-0.6.0/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:25:57.000000 tkmatrix-0.6.0/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-08 16:25:57.000000 tkmatrix-0.6.0/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-08 16:25:57.000000 tkmatrix-0.6.0/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.887184 tkmatrix-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:17:21.887184 tkmatrix-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.6.0/LICENSE` & `tkmatrix-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/PKG-INFO` & `tkmatrix-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.0
+Version: 0.6.2
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.6.0/README.md` & `tkmatrix-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/setup.py` & `tkmatrix-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.6.0"
+version = "0.6.2"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
@@ -21,16 +21,16 @@
     ],
     python_requires='>=3.8',
     install_requires=['argparse==1.4.0',
                         'beautifulsoup4==4.9.3',
                         'configparser==5.0.1',
                         "corner==2.1.0",
                         "cython==0.29.21",
-                        "ellc==1.8.7",
-                        "lcbuilder==0.10.8",
+                        "ellc==1.8.5",
+                        "lcbuilder==0.12.2",
                         "matplotlib==3.5.2",
                         "mock==4.0.3",
                         'numba>=0.53.0rc1',
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "seaborn==0.11.1",
                         'setuptools>=41.0.0',
                         "scipy==1.8.0",
```

### Comparing `tkmatrix-0.6.0/tkmatrix/__main__.py` & `tkmatrix-0.6.2/tkmatrix/__main__.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix/inject_model.py` & `tkmatrix-0.6.2/tkmatrix/inject_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix/inject_rv_model.py` & `tkmatrix-0.6.2/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix/properties.yaml` & `tkmatrix-0.6.2/tkmatrix/properties.yaml`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix/rv.py` & `tkmatrix-0.6.2/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.6.2/tkmatrix/tests/test_tkmatrix.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.6.2/tkmatrix/tkmatrix_class.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.0/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.6.2/tkmatrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.0
+Version: 0.6.2
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

