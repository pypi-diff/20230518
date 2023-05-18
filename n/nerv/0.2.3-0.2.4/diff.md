# Comparing `tmp/nerv-0.2.3.tar.gz` & `tmp/nerv-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerv-0.2.3.tar", last modified: Thu May 18 05:10:53 2023, max compression
+gzip compressed data, was "nerv-0.2.4.tar", last modified: Thu May 18 05:24:05 2023, max compression
```

## Comparing `nerv-0.2.3.tar` & `nerv-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:10:53.240956 nerv-0.2.3/
--rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.3/LICENSE
--rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 05:10:53.240956 nerv-0.2.3/PKG-INFO
--rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.3/README.md
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:10:53.236956 nerv-0.2.3/nerv/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.3/nerv/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.3/nerv/app.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:10:53.240956 nerv-0.2.3/nerv/assets/
--rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.3/nerv/assets/favicon.ico
--rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.3/nerv/assets/styles.css
--rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.3/nerv/callbacks.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.3/nerv/layouts.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.3/nerv/utility.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:10:53.236956 nerv-0.2.3/nerv.egg-info/
--rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 05:10:53.000000 nerv-0.2.3/nerv.egg-info/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)      355 2023-05-18 05:10:53.000000 nerv-0.2.3/nerv.egg-info/SOURCES.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 05:10:53.000000 nerv-0.2.3/nerv.egg-info/dependency_links.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 05:10:53.000000 nerv-0.2.3/nerv.egg-info/requires.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 05:10:53.000000 nerv-0.2.3/nerv.egg-info/top_level.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 05:10:53.240956 nerv-0.2.3/setup.cfg
--rw-rw-r--   0 arman     (1000) arman     (1000)     1376 2023-05-18 05:08:02.000000 nerv-0.2.3/setup.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:10:53.240956 nerv-0.2.3/tests/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.3/tests/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.3/tests/conftest.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.3/tests/test_app_callbacks.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:24:05.391333 nerv-0.2.4/
+-rw-------   0 arman     (1000) arman     (1000)      790 2023-05-18 05:20:26.000000 nerv-0.2.4/CHANGELOG.md
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.4/LICENSE
+-rw-rw-r--   0 arman     (1000) arman     (1000)       37 2023-05-18 05:18:35.000000 nerv-0.2.4/MANIFEST.in
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 05:24:05.391333 nerv-0.2.4/PKG-INFO
+-rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.4/README.md
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:24:05.387333 nerv-0.2.4/nerv/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.4/nerv/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.4/nerv/app.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:24:05.387333 nerv-0.2.4/nerv/assets/
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.4/nerv/assets/favicon.ico
+-rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.4/nerv/assets/styles.css
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.4/nerv/callbacks.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.4/nerv/layouts.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.4/nerv/utility.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:24:05.387333 nerv-0.2.4/nerv.egg-info/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 05:24:05.000000 nerv-0.2.4/nerv.egg-info/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)      380 2023-05-18 05:24:05.000000 nerv-0.2.4/nerv.egg-info/SOURCES.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 05:24:05.000000 nerv-0.2.4/nerv.egg-info/dependency_links.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 05:24:05.000000 nerv-0.2.4/nerv.egg-info/requires.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 05:24:05.000000 nerv-0.2.4/nerv.egg-info/top_level.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 05:24:05.391333 nerv-0.2.4/setup.cfg
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1319 2023-05-18 05:21:06.000000 nerv-0.2.4/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 05:24:05.391333 nerv-0.2.4/tests/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.4/tests/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.4/tests/conftest.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.4/tests/test_app_callbacks.py
```

### Comparing `nerv-0.2.3/LICENSE` & `nerv-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/PKG-INFO` & `nerv-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerv
-Version: 0.2.3
+Version: 0.2.4
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
 
-## What's new in 0.2.3
+## What's new in 0.2.4
 
 ### Added
 
 - Functionality for visualizing multiple experiments
 - Home page, consists of the experiment directories found in the input path
 - Navbar, includes a link to the home page, settings, GitHub, and Docs
 - Settings, includes a theme changer that enables users to modify the application theme to their liking
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.2.3 Summary: Neuroimaging Results
+Metadata-Version: 2.1 Name: nerv Version: 0.2.4 Summary: Neuroimaging Results
 Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
 Author-email:
 protonmail.ch> License: MIT Keywords: python,dash,pandas,data
 visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown License-File: LICENSE ## What's new in
-0.2.3 ### Added - Functionality for visualizing multiple experiments - Home
+0.2.4 ### Added - Functionality for visualizing multiple experiments - Home
 page, consists of the experiment directories found in the input path - Navbar,
 includes a link to the home page, settings, GitHub, and Docs - Settings,
 includes a theme changer that enables users to modify the application theme to
 their liking ### Changed - The `start` function now expects a directory path as
 input, where each subdirectory represents an experiment and contains the
 corresponding JSON files for visualization - favicon
                      # Neuroimaging Results Visualization
```

### Comparing `nerv-0.2.3/README.md` & `nerv-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/nerv/app.py` & `nerv-0.2.4/nerv/app.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/nerv/assets/favicon.ico` & `nerv-0.2.4/nerv/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/nerv/callbacks.py` & `nerv-0.2.4/nerv/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/nerv/layouts.py` & `nerv-0.2.4/nerv/layouts.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/nerv/utility.py` & `nerv-0.2.4/nerv/utility.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/nerv.egg-info/PKG-INFO` & `nerv-0.2.4/nerv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerv
-Version: 0.2.3
+Version: 0.2.4
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
 
-## What's new in 0.2.3
+## What's new in 0.2.4
 
 ### Added
 
 - Functionality for visualizing multiple experiments
 - Home page, consists of the experiment directories found in the input path
 - Navbar, includes a link to the home page, settings, GitHub, and Docs
 - Settings, includes a theme changer that enables users to modify the application theme to their liking
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.2.3 Summary: Neuroimaging Results
+Metadata-Version: 2.1 Name: nerv Version: 0.2.4 Summary: Neuroimaging Results
 Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
 Author-email:
 protonmail.ch> License: MIT Keywords: python,dash,pandas,data
 visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown License-File: LICENSE ## What's new in
-0.2.3 ### Added - Functionality for visualizing multiple experiments - Home
+0.2.4 ### Added - Functionality for visualizing multiple experiments - Home
 page, consists of the experiment directories found in the input path - Navbar,
 includes a link to the home page, settings, GitHub, and Docs - Settings,
 includes a theme changer that enables users to modify the application theme to
 their liking ### Changed - The `start` function now expects a directory path as
 input, where each subdirectory represents an experiment and contains the
 corresponding JSON files for visualization - favicon
                      # Neuroimaging Results Visualization
```

### Comparing `nerv-0.2.3/setup.py` & `nerv-0.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,29 @@
 with open("README.md", "r") as file:
     readme = file.read()
 
 
 with open("requirements.txt", "r") as file:
     install_requires = file.read().split("\n")
 
-VERSION = "0.2.3"
+VERSION = "0.2.4"
 DESCRIPTION = "Neuroimaging Results Visualization"
 LONG_DESCRIPTION = f"## What's new in {VERSION}\n\n{''.join(changelog)}\n\n{readme}"
 
 setup(
     name="nerv",
     version=VERSION,
     author="rmanaem",
     author_email="<rmanaem@protonmail.ch>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     url="https://github.com/rmanaem/nerv",
     packages=find_packages(),
     include_package_data=True,
-    package_data={"nerv": ["assets/*", "CHANGELOG.md"]},
     install_requires=install_requires,
     license="MIT",
     keywords=[
         "python",
         "dash",
         "pandas",
         "data visualization",
```

### Comparing `nerv-0.2.3/tests/conftest.py` & `nerv-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nerv-0.2.3/tests/test_app_callbacks.py` & `nerv-0.2.4/tests/test_app_callbacks.py`

 * *Files identical despite different names*

