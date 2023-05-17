# Comparing `tmp/dctrackclient-0.4.3.tar.gz` & `tmp/dctrackclient-0.4.4.tar.gz`

## Comparing `dctrackclient-0.4.3.tar` & `dctrackclient-0.4.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.4.3/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.4.3/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 dctrackclient-0.4.3/../README.md
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 dctrackclient-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.4.4/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.4.4/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 dctrackclient-0.4.4/../README.md
+-rw-r--r--   0        0        0     9751 2020-02-02 00:00:00.000000 dctrackclient-0.4.4/PKG-INFO
```

### Comparing `dctrackclient-0.4.3/src/dcTrackClient/__init__.py` & `dctrackclient-0.4.4/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.4.3/pyproject.toml` & `dctrackclient-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.4.3/../README.md` & `dctrackclient-0.4.4/../README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 **WARNING: this project is still under development and may not be stable!**
 
 # dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/publish.yml?logo=github) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient?logo=pypi) ![npm](https://img.shields.io/npm/v/dctrackclient) ![npm](https://img.shields.io/npm/dt/dctrackclient?logo=npm)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
-## Initialize a connection to the dcTrack API
+## Installation
 
-Import the class:
+> dcTrackClient can be installed from the package manager of your choice.
+
+### Python
 
-```py
-from dcTrackClient import Client
 ```
+pip install dcTrackClient
+```
+
+### JavaScript
 
-Authenticate using a base URL (the same URL to access the GUI) and a username and password:
+```
+npm i dctrackclient
+```
+
+## Initialize a connection to the dcTrack API
+
+> Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
+
+### Python
 
 ```py
+from dcTrackClient import Client
+## Using a username and password ##
 api = Client('https://dctrack.example.com/', username='user', password='pass')
+## Using an API token ##
+api = Client('https://dctrack.example.com/', apiToken='token')
 ```
 
-Authenticate using a base URL and an API token:
+### JavaScript
 
-```py
-api = Client('https://dctrack.example.com/', apiToken='asdf')
+```js
+import * as api from 'dctrackclient';
+// Using a username and password // 
+api.Client.authenticate('https://dctrack.example.com/', { username: 'user', password: 'pass' });
+// Using an API token //
+api.Client.authenticate('https://dctrack.example.com/', { apiToken: 'token' });
 ```
 
 ## Usage Example
 
+> This section is currently under construction.
+
 ### Create an item:
 
 - This example shows the minimum attributes required to create an item
 - See [the official documentation](#official-dctrack-documentation) for a comprehensive list of attributes
 - This function returns the JSON object for the newly created item
 - If it fails, the function will return a JSON object containing the error message
```

### Comparing `dctrackclient-0.4.3/PKG-INFO` & `dctrackclient-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.4.3
+Version: 0.4.4
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -16,36 +16,58 @@
 
 **WARNING: this project is still under development and may not be stable!**
 
 # dcTrackClient ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/nicfv/dcTrackClient/publish.yml?logo=github) ![PyPI](https://img.shields.io/pypi/v/dcTrackClient) ![PyPI - Downloads](https://img.shields.io/pypi/dm/dcTrackClient?logo=pypi) ![npm](https://img.shields.io/npm/v/dctrackclient) ![npm](https://img.shields.io/npm/dt/dctrackclient?logo=npm)
 
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
-## Initialize a connection to the dcTrack API
+## Installation
 
-Import the class:
+> dcTrackClient can be installed from the package manager of your choice.
+
+### Python
 
-```py
-from dcTrackClient import Client
 ```
+pip install dcTrackClient
+```
+
+### JavaScript
 
-Authenticate using a base URL (the same URL to access the GUI) and a username and password:
+```
+npm i dctrackclient
+```
+
+## Initialize a connection to the dcTrack API
+
+> Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
+
+### Python
 
 ```py
+from dcTrackClient import Client
+## Using a username and password ##
 api = Client('https://dctrack.example.com/', username='user', password='pass')
+## Using an API token ##
+api = Client('https://dctrack.example.com/', apiToken='token')
 ```
 
-Authenticate using a base URL and an API token:
+### JavaScript
 
-```py
-api = Client('https://dctrack.example.com/', apiToken='asdf')
+```js
+import * as api from 'dctrackclient';
+// Using a username and password // 
+api.Client.authenticate('https://dctrack.example.com/', { username: 'user', password: 'pass' });
+// Using an API token //
+api.Client.authenticate('https://dctrack.example.com/', { apiToken: 'token' });
 ```
 
 ## Usage Example
 
+> This section is currently under construction.
+
 ### Create an item:
 
 - This example shows the minimum attributes required to create an item
 - See [the official documentation](#official-dctrack-documentation) for a comprehensive list of attributes
 - This function returns the JSON object for the newly created item
 - If it fails, the function will return a JSON object containing the error message
```

