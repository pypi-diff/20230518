# Comparing `tmp/nerv-0.2.0.tar.gz` & `tmp/nerv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerv-0.2.0.tar", last modified: Thu May 18 04:10:11 2023, max compression
+gzip compressed data, was "nerv-0.2.1.tar", last modified: Thu May 18 04:43:31 2023, max compression
```

## Comparing `nerv-0.2.0.tar` & `nerv-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.848473 nerv-0.2.0/
--rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.0/LICENSE
--rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 04:10:11.848473 nerv-0.2.0/PKG-INFO
--rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.0/README.md
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/nerv/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.0/nerv/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/app.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/nerv/assets/
--rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/assets/favicon.ico
--rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.0/nerv/assets/styles.css
--rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.0/nerv/callbacks.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/layouts.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/utility.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/nerv.egg-info/
--rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)      355 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/SOURCES.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/dependency_links.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/requires.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/top_level.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 04:10:11.848473 nerv-0.2.0/setup.cfg
--rw-rw-r--   0 arman     (1000) arman     (1000)     1360 2023-05-18 03:59:25.000000 nerv-0.2.0/setup.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/tests/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.0/tests/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.0/tests/conftest.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.0/tests/test_app_callbacks.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.938956 nerv-0.2.1/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.1/LICENSE
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3760 2023-05-18 04:43:31.938956 nerv-0.2.1/PKG-INFO
+-rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.1/README.md
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.934956 nerv-0.2.1/nerv/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.1/nerv/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/app.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.938956 nerv-0.2.1/nerv/assets/
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/assets/favicon.ico
+-rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.1/nerv/assets/styles.css
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.1/nerv/callbacks.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/layouts.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.1/nerv/utility.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.934956 nerv-0.2.1/nerv.egg-info/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     3760 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)      355 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/SOURCES.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/dependency_links.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/requires.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 04:43:31.000000 nerv-0.2.1/nerv.egg-info/top_level.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 04:43:31.938956 nerv-0.2.1/setup.cfg
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1460 2023-05-18 04:42:14.000000 nerv-0.2.1/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:43:31.938956 nerv-0.2.1/tests/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.1/tests/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.1/tests/conftest.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.1/tests/test_app_callbacks.py
```

### Comparing `nerv-0.2.0/LICENSE` & `nerv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/PKG-INFO` & `nerv-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Neuroimaging Results Visualization
 Home-page: https://github.com/rmanaem/nerv
 Author: rmanaem
 Author-email: <rmanaem@protonmail.ch>
 License: MIT
 Keywords: python,dash,pandas,data visualization,plotly,neuroscience
 Platform: UNKNOWN
@@ -14,27 +14,19 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## What's new in 0.2.0
+## What's new in 0.2.1
 
-### Added
+### Fixed
 
-- Functionality for visualizing multiple experiments
-- Home page, consists of the experiment directories found in the input path
-- Navbar, includes a link to the home page, settings, GitHub, and Docs
-- Settings, includes a theme changer that enables users to modify the application theme to their liking
-
-### Changed
-
-- The `start` function now expects a directory path as input, where each subdirectory represents an experiment and contains the corresponding JSON files for visualization
-- favicon
+- Pip subprocess issue with paths
 
 
 <div align="center">
 
 # Neuroimaging Results Visualization
 
 <div>
```

#### html2text {}

```diff
@@ -1,24 +1,18 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.2.0 Summary: Neuroimaging Results
+Metadata-Version: 2.1 Name: nerv Version: 0.2.1 Summary: Neuroimaging Results
 Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
 Author-email:
 protonmail.ch> License: MIT Keywords: python,dash,pandas,data
 visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown License-File: LICENSE ## What's new in
-0.2.0 ### Added - Functionality for visualizing multiple experiments - Home
-page, consists of the experiment directories found in the input path - Navbar,
-includes a link to the home page, settings, GitHub, and Docs - Settings,
-includes a theme changer that enables users to modify the application theme to
-their liking ### Changed - The `start` function now expects a directory path as
-input, where each subdirectory represents an experiment and contains the
-corresponding JSON files for visualization - favicon
+0.2.1 ### Fixed - Pip subprocess issue with paths
                      # Neuroimaging Results Visualization
     [https://img.shields.io/github/actions/workflow/status/neurobagel/api/
 test.yaml?color=BDB76B&label=test&style=flat-square] [Python] [GitHub_license]
 
 Neuroimaging Results Visualization (NeRV) is a web interface developed in
 Python using [Plotly Dash](https://dash.plotly.com/), [Dash Bootstrap
 Components](https://dash-bootstrap-components.opensource.faculty.ai/), and
```

### Comparing `nerv-0.2.0/README.md` & `nerv-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/nerv/app.py` & `nerv-0.2.1/nerv/app.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/nerv/assets/favicon.ico` & `nerv-0.2.1/nerv/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/nerv/callbacks.py` & `nerv-0.2.1/nerv/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/nerv/layouts.py` & `nerv-0.2.1/nerv/layouts.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/nerv/utility.py` & `nerv-0.2.1/nerv/utility.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/nerv.egg-info/PKG-INFO` & `nerv-0.2.1/nerv.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Neuroimaging Results Visualization
 Home-page: https://github.com/rmanaem/nerv
 Author: rmanaem
 Author-email: <rmanaem@protonmail.ch>
 License: MIT
 Keywords: python,dash,pandas,data visualization,plotly,neuroscience
 Platform: UNKNOWN
@@ -14,27 +14,19 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## What's new in 0.2.0
+## What's new in 0.2.1
 
-### Added
+### Fixed
 
-- Functionality for visualizing multiple experiments
-- Home page, consists of the experiment directories found in the input path
-- Navbar, includes a link to the home page, settings, GitHub, and Docs
-- Settings, includes a theme changer that enables users to modify the application theme to their liking
-
-### Changed
-
-- The `start` function now expects a directory path as input, where each subdirectory represents an experiment and contains the corresponding JSON files for visualization
-- favicon
+- Pip subprocess issue with paths
 
 
 <div align="center">
 
 # Neuroimaging Results Visualization
 
 <div>
```

#### html2text {}

```diff
@@ -1,24 +1,18 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.2.0 Summary: Neuroimaging Results
+Metadata-Version: 2.1 Name: nerv Version: 0.2.1 Summary: Neuroimaging Results
 Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
 Author-email:
 protonmail.ch> License: MIT Keywords: python,dash,pandas,data
 visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown License-File: LICENSE ## What's new in
-0.2.0 ### Added - Functionality for visualizing multiple experiments - Home
-page, consists of the experiment directories found in the input path - Navbar,
-includes a link to the home page, settings, GitHub, and Docs - Settings,
-includes a theme changer that enables users to modify the application theme to
-their liking ### Changed - The `start` function now expects a directory path as
-input, where each subdirectory represents an experiment and contains the
-corresponding JSON files for visualization - favicon
+0.2.1 ### Fixed - Pip subprocess issue with paths
                      # Neuroimaging Results Visualization
     [https://img.shields.io/github/actions/workflow/status/neurobagel/api/
 test.yaml?color=BDB76B&label=test&style=flat-square] [Python] [GitHub_license]
 
 Neuroimaging Results Visualization (NeRV) is a web interface developed in
 Python using [Plotly Dash](https://dash.plotly.com/), [Dash Bootstrap
 Components](https://dash-bootstrap-components.opensource.faculty.ai/), and
```

### Comparing `nerv-0.2.0/setup.py` & `nerv-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import os
+
 from setuptools import find_packages, setup
 
-with open("CHANGELOG.md", "r") as file:
-    changelog = file.readlines()[9:20]
+dir = os.path.abspath(os.path.dirname(__file__))
+
+with open(os.path.join(dir, "CHANGELOG.md"), "r") as file:
+    changelog = file.readlines()[9:12]
+
 
-with open("README.md", "r") as file:
+with open(os.path.join(dir, "README.md"), "r") as file:
     readme = file.read()
 
 
 with open("requirements.txt", "r") as file:
     install_requires = file.read().split("\n")
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 DESCRIPTION = "Neuroimaging Results Visualization"
 LONG_DESCRIPTION = f"## What's new in {VERSION}\n\n{''.join(changelog)}\n\n{readme}"
 
 setup(
     name="nerv",
     version=VERSION,
     author="rmanaem",
```

### Comparing `nerv-0.2.0/tests/conftest.py` & `nerv-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.0/tests/test_app_callbacks.py` & `nerv-0.2.1/tests/test_app_callbacks.py`

 * *Files identical despite different names*

