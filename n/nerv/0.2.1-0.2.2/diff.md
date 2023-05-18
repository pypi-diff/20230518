# Comparing `tmp/nerv-0.2.1.tar.gz` & `tmp/nerv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerv-0.2.1.tar", last modified: Thu May 18 04:43:31 2023, max compression
+gzip compressed data, was "nerv-0.2.2.tar", last modified: Thu May 18 04:53:10 2023, max compression
```

## Comparing `nerv-0.2.1.tar` & `nerv-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.938956 nerv-0.2.1/
--rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.1/LICENSE
--rw-rw-r--   0 arman     (1000) arman     (1000)     3760 2023-05-18 04:43:31.938956 nerv-0.2.1/PKG-INFO
--rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.1/README.md
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.934956 nerv-0.2.1/nerv/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.1/nerv/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/app.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.938956 nerv-0.2.1/nerv/assets/
--rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/assets/favicon.ico
--rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.1/nerv/assets/styles.css
--rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.1/nerv/callbacks.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/layouts.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/utility.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.934956 nerv-0.2.1/nerv.egg-info/
--rw-rw-r--   0 arman     (1000) arman     (1000)     3760 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)      355 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/SOURCES.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/dependency_links.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/requires.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/top_level.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 04:43:31.938956 nerv-0.2.1/setup.cfg
--rw-rw-r--   0 arman     (1000) arman     (1000)     1460 2023-05-18 04:42:14.000000 nerv-0.2.1/setup.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.938956 nerv-0.2.1/tests/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.1/tests/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.1/tests/conftest.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.1/tests/test_app_callbacks.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:53:10.102920 nerv-0.2.2/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.2/LICENSE
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3760 2023-05-18 04:53:10.102920 nerv-0.2.2/PKG-INFO
+-rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.2/README.md
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:53:10.098920 nerv-0.2.2/nerv/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.2/nerv/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.2/nerv/app.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:53:10.098920 nerv-0.2.2/nerv/assets/
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.2/nerv/assets/favicon.ico
+-rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.2/nerv/assets/styles.css
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.2/nerv/callbacks.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.2/nerv/layouts.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.2/nerv/utility.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:53:10.098920 nerv-0.2.2/nerv.egg-info/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3760 2023-05-18 04:53:10.000000 nerv-0.2.2/nerv.egg-info/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)      355 2023-05-18 04:53:10.000000 nerv-0.2.2/nerv.egg-info/SOURCES.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 04:53:10.000000 nerv-0.2.2/nerv.egg-info/dependency_links.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 04:53:10.000000 nerv-0.2.2/nerv.egg-info/requires.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 04:53:10.000000 nerv-0.2.2/nerv.egg-info/top_level.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 04:53:10.102920 nerv-0.2.2/setup.cfg
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1514 2023-05-18 04:52:38.000000 nerv-0.2.2/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:53:10.102920 nerv-0.2.2/tests/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.2/tests/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.2/tests/conftest.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.2/tests/test_app_callbacks.py
```

### Comparing `nerv-0.2.1/LICENSE` & `nerv-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/PKG-INFO` & `nerv-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerv
-Version: 0.2.1
+Version: 0.2.2
 Summary: Neuroimaging Results Visualization
 Home-page: https://github.com/rmanaem/nerv
 Author: rmanaem
 Author-email: <rmanaem@protonmail.ch>
 License: MIT
 Keywords: python,dash,pandas,data visualization,plotly,neuroscience
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## What's new in 0.2.1
+## What's new in 0.2.2
 
 ### Fixed
 
 - Pip subprocess issue with paths
 
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.2.1 Summary: Neuroimaging Results
+Metadata-Version: 2.1 Name: nerv Version: 0.2.2 Summary: Neuroimaging Results
 Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
 Author-email:
 protonmail.ch> License: MIT Keywords: python,dash,pandas,data
 visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown License-File: LICENSE ## What's new in
-0.2.1 ### Fixed - Pip subprocess issue with paths
+0.2.2 ### Fixed - Pip subprocess issue with paths
                      # Neuroimaging Results Visualization
     [https://img.shields.io/github/actions/workflow/status/neurobagel/api/
 test.yaml?color=BDB76B&label=test&style=flat-square] [Python] [GitHub_license]
 
 Neuroimaging Results Visualization (NeRV) is a web interface developed in
 Python using [Plotly Dash](https://dash.plotly.com/), [Dash Bootstrap
 Components](https://dash-bootstrap-components.opensource.faculty.ai/), and
```

### Comparing `nerv-0.2.1/README.md` & `nerv-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/nerv/app.py` & `nerv-0.2.2/nerv/app.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/nerv/assets/favicon.ico` & `nerv-0.2.2/nerv/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/nerv/callbacks.py` & `nerv-0.2.2/nerv/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/nerv/layouts.py` & `nerv-0.2.2/nerv/layouts.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/nerv/utility.py` & `nerv-0.2.2/nerv/utility.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/nerv.egg-info/PKG-INFO` & `nerv-0.2.2/nerv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerv
-Version: 0.2.1
+Version: 0.2.2
 Summary: Neuroimaging Results Visualization
 Home-page: https://github.com/rmanaem/nerv
 Author: rmanaem
 Author-email: <rmanaem@protonmail.ch>
 License: MIT
 Keywords: python,dash,pandas,data visualization,plotly,neuroscience
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## What's new in 0.2.1
+## What's new in 0.2.2
 
 ### Fixed
 
 - Pip subprocess issue with paths
 
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.2.1 Summary: Neuroimaging Results
+Metadata-Version: 2.1 Name: nerv Version: 0.2.2 Summary: Neuroimaging Results
 Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
 Author-email:
 protonmail.ch> License: MIT Keywords: python,dash,pandas,data
 visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown License-File: LICENSE ## What's new in
-0.2.1 ### Fixed - Pip subprocess issue with paths
+0.2.2 ### Fixed - Pip subprocess issue with paths
                      # Neuroimaging Results Visualization
     [https://img.shields.io/github/actions/workflow/status/neurobagel/api/
 test.yaml?color=BDB76B&label=test&style=flat-square] [Python] [GitHub_license]
 
 Neuroimaging Results Visualization (NeRV) is a web interface developed in
 Python using [Plotly Dash](https://dash.plotly.com/), [Dash Bootstrap
 Components](https://dash-bootstrap-components.opensource.faculty.ai/), and
```

### Comparing `nerv-0.2.1/setup.py` & `nerv-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+import codecs
 import os
 
 from setuptools import find_packages, setup
 
 dir = os.path.abspath(os.path.dirname(__file__))
 
-with open(os.path.join(dir, "CHANGELOG.md"), "r") as file:
+with codecs.open(os.path.join(dir, "CHANGELOG.md"), encoding="utf-8") as file:
     changelog = file.readlines()[9:12]
 
 
-with open(os.path.join(dir, "README.md"), "r") as file:
+with codecs.open(os.path.join(dir, "README.md"), encoding="utf-8") as file:
     readme = file.read()
 
 
 with open("requirements.txt", "r") as file:
     install_requires = file.read().split("\n")
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 DESCRIPTION = "Neuroimaging Results Visualization"
 LONG_DESCRIPTION = f"## What's new in {VERSION}\n\n{''.join(changelog)}\n\n{readme}"
 
 setup(
     name="nerv",
     version=VERSION,
     author="rmanaem",
```

### Comparing `nerv-0.2.1/tests/conftest.py` & `nerv-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.1/tests/test_app_callbacks.py` & `nerv-0.2.2/tests/test_app_callbacks.py`

 * *Files identical despite different names*

