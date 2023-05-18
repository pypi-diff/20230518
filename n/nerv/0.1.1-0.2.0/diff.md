# Comparing `tmp/nerv-0.1.1.tar.gz` & `tmp/nerv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerv-0.1.1.tar", last modified: Thu Apr 20 00:24:42 2023, max compression
+gzip compressed data, was "nerv-0.2.0.tar", last modified: Thu May 18 04:10:11 2023, max compression
```

## Comparing `nerv-0.1.1.tar` & `nerv-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-04-20 00:24:42.803744 nerv-0.1.1/
--rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.1.1/LICENSE
--rw-rw-r--   0 arman     (1000) arman     (1000)     2765 2023-04-20 00:24:42.799744 nerv-0.1.1/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)     2086 2023-04-19 23:34:19.000000 nerv-0.1.1/README.md
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-04-20 00:24:42.795744 nerv-0.1.1/nerv/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.1.1/nerv/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     3842 2023-04-19 23:34:19.000000 nerv-0.1.1/nerv/app.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-04-20 00:24:42.799744 nerv-0.1.1/nerv/assets/
--rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-04-19 23:34:19.000000 nerv-0.1.1/nerv/assets/styles.css
--rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-04-19 23:34:19.000000 nerv-0.1.1/nerv/callbacks.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     4406 2023-04-19 23:34:19.000000 nerv-0.1.1/nerv/layouts.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     8568 2023-04-19 23:34:19.000000 nerv-0.1.1/nerv/utility.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-04-20 00:24:42.799744 nerv-0.1.1/nerv.egg-info/
--rw-rw-r--   0 arman     (1000) arman     (1000)     2765 2023-04-20 00:24:42.000000 nerv-0.1.1/nerv.egg-info/PKG-INFO
--rw-rw-r--   0 arman     (1000) arman     (1000)      331 2023-04-20 00:24:42.000000 nerv-0.1.1/nerv.egg-info/SOURCES.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-04-20 00:24:42.000000 nerv-0.1.1/nerv.egg-info/dependency_links.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)      562 2023-04-20 00:24:42.000000 nerv-0.1.1/nerv.egg-info/requires.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-04-20 00:24:42.000000 nerv-0.1.1/nerv.egg-info/top_level.txt
--rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-04-20 00:24:42.803744 nerv-0.1.1/setup.cfg
--rw-rw-r--   0 arman     (1000) arman     (1000)     1363 2023-04-20 00:23:20.000000 nerv-0.1.1/setup.py
-drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-04-20 00:24:42.799744 nerv-0.1.1/tests/
--rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-04-19 23:34:19.000000 nerv-0.1.1/tests/__init__.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-04-19 23:34:19.000000 nerv-0.1.1/tests/conftest.py
--rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-04-19 23:35:30.000000 nerv-0.1.1/tests/test_app_callbacks.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.848473 nerv-0.2.0/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1072 2022-07-07 21:55:46.000000 nerv-0.2.0/LICENSE
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 04:10:11.848473 nerv-0.2.0/PKG-INFO
+-rw-------   0 arman     (1000) arman     (1000)     3011 2023-05-18 04:06:51.000000 nerv-0.2.0/README.md
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/nerv/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2022-07-07 21:55:46.000000 nerv-0.2.0/nerv/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6598 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/app.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/nerv/assets/
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10462 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/assets/favicon.ico
+-rw-rw-r--   0 arman     (1000) arman     (1000)      171 2023-05-14 18:46:58.000000 nerv-0.2.0/nerv/assets/styles.css
+-rw-rw-r--   0 arman     (1000) arman     (1000)    10204 2023-05-15 05:24:51.000000 nerv-0.2.0/nerv/callbacks.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     7782 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/layouts.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     8836 2023-05-18 03:59:25.000000 nerv-0.2.0/nerv/utility.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/nerv.egg-info/
+-rw-rw-r--   0 arman     (1000) arman     (1000)     4225 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/PKG-INFO
+-rw-rw-r--   0 arman     (1000) arman     (1000)      355 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/SOURCES.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)        1 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/dependency_links.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       59 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/requires.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       11 2023-05-18 04:10:11.000000 nerv-0.2.0/nerv.egg-info/top_level.txt
+-rw-rw-r--   0 arman     (1000) arman     (1000)       38 2023-05-18 04:10:11.848473 nerv-0.2.0/setup.cfg
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1360 2023-05-18 03:59:25.000000 nerv-0.2.0/setup.py
+drwxrwxr-x   0 arman     (1000) arman     (1000)        0 2023-05-18 04:10:11.844473 nerv-0.2.0/tests/
+-rw-rw-r--   0 arman     (1000) arman     (1000)        0 2023-05-10 00:08:49.000000 nerv-0.2.0/tests/__init__.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     6280 2023-05-10 00:08:49.000000 nerv-0.2.0/tests/conftest.py
+-rw-rw-r--   0 arman     (1000) arman     (1000)     1704 2023-05-10 00:08:49.000000 nerv-0.2.0/tests/test_app_callbacks.py
```

### Comparing `nerv-0.1.1/LICENSE` & `nerv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nerv-0.1.1/PKG-INFO` & `nerv-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: nerv
-Version: 0.1.1
-Summary: Neuroimaging Results Visualization
-Home-page: https://github.com/rmanaem/nerv
-Author: rmanaem
-Author-email: <rmanaem@protonmail.ch>
-License: MIT
-Keywords: python,dash,pandas,data visualization,plotly,neuroscience
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 <div align="center">
 
 # Neuroimaging Results Visualization
 
 <div>
     <a href="https://github.com/rmanaem/nerv/actions/workflows/test.yaml">
         <img src="https://img.shields.io/github/actions/workflow/status/neurobagel/api/test.yaml?color=BDB76B&label=test&style=flat-square">
@@ -33,46 +12,62 @@
     <a href="LICENSE">
         <img src="https://img.shields.io/github/license/neurobagel/api?color=CD5C5C&style=flat-square" alt="GitHub license">
     </a>
 </div>
 <br>
 </div>
 
-Neuroimaging Results Visualization (NeRV) is a web interface developed in Python using [Plotly Dash](https://dash.plotly.com/),  [Dash Bootstrap Components](https://dash-bootstrap-components.opensource.faculty.ai/), and [pandas](https://pandas.pydata.org/) for visualization of neuroimaging results obtained from continuous testing of neuroimaging data across software pipelines.
+Neuroimaging Results Visualization (NeRV) is a web interface developed in Python using [Plotly Dash](https://dash.plotly.com/), [Dash Bootstrap Components](https://dash-bootstrap-components.opensource.faculty.ai/), and [pandas](https://pandas.pydata.org/) for visualization of neuroimaging results obtained from continuous testing of neuroimaging data across software pipelines.
+
+- [Getting Started](#getting-started)
+  - [Installation](#installation)
+  - [Example usage](#example-usage)
+- [Deployment](#deployment)
+- [License](#license)
 
 ______________________________________________________________________
 
 ## Getting Started
 
 ### Installation
 
+Install NeRV using pip:
+
 ```bash
 pip install nerv
 ```
 
-In order for NeRV to generate and populate plots the underlying app requires access to the directory containing the datasets. The path to directory can be passed to the app module as input to the start function.
-
 ### Example usage
 
+In order for NeRV to generate and populate plots the underlying app requires access to the directory that houses subdirectories, which in turn contain the JSON files to be visualized. The path to directory can be passed to the app as input to the `start` function.
+
 ```python
 from nerv import app
 
 app.start("path-to-data-directory")
 ```
 
 After executing the file containing the above code snippet, a local server is started at port 8050 (by default). You can access the running NeRV application using a browser through the URL `localhost:8050`.
 
-<p alt="ui" align="center"><a href="https://github.com/rmanaem/nerv/blob/master/img/ui.png"><img src="https://github.com/rmanaem/nerv/blob/master/img/ui.png?raw=true"/></a></p>
+![ui](https://github.com/rmanaem/nerv/blob/master/img/ui.png?raw=true)
 
 ______________________________________________________________________
 
 ## Deployment
 
-_Work in progress_
+To deploy your NeRV app, you can utilize [Gunicorn](https://gunicorn.org/). Simply follow the instructions outlined in the Dash documentation [here](https://dash.plotly.comdeployment#heroku-for-sharing-public-dash-apps), making the necessary adjustment in the app.py module content:
+
+**app.py**
+
+```Python
+from nerv import app
+
+server = app.start("path-to-data-directory", False)
+```
+
+Note that when the `local` parameter of the `start` function is set to `False`, it will return the `app.server` object. This object represents the underlying Flask server that drives the Dash application. You can utilize the `app.server` object to customize and extend the NeRV application, going beyond the default functionality offered. For more details, refer to the [Flask documentation](https://flask.palletsprojects.com/).
 
 ______________________________________________________________________
 
 ## License
 
 This project is licensed under the terms of [MIT License](LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: nerv Version: 0.1.1 Summary: Neuroimaging Results
-Visualization Home-page: https://github.com/rmanaem/nerv Author: rmanaem
-Author-email:
-protonmail.ch> License: MIT Keywords: python,dash,pandas,data
-visualization,plotly,neuroscience Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown License-File: LICENSE
                      # Neuroimaging Results Visualization
     [https://img.shields.io/github/actions/workflow/status/neurobagel/api/
 test.yaml?color=BDB76B&label=test&style=flat-square] [Python] [GitHub_license]
 
 Neuroimaging Results Visualization (NeRV) is a web interface developed in
 Python using [Plotly Dash](https://dash.plotly.com/), [Dash Bootstrap
 Components](https://dash-bootstrap-components.opensource.faculty.ai/), and
 [pandas](https://pandas.pydata.org/) for visualization of neuroimaging results
 obtained from continuous testing of neuroimaging data across software
-pipelines.
+pipelines. - [Getting Started](#getting-started) - [Installation]
+(#installation) - [Example usage](#example-usage) - [Deployment](#deployment) -
+[License](#license)
 ______________________________________________________________________ ##
-Getting Started ### Installation ```bash pip install nerv ``` In order for NeRV
-to generate and populate plots the underlying app requires access to the
-directory containing the datasets. The path to directory can be passed to the
-app module as input to the start function. ### Example usage ```python from
-nerv import app app.start("path-to-data-directory") ``` After executing the
-file containing the above code snippet, a local server is started at port 8050
-(by default). You can access the running NeRV application using a browser
-through the URL `localhost:8050`.
-       [https://github.com/rmanaem/nerv/blob/master/img/ui.png?raw=true]
+Getting Started ### Installation Install NeRV using pip: ```bash pip install
+nerv ``` ### Example usage In order for NeRV to generate and populate plots the
+underlying app requires access to the directory that houses subdirectories,
+which in turn contain the JSON files to be visualized. The path to directory
+can be passed to the app as input to the `start` function. ```python from nerv
+import app app.start("path-to-data-directory") ``` After executing the file
+containing the above code snippet, a local server is started at port 8050 (by
+default). You can access the running NeRV application using a browser through
+the URL `localhost:8050`. ![ui](https://github.com/rmanaem/nerv/blob/master/
+img/ui.png?raw=true)
 ______________________________________________________________________ ##
-Deployment _Work in progress_
+Deployment To deploy your NeRV app, you can utilize [Gunicorn](https://
+gunicorn.org/). Simply follow the instructions outlined in the Dash
+documentation [here](https://dash.plotly.comdeployment#heroku-for-sharing-
+public-dash-apps), making the necessary adjustment in the app.py module
+content: **app.py** ```Python from nerv import app server = app.start("path-to-
+data-directory", False) ``` Note that when the `local` parameter of the `start`
+function is set to `False`, it will return the `app.server` object. This object
+represents the underlying Flask server that drives the Dash application. You
+can utilize the `app.server` object to customize and extend the NeRV
+application, going beyond the default functionality offered. For more details,
+refer to the [Flask documentation](https://flask.palletsprojects.com/).
 ______________________________________________________________________ ##
 License This project is licensed under the terms of [MIT License](LICENSE).
```

### Comparing `nerv-0.1.1/nerv/callbacks.py` & `nerv-0.2.0/nerv/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerv-0.1.1/nerv/utility.py` & `nerv-0.2.0/nerv/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,52 @@
 
 import dash_bootstrap_components as dbc
 import pandas as pd
 import plotly.express as px
 from dash import html
 
 COLORS = [
-    px.colors.qualitative.G10,
     px.colors.sequential.Teal,
-    px.colors.sequential.Brwnyl,
-    px.colors.sequential.Burg,
+    px.colors.sequential.OrRd,
     px.colors.sequential.Purp,
+    px.colors.sequential.Greens,
+    px.colors.sequential.Pinkyl,
+    px.colors.sequential.Brwnyl,
+    px.colors.sequential.solar,
+    px.colors.sequential.turbid,
 ]
 
+DBC_THEMES = {
+    "BOOTSTRAP": dbc.themes.BOOTSTRAP,
+    "CERULEAN": dbc.themes.CERULEAN,
+    "COSMO": dbc.themes.COSMO,
+    "CYBORG": dbc.themes.CYBORG,
+    "DARKLY": dbc.themes.DARKLY,
+    "FLATLY": dbc.themes.FLATLY,
+    "JOURNAL": dbc.themes.JOURNAL,
+    "LITERA": dbc.themes.LITERA,
+    "LUMEN": dbc.themes.LUMEN,
+    "LUX": dbc.themes.LUX,
+    "MATERIA": dbc.themes.MATERIA,
+    "MINTY": dbc.themes.MINTY,
+    "MORPH": dbc.themes.MORPH,
+    "PULSE": dbc.themes.PULSE,
+    "SANDSTONE": dbc.themes.SANDSTONE,
+    "SIMPLEX": dbc.themes.SIMPLEX,
+    "SKETCHY": dbc.themes.SKETCHY,
+    "SLATE": dbc.themes.SLATE,
+    "SOLAR": dbc.themes.SOLAR,
+    "SPACELAB": dbc.themes.SPACELAB,
+    "SUPERHERO": dbc.themes.SUPERHERO,
+    "UNITED": dbc.themes.UNITED,
+    "VAPOR": dbc.themes.VAPOR,
+    "YETI": dbc.themes.YETI,
+    "ZEPHYR": dbc.themes.ZEPHYR,
+}
+
 
 def pull_files(path):
     """
     Creates a list of paths for .json files in the input path.
 
     Parameters
     ----------
@@ -109,37 +140,14 @@
     files = pull_files(path)
     dfs = []
     for i, j in enumerate(files):
         dfs.append(process_file(j, i))
     return pd.concat(dfs)
 
 
-def pull_directories(path):
-    """
-    Generates a list of tuples for each directory located in the input path.
-    Tuples are in (directory name, dataframe generated from the files
-    in directory) form. Dataframes are generated using pull_files function.
-
-    Parameters
-    ----------
-    path : str
-        Path of the directory containing direcotries that all contain .json files
-        to be visualized.
-
-    Returns
-    ----------
-    list
-        A list of tuples in (directory name, directory dataframe) form.
-    """
-    files = []
-    for directory in os.listdir(path):
-        files.append((directory, process_files(os.path.join(path, directory))))
-    return files
-
-
 def generate_summary(df):
     """
     Generates a summary for the input dataframe's data.
     The summary includes total number of datapoints, total number
     of missing datapoints, and number of missing datapoints in
     each dataset-pipeline.
```

### Comparing `nerv-0.1.1/setup.py` & `nerv-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-import codecs
-import os
-
 from setuptools import find_packages, setup
 
-here = os.path.abspath(os.path.dirname(__file__))
+with open("CHANGELOG.md", "r") as file:
+    changelog = file.readlines()[9:20]
+
+with open("README.md", "r") as file:
+    readme = file.read()
 
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
-    long_description = "\n" + file.read()
 
 with open("requirements.txt", "r") as file:
     install_requires = file.read().split("\n")
 
-VERSION = "0.1.1"
+VERSION = "0.2.0"
 DESCRIPTION = "Neuroimaging Results Visualization"
-LONG_DESCRIPTION = long_description
+LONG_DESCRIPTION = f"## What's new in {VERSION}\n\n{''.join(changelog)}\n\n{readme}"
 
 setup(
     name="nerv",
     version=VERSION,
     author="rmanaem",
     author_email="<rmanaem@protonmail.ch>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    long_description=long_description,
+    long_description=LONG_DESCRIPTION,
     url="https://github.com/rmanaem/nerv",
     packages=find_packages(),
     include_package_data=True,
     package_data={"nerv": ["assets/*"]},
     install_requires=install_requires,
     license="MIT",
     keywords=[
```

### Comparing `nerv-0.1.1/tests/conftest.py` & `nerv-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nerv-0.1.1/tests/test_app_callbacks.py` & `nerv-0.2.0/tests/test_app_callbacks.py`

 * *Files identical despite different names*

