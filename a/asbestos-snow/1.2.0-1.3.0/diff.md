# Comparing `tmp/asbestos_snow-1.2.0.tar.gz` & `tmp/asbestos_snow-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asbestos_snow-1.2.0.tar", max compression
+gzip compressed data, was "asbestos_snow-1.3.0.tar", max compression
```

## Comparing `asbestos_snow-1.2.0.tar` & `asbestos_snow-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2023-04-06 15:57:51.958541 asbestos_snow-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     2362 2023-04-06 15:57:51.958541 asbestos_snow-1.2.0/README.md
--rw-r--r--   0        0        0      367 2023-04-06 15:57:51.958541 asbestos_snow-1.2.0/asbestos/__init__.py
--rw-r--r--   0        0        0    18017 2023-04-06 15:57:51.958541 asbestos_snow-1.2.0/asbestos/asbestos.py
--rw-r--r--   0        0        0      360 2023-04-06 15:57:51.958541 asbestos_snow-1.2.0/asbestos/exceptions.py
--rw-r--r--   0        0        0     1618 2023-04-06 15:57:51.958541 asbestos_snow-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3440 1970-01-01 00:00:00.000000 asbestos_snow-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-18 17:04:31.282493 asbestos_snow-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2378 2023-05-18 17:04:31.282493 asbestos_snow-1.3.0/README.md
+-rw-r--r--   0        0        0      367 2023-05-18 17:04:31.282493 asbestos_snow-1.3.0/asbestos/__init__.py
+-rw-r--r--   0        0        0    18036 2023-05-18 17:04:31.282493 asbestos_snow-1.3.0/asbestos/asbestos.py
+-rw-r--r--   0        0        0      360 2023-05-18 17:04:31.282493 asbestos_snow-1.3.0/asbestos/exceptions.py
+-rw-r--r--   0        0        0     1616 2023-05-18 17:04:31.282493 asbestos_snow-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 asbestos_snow-1.3.0/PKG-INFO
```

### Comparing `asbestos_snow-1.2.0/LICENSE.md` & `asbestos_snow-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `asbestos_snow-1.2.0/README.md` & `asbestos_snow-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # asbestos
 An easy way to mock Snowflake connections in Python!
 
 ## What is this?
 
-`asbestos` is a library to allow easy mocking of Snowflake calls during local development or testing to save on costs and time. The docs have more information, but here's a quick example:
+`asbestos` is a library for Python 3.9+ to allow easy mocking of Snowflake calls during local development or testing to save on costs and time. The docs have more information, but here's a quick example:
 
 ```python
 from asbestos import asbestos_cursor, config as asbestos_config
 
 
 def snowflake_cursor() -> SnowflakeCursor | AsbestosCursor:
     # Use a flag to decide whether it returns the test cursor
```

### Comparing `asbestos_snow-1.2.0/asbestos/asbestos.py` & `asbestos_snow-1.3.0/asbestos/asbestos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 from asbestos.exceptions import AsbestosDuplicateQuery, AsbestosMissingConfig
 
 EXAMPLE_QUERY = "hello"
 EXAMPLE_RESPONSE = "world"
 
 # Monkeypatch this from anywhere to make Asbestos return whatever you need.
@@ -40,15 +40,15 @@
         response: dict[Any],
         ephemeral: bool = False,
         data: Optional[tuple[Any]] = None,
         force_pagination_size: Optional[int] = None,
     ) -> None:
         self.query: str = query
         self.data: Optional[tuple[Any]] = data
-        self.response: dict[Any] | list[dict[Any]] = response
+        self.response: Union[dict[Any], list[dict[Any]]] = response
         self.ephemeral: bool = ephemeral
         self.sfqid: int = 0
         self.force_pagination_size = force_pagination_size
         self.set_sfqid()
 
     def __str__(self) -> str:
         query = f"{self.query[:30]}..." if len(self.query) > 30 else self.query
@@ -319,15 +319,15 @@
         self.data = inserted_data
         self._get(remove_ephemeral=False)
 
     def execute_async(self, *args, **kwargs) -> None:
         """Functions the same as `.execute()`."""
         self.execute(*args, **kwargs)
 
-    def _get(self, remove_ephemeral: bool = True) -> dict | list[dict]:
+    def _get(self, remove_ephemeral: bool = True) -> Union[dict, list[dict]]:
         resp = self.config.lookup_query(self.query, self.data)
         if remove_ephemeral:
             self.config.remove_ephemeral_response(resp)
         self.config.last_run_query = resp
         return OVERRIDE_RESPONSE if OVERRIDE_RESPONSE else resp.response
 
     def fetchone(self) -> dict:
```

### Comparing `asbestos_snow-1.2.0/pyproject.toml` & `asbestos_snow-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "asbestos-snow"
-version = "1.2.0"
+version = "1.3.0"
 description = "An easy way to mock Snowflake connections in Python!"
 authors = ["Joe Kaufeld <jkaufeld@spoton.com>", "SpotOn <opensource@spoton.com>"]
 readme = "README.md"
 packages = [{include = "asbestos"}]
 repository = "https://github.com/spotoninc/asbestos"
 documentation = "https://spotoninc.github.io/asbestos"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Database",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: Mocking",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 seed-isort-config = "^2.2.0"
 pytest = "^7.2.0"
 pdbpp = "^0.10.3"
```

### Comparing `asbestos_snow-1.2.0/PKG-INFO` & `asbestos_snow-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: asbestos-snow
-Version: 1.2.0
+Version: 1.3.0
 Summary: An easy way to mock Snowflake connections in Python!
 Home-page: https://github.com/spotoninc/asbestos
 Author: Joe Kaufeld
 Author-email: jkaufeld@spoton.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Project-URL: Documentation, https://spotoninc.github.io/asbestos
 Project-URL: Repository, https://github.com/spotoninc/asbestos
 Description-Content-Type: text/markdown
 
 # asbestos
 An easy way to mock Snowflake connections in Python!
 
 ## What is this?
 
-`asbestos` is a library to allow easy mocking of Snowflake calls during local development or testing to save on costs and time. The docs have more information, but here's a quick example:
+`asbestos` is a library for Python 3.9+ to allow easy mocking of Snowflake calls during local development or testing to save on costs and time. The docs have more information, but here's a quick example:
 
 ```python
 from asbestos import asbestos_cursor, config as asbestos_config
 
 
 def snowflake_cursor() -> SnowflakeCursor | AsbestosCursor:
     # Use a flag to decide whether it returns the test cursor
```

