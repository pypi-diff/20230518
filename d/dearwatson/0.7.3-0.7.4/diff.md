# Comparing `tmp/dearwatson-0.7.3.tar.gz` & `tmp/dearwatson-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.7.3.tar", last modified: Mon May 15 16:16:55 2023, max compression
+gzip compressed data, was "dearwatson-0.7.4.tar", last modified: Thu May 18 13:57:23 2023, max compression
```

## Comparing `dearwatson-0.7.3.tar` & `dearwatson-0.7.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-15 16:16:43.000000 dearwatson-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 16:16:43.000000 dearwatson-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 16:16:55.719729 dearwatson-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 16:16:43.000000 dearwatson-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.715728 dearwatson-0.7.3/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-15 16:16:55.000000 dearwatson-0.7.3/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:16:55.719729 dearwatson-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-15 16:16:43.000000 dearwatson-0.7.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 16:16:43.000000 dearwatson-0.7.3/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.715728 dearwatson-0.7.3/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.715728 dearwatson-0.7.3/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.711728 dearwatson-0.7.3/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-15 16:16:43.000000 dearwatson-0.7.3/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:44.000000 dearwatson-0.7.3/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-15 16:16:44.000000 dearwatson-0.7.3/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:16:55.719729 dearwatson-0.7.3/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:16:45.000000 dearwatson-0.7.3/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-15 16:16:45.000000 dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-15 16:16:45.000000 dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   107144 2023-05-15 16:16:44.000000 dearwatson-0.7.3/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-18 13:57:11.000000 dearwatson-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 13:57:11.000000 dearwatson-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-18 13:57:23.947231 dearwatson-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 13:57:11.000000 dearwatson-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 13:57:23.000000 dearwatson-0.7.4/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:57:23.947231 dearwatson-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-18 13:57:12.000000 dearwatson-0.7.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-18 13:57:12.000000 dearwatson-0.7.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.943231 dearwatson-0.7.4/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-18 13:57:12.000000 dearwatson-0.7.4/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:57:23.947231 dearwatson-0.7.4/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107144 2023-05-18 13:57:13.000000 dearwatson-0.7.4/watson/watson.py
```

### Comparing `dearwatson-0.7.3/LICENSE` & `dearwatson-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/PKG-INFO` & `dearwatson-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.3
+Version: 0.7.4
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.3/README.md` & `dearwatson-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.7.4/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.3
+Version: 0.7.4
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.3/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.4/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/setup.py` & `dearwatson-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.7.3"
+version = "0.7.4"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
@@ -23,15 +23,15 @@
     python_requires='>=3.8',
     install_requires=[
                         "bokeh==2.4.2", # TPFPlotter dependency
                         'configparser==5.0.1',
                         "cython==0.29.21",
                         "extension-helpers==0.1",
                         "imageio==2.9.0",
-                        "lcbuilder==0.12.1",
+                        "lcbuilder==0.12.2",
                         "matplotlib==3.5.2",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "pyyaml==5.4.1",
                         "reportlab==3.5.59",
                         'setuptools>=41.0.0',
     ]
-)
+)
```

### Comparing `dearwatson-0.7.3/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.4/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/neighbours.py` & `dearwatson-0.7.4/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/report.py` & `dearwatson-0.7.4/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/resources/images/sherlock3.png` & `dearwatson-0.7.4/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/resources/images/watson.png` & `dearwatson-0.7.4/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/tests/test_watson.py` & `dearwatson-0.7.4/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.4/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.3/watson/watson.py` & `dearwatson-0.7.4/watson/watson.py`

 * *Files identical despite different names*

