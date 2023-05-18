# Comparing `tmp/stac-fastapi.pgstac-2.4.6.tar.gz` & `tmp/stac-fastapi.pgstac-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.pgstac-2.4.6.tar", last modified: Thu May 11 15:16:57 2023, max compression
+gzip compressed data, was "stac-fastapi.pgstac-2.4.7.tar", last modified: Thu May 18 12:48:46 2023, max compression
```

## Comparing `stac-fastapi.pgstac-2.4.6.tar` & `stac-fastapi.pgstac-2.4.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 15:16:57.000000 stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.225381 stac-fastapi.pgstac-2.4.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:57.229380 stac-fastapi.pgstac-2.4.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-11 15:16:45.000000 stac-fastapi.pgstac-2.4.6/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 12:48:46.000000 stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21437 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.943508 stac-fastapi.pgstac-2.4.7/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:46.947508 stac-fastapi.pgstac-2.4.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50432 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-18 12:48:37.000000 stac-fastapi.pgstac-2.4.7/tests/resources/test_mgmt.py
```

### Comparing `stac-fastapi.pgstac-2.4.6/LICENSE` & `stac-fastapi.pgstac-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/PKG-INFO` & `stac-fastapi.pgstac-2.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.6
+Version: 2.4.7
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.pgstac-2.4.6/README.md` & `stac-fastapi.pgstac-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/setup.py` & `stac-fastapi.pgstac-2.4.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     desc = f.read()
 
 install_requires = [
     "attrs",
     "orjson",
     "pydantic[dotenv]",
     "stac_pydantic==2.0.*",
-    "stac-fastapi.types",
-    "stac-fastapi.api",
-    "stac-fastapi.extensions",
+    "stac-fastapi.types~=2.4.7",
+    "stac-fastapi.api~=2.4.7",
+    "stac-fastapi.extensions~=2.4.7",
     "asyncpg",
     "buildpg",
     "brotli_asgi",
     "pygeofilter>=0.2",
     "pypgstac==0.7.*",
 ]
```

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/app.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/config.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 """Postgres API configuration."""
 
-from typing import Type
+from typing import List, Type
 from urllib.parse import quote
 
 from stac_fastapi.types.config import ApiSettings
 
 from stac_fastapi.pgstac.types.base_item_cache import (
     BaseItemCache,
     DefaultBaseItemCache,
 )
 
+DEFAULT_INVALID_ID_CHARS = [
+    ":",
+    "/",
+    "?",
+    "#",
+    "[",
+    "]",
+    "@",
+    "!",
+    "$",
+    "&",
+    "'",
+    "(",
+    ")",
+    "*",
+    "+",
+    ",",
+    ";",
+    "=",
+]
+
 
 class Settings(ApiSettings):
     """Postgres-specific API settings.
 
     Attributes:
         postgres_user: postgres username.
         postgres_pass: postgres password.
         postgres_host_reader: hostname for the reader connection.
         postgres_host_writer: hostname for the writer connection.
         postgres_port: database port.
         postgres_dbname: database name.
         use_api_hydrate: perform hydration of stac items within stac-fastapi.
+        invalid_id_chars: list of characters that are not allowed in item or collection ids.
     """
 
     postgres_user: str
     postgres_pass: str
     postgres_host_reader: str
     postgres_host_writer: str
     postgres_port: str
@@ -34,14 +56,15 @@
     db_min_conn_size: int = 10
     db_max_conn_size: int = 10
     db_max_queries: int = 50000
     db_max_inactive_conn_lifetime: float = 300
 
     use_api_hydrate: bool = False
     base_item_cache: Type[BaseItemCache] = DefaultBaseItemCache
+    invalid_id_chars: List[str] = DEFAULT_INVALID_ID_CHARS
 
     testing: bool = False
 
     @property
     def reader_connection_string(self):
         """Create reader psql connection string."""
         return f"postgresql://{self.postgres_user}:{quote(self.postgres_pass)}@{self.postgres_host_reader}:{self.postgres_port}/{self.postgres_dbname}"
```

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/core.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/core.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/db.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/filter.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/extensions/query.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/models/links.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/models/links.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/base_item_cache.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/types/search.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/types/search.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi/pgstac/utils.py` & `stac-fastapi.pgstac-2.4.7/stac_fastapi/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 2.4.6
+Version: 2.4.7
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.pgstac-2.4.6/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac-fastapi.pgstac-2.4.7/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/tests/api/test_api.py` & `stac-fastapi.pgstac-2.4.7/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/tests/clients/test_postgres.py` & `stac-fastapi.pgstac-2.4.7/tests/resources/test_collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-import logging
-import uuid
-from contextlib import asynccontextmanager
-from copy import deepcopy
-from typing import Callable, Literal
+from typing import Callable
 
+import pystac
 import pytest
-from fastapi import Request
-from stac_pydantic import Collection, Item
-
-from stac_fastapi.pgstac.db import close_db_connection, connect_to_db, get_connection
-
-# from tests.conftest import MockStarletteRequest
-logger = logging.getLogger(__name__)
+from stac_pydantic import Collection
 
 
 async def test_create_collection(app_client, load_test_data: Callable):
     in_json = load_test_data("test_collection.json")
     in_coll = Collection.parse_obj(in_json)
     resp = await app_client.post(
         "/collections",
@@ -25,188 +16,229 @@
     post_coll = Collection.parse_obj(resp.json())
     assert in_coll.dict(exclude={"links"}) == post_coll.dict(exclude={"links"})
     resp = await app_client.get(f"/collections/{post_coll.id}")
     assert resp.status_code == 200
     get_coll = Collection.parse_obj(resp.json())
     assert post_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
 
+    post_self_link = next(
+        (link for link in post_coll.links if link.rel == "self"), None
+    )
+    get_self_link = next((link for link in get_coll.links if link.rel == "self"), None)
+    assert post_self_link is not None and get_self_link is not None
+    assert post_self_link.href == get_self_link.href
 
-async def test_update_collection(app_client, load_test_collection):
+
+async def test_update_collection(app_client, load_test_data, load_test_collection):
     in_coll = load_test_collection
     in_coll.keywords.append("newkeyword")
 
     resp = await app_client.put("/collections", json=in_coll.dict())
     assert resp.status_code == 200
+    put_coll = Collection.parse_obj(resp.json())
 
     resp = await app_client.get(f"/collections/{in_coll.id}")
     assert resp.status_code == 200
 
     get_coll = Collection.parse_obj(resp.json())
     assert in_coll.dict(exclude={"links"}) == get_coll.dict(exclude={"links"})
     assert "newkeyword" in get_coll.keywords
 
+    put_self_link = next((link for link in put_coll.links if link.rel == "self"), None)
+    get_self_link = next((link for link in get_coll.links if link.rel == "self"), None)
+    assert put_self_link is not None and get_self_link is not None
+    assert put_self_link.href == get_self_link.href
+
 
-async def test_delete_collection(app_client, load_test_collection):
+async def test_delete_collection(
+    app_client, load_test_data: Callable, load_test_collection
+):
     in_coll = load_test_collection
 
     resp = await app_client.delete(f"/collections/{in_coll.id}")
     assert resp.status_code == 200
 
     resp = await app_client.get(f"/collections/{in_coll.id}")
     assert resp.status_code == 404
 
 
-async def test_create_item(app_client, load_test_data: Callable, load_test_collection):
-    coll = load_test_collection
-
-    in_json = load_test_data("test_item.json")
-    in_item = Item.parse_obj(in_json)
+async def test_create_collection_conflict(app_client, load_test_data: Callable):
+    in_json = load_test_data("test_collection.json")
+    Collection.parse_obj(in_json)
     resp = await app_client.post(
-        f"/collections/{coll.id}/items",
+        "/collections",
         json=in_json,
     )
     assert resp.status_code == 200
+    Collection.parse_obj(resp.json())
+    resp = await app_client.post(
+        "/collections",
+        json=in_json,
+    )
+    assert resp.status_code == 409
 
-    post_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == post_item.dict(exclude={"links"})
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{post_item.id}")
+async def test_delete_missing_collection(
+    app_client,
+):
+    resp = await app_client.delete("/collections")
+    assert resp.status_code == 405
 
-    assert resp.status_code == 200
 
-    get_item = Item.parse_obj(resp.json())
-    assert in_item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
+async def test_update_new_collection(app_client, load_test_collection):
+    in_coll = load_test_collection
+    in_coll.id = "test-updatenew"
 
+    resp = await app_client.put("/collections", json=in_coll.dict())
+    assert resp.status_code == 404
 
-async def test_update_item(app_client, load_test_collection, load_test_item):
-    coll = load_test_collection
-    item = load_test_item
 
-    item.properties.description = "Update Test"
+async def test_nocollections(
+    app_client,
+):
+    resp = await app_client.get("/collections")
+    assert resp.status_code == 200
 
-    resp = await app_client.put(
-        f"/collections/{coll.id}/items/{item.id}", content=item.json()
+
+async def test_returns_valid_collection(app_client, load_test_data):
+    """Test updating a collection which already exists"""
+    in_json = load_test_data("test_collection.json")
+    resp = await app_client.post(
+        "/collections",
+        json=in_json,
     )
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item.id}")
+    resp = await app_client.get(f"/collections/{in_json['id']}")
     assert resp.status_code == 200
-    get_item = Item.parse_obj(resp.json())
-    assert item.dict(exclude={"links"}) == get_item.dict(exclude={"links"})
-    assert get_item.properties.description == "Update Test"
+    resp_json = resp.json()
 
+    # Mock root to allow validation
+    mock_root = pystac.Catalog(
+        id="test", description="test desc", href="https://example.com"
+    )
+    collection = pystac.Collection.from_dict(
+        resp_json, root=mock_root, preserve_dict=False
+    )
+    collection.validate()
 
-async def test_delete_item(app_client, load_test_collection, load_test_item):
-    coll = load_test_collection
-    item = load_test_item
 
-    resp = await app_client.delete(f"/collections/{coll.id}/items/{item.id}")
+async def test_returns_valid_links_in_collections(app_client, load_test_data):
+    """Test links from listing collections"""
+    in_json = load_test_data("test_collection.json")
+    resp = await app_client.post(
+        "/collections",
+        json=in_json,
+    )
     assert resp.status_code == 200
 
-    resp = await app_client.get(f"/collections/{coll.id}/items/{item.id}")
-    assert resp.status_code == 404
-
-
-async def test_get_collection_items(app_client, load_test_collection, load_test_item):
-    coll = load_test_collection
-    item = load_test_item
-
-    for _ in range(4):
-        item.id = str(uuid.uuid4())
-        resp = await app_client.post(
-            f"/collections/{coll.id}/items",
-            content=item.json(),
-        )
-        assert resp.status_code == 200
+    # Get collection by ID
+    resp = await app_client.get(f"/collections/{in_json['id']}")
+    assert resp.status_code == 200
+    resp_json = resp.json()
 
-    resp = await app_client.get(
-        f"/collections/{coll.id}/items",
+    # Mock root to allow validation
+    mock_root = pystac.Catalog(
+        id="test", description="test desc", href="https://example.com"
     )
+    collection = pystac.Collection.from_dict(
+        resp_json, root=mock_root, preserve_dict=False
+    )
+    assert collection.validate()
+
+    # List collections
+    resp = await app_client.get("/collections")
     assert resp.status_code == 200
-    fc = resp.json()
-    assert "features" in fc
-    assert len(fc["features"]) == 5
+    resp_json = resp.json()
+    collections = resp_json["collections"]
+    # Find collection in list by ID
+    single_coll = next(coll for coll in collections if coll["id"] == in_json["id"])
+    is_coll_from_list_valid = False
+    single_coll_mocked_link = dict()
+    if single_coll is not None:
+        single_coll_mocked_link = pystac.Collection.from_dict(
+            single_coll, root=mock_root, preserve_dict=False
+        )
+        is_coll_from_list_valid = single_coll_mocked_link.validate()
 
+    assert is_coll_from_list_valid
 
-async def test_create_bulk_items(
-    app_client, load_test_data: Callable, load_test_collection
-):
-    coll = load_test_collection
-    item = load_test_data("test_item.json")
+    # Check links from the collection GET and list
+    assert [
+        i
+        for i in collection.to_dict()["links"]
+        if i not in single_coll_mocked_link.to_dict()["links"]
+    ] == []
 
-    items = {}
-    for _ in range(2):
-        _item = deepcopy(item)
-        _item["id"] = str(uuid.uuid4())
-        items[_item["id"]] = _item
 
-    payload = {"items": items}
+async def test_returns_license_link(app_client, load_test_collection):
+    coll = load_test_collection
 
-    resp = await app_client.post(
-        f"/collections/{coll.id}/bulk_items",
-        json=payload,
-    )
+    resp = await app_client.get(f"/collections/{coll.id}")
     assert resp.status_code == 200
-    assert resp.text == '"Successfully added 2 items."'
+    resp_json = resp.json()
+    link_rel_types = [link["rel"] for link in resp_json["links"]]
+    assert "license" in link_rel_types
 
-    for item_id in items.keys():
-        resp = await app_client.get(f"/collections/{coll.id}/items/{item_id}")
-        assert resp.status_code == 200
 
+@pytest.mark.asyncio
+async def test_get_collection_forwarded_header(app_client, load_test_collection):
+    coll = load_test_collection
+    resp = await app_client.get(
+        f"/collections/{coll.id}",
+        headers={"Forwarded": "proto=https;host=test:1234"},
+    )
+    for link in [
+        link
+        for link in resp.json()["links"]
+        if link["rel"] in ["items", "parent", "root", "self"]
+    ]:
+        assert link["href"].startswith("https://test:1234/")
 
-# TODO since right now puts implement upsert
-# test_create_collection_already_exists
-# test create_item_already_exists
-
-
-# def test_get_collection_items(
-#     postgres_core: CoreCrudClient,
-#     postgres_transactions: TransactionsClient,
-#     load_test_data: Callable,
-# ):
-#     coll = Collection.parse_obj(load_test_data("test_collection.json"))
-#     postgres_transactions.create_collection(coll, request=MockStarletteRequest)
-
-#     item = Item.parse_obj(load_test_data("test_item.json"))
 
-#     for _ in range(5):
-#         item.id = str(uuid.uuid4())
-#         postgres_transactions.create_item(item, request=MockStarletteRequest)
+@pytest.mark.asyncio
+async def test_get_collection_x_forwarded_headers(app_client, load_test_collection):
+    coll = load_test_collection
+    resp = await app_client.get(
+        f"/collections/{coll.id}",
+        headers={
+            "X-Forwarded-Port": "1234",
+            "X-Forwarded-Proto": "https",
+        },
+    )
+    for link in [
+        link
+        for link in resp.json()["links"]
+        if link["rel"] in ["items", "parent", "root", "self"]
+    ]:
+        assert link["href"].startswith("https://test:1234/")
 
-#     fc = postgres_core.item_collection(coll.id, request=MockStarletteRequest)
-#     assert len(fc.features) == 5
 
-#     for item in fc.features:
-#         assert item.collection == coll.id
+@pytest.mark.asyncio
+async def test_get_collection_duplicate_forwarded_headers(
+    app_client, load_test_collection
+):
+    coll = load_test_collection
+    resp = await app_client.get(
+        f"/collections/{coll.id}",
+        headers={
+            "Forwarded": "proto=https;host=test:1234",
+            "X-Forwarded-Port": "4321",
+            "X-Forwarded-Proto": "http",
+        },
+    )
+    for link in [
+        link
+        for link in resp.json()["links"]
+        if link["rel"] in ["items", "parent", "root", "self"]
+    ]:
+        assert link["href"].startswith("https://test:1234/")
 
 
-@asynccontextmanager
-async def custom_get_connection(
-    request: Request,
-    readwrite: Literal["r", "w"],
-):
-    """An example of customizing the connection getter"""
-    async with get_connection(request, readwrite) as conn:
-        await conn.execute("SELECT set_config('api.test', 'added-config', false)")
-        yield conn
-
-
-class TestDbConnect:
-    @pytest.fixture
-    async def app(self, api_client):
-        """
-        app fixture override to setup app with a customized db connection getter
-        """
-        logger.debug("Customizing app setup")
-        await connect_to_db(api_client.app, custom_get_connection)
-        yield api_client.app
-        await close_db_connection(api_client.app)
-
-    async def test_db_setup(self, api_client, app_client):
-        @api_client.app.get(f"{api_client.router.prefix}/db-test")
-        async def example_view(request: Request):
-            async with request.app.state.get_connection(request, "r") as conn:
-                return await conn.fetchval("SELECT current_setting('api.test', true)")
-
-        response = await app_client.get("/db-test")
-        assert response.status_code == 200
-        assert response.json() == "added-config"
+@pytest.mark.asyncio
+async def test_get_collections_forwarded_header(app_client, load_test_collection):
+    resp = await app_client.get(
+        "/collections",
+        headers={"Forwarded": "proto=https;host=test:1234"},
+    )
+    for link in resp.json()["links"]:
+        assert link["href"].startswith("https://test:1234/")
```

### Comparing `stac-fastapi.pgstac-2.4.6/tests/resources/test_conformance.py` & `stac-fastapi.pgstac-2.4.7/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.pgstac-2.4.6/tests/resources/test_item.py` & `stac-fastapi.pgstac-2.4.7/tests/resources/test_item.py`

 * *Files identical despite different names*

