# Comparing `tmp/gdptools_pygeoapi_plugin-0.0.6.dev0.tar.gz` & `tmp/gdptools_pygeoapi_plugin-0.0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdptools_pygeoapi_plugin-0.0.6.dev0.tar", max compression
+gzip compressed data, was "gdptools_pygeoapi_plugin-0.0.7.dev0.tar", max compression
```

## Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0.tar` & `gdptools_pygeoapi_plugin-0.0.7.dev0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1640 2022-09-08 23:56:38.751663 gdptools_pygeoapi_plugin-0.0.6.dev0/LICENSE.md
--rw-r--r--   0        0        0     2556 2022-09-08 23:56:38.701663 gdptools_pygeoapi_plugin-0.0.6.dev0/README.md
--rw-r--r--   0        0        0     2911 2023-04-26 14:30:24.126025 gdptools_pygeoapi_plugin-0.0.6.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-08 15:57:52.951663 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/__init__.py
--rw-r--r--   0        0        0     9014 2023-03-16 15:57:07.478580 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py
--rw-r--r--   0        0        0     2046 2023-03-16 16:50:55.466982 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py
--rw-r--r--   0        0        0     9261 2023-03-16 15:55:31.368763 gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py
--rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 gdptools_pygeoapi_plugin-0.0.6.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1640 2022-09-08 23:56:38.751663 gdptools_pygeoapi_plugin-0.0.7.dev0/LICENSE.md
+-rw-r--r--   0        0        0     2556 2022-09-08 23:56:38.701663 gdptools_pygeoapi_plugin-0.0.7.dev0/README.md
+-rw-r--r--   0        0        0     2832 2023-05-18 15:39:42.124008 gdptools_pygeoapi_plugin-0.0.7.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-08 15:57:52.951663 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/__init__.py
+-rw-r--r--   0        0        0     9014 2023-03-16 15:57:07.478580 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py
+-rw-r--r--   0        0        0     2106 2023-05-18 15:03:49.530427 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py
+-rw-r--r--   0        0        0     9261 2023-03-16 15:55:31.368763 gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py
+-rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 gdptools_pygeoapi_plugin-0.0.7.dev0/PKG-INFO
```

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/LICENSE.md` & `gdptools_pygeoapi_plugin-0.0.7.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/README.md` & `gdptools_pygeoapi_plugin-0.0.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/pyproject.toml` & `gdptools_pygeoapi_plugin-0.0.7.dev0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gdptools-pygeoapi-plugin"
-version = "0.0.6-dev0"
+version = "0.0.7-dev0"
 description = "Gdptools Pygeoapi Plugin"
 authors = ["Richard McDonald <rmcd@usgs.gov>"]
 license = "LICENSE.md"
 readme = "README.md"
 homepage = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin"
 repository = "https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin"
 documentation = "https://gdptools-pygeoapi-plugin.readthedocs.io"
@@ -54,19 +54,15 @@
 sphinx-rtd-theme = "^0.5.2"
 sphinx-click = "^3.0.1"
 Pygments = "^2.9.0"
 poetry2conda = "^0.3.0"
 nox = "^2021.10.1"
 nox_poetry = "^0.8.6"
 types-all = "^1.0.0"
-bandit = "1.7.2"
-aiohttp = "^3.8.3"
-asyncio = "^3.4.3"
-ipykernel = "^6.16.0"
-nest-asyncio = "^1.5.6"
+urllib3 = "<=1.26.15"
 
 [tool.poetry.scripts]
 gdptools-pygeoapi-plugin = "gdptools_pygeoapi_plugin.__main__:main"
 
 [tool.poetry2conda]
 name = "gdptools-pygeoapi-plugin"
```

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py` & `gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/calc_weights_catalog.py`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py` & `gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/proc_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 LOGGER = logging.getLogger(__name__)
 
 PROCESS_METADATA = {
     "version": "0.1.0",
     "id": "test_processing",
     "title": "Timed processing function for testing",
     "description": "Simple processing function for timed duration",
+    "jobControlOptions": ["sync-execute", "async-execute"],
     "keywords": ["process-testing"],
     "links": [
         {
             "type": "text/html",
             "rel": "canonical",
             "title": "information",
             "href": "https://example.org/process",
```

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py` & `gdptools_pygeoapi_plugin-0.0.7.dev0/src/gdptools_pygeoapi_plugin/_pygeoapi_process/run_weights_catalog.py`

 * *Files identical despite different names*

### Comparing `gdptools_pygeoapi_plugin-0.0.6.dev0/PKG-INFO` & `gdptools_pygeoapi_plugin-0.0.7.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdptools-pygeoapi-plugin
-Version: 0.0.6.dev0
+Version: 0.0.7.dev0
 Summary: Gdptools Pygeoapi Plugin
 Home-page: https://code.usgs.gov/wma/nhgf/toolsteam/gdptools-pygeoapi-plugin
 License: LICENSE.md
 Author: Richard McDonald
 Author-email: rmcd@usgs.gov
 Requires-Python: >=3.9,<3.10
 Classifier: Development Status :: 1 - Planning
```

