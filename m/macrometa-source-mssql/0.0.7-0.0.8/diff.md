# Comparing `tmp/macrometa-source-mssql-0.0.7.tar.gz` & `tmp/macrometa-source-mssql-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.7.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-0.0.8.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.7.tar` & `macrometa-source-mssql-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/LICENSE
--rw-r--r--   0        0        0    34634 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1476 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2287 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-18 09:00:09.997575 macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1537 2023-05-18 09:00:10.245578 macrometa-source-mssql-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.7/setup.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/LICENSE
+-rw-r--r--   0        0        0    34837 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1476 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8025 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2206 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    14533 2023-05-18 11:18:43.334210 macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1537 2023-05-18 11:18:43.578209 macrometa-source-mssql-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.8/setup.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.8/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.7/LICENSE` & `macrometa-source-mssql-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.7/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-0.0.8/macrometa_source_mssql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -734,14 +734,15 @@
         state, catalog_entry.tap_stream_id, "initial_full_table_complete", True
     )
 
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def do_sync_log_based(mssql_conn, config, catalog_entry, state, columns):
+    LOGGER.info(f"inside do_sync_log_based...")
     mssql_conn = MSSQLConnection(config)
     md_map = metadata.to_map(catalog_entry.metadata)
     replication_key = md_map.get((), {}).get("replication-key")
     # Add additional keys to the schema
     log_based.add_synthetic_keys_to_schema(catalog_entry)
 
     LOGGER.info("SingerSchema written")
@@ -800,15 +801,15 @@
 
     state = singer.set_currently_syncing(state, None)
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def sync_cdc_streams(mssql_conn, cdc_catalog, config, state):
     mssql_conn = MSSQLConnection(config)
-
+    LOGGER.info(f"inside sync_cdc_streams...")
     if cdc_catalog.streams:
         for catalog_entry in cdc_catalog.streams:
             columns = list(catalog_entry.schema.properties.keys())
             if not columns:
                 LOGGER.warning(
                     "There are no columns selected for stream %s, skipping it.",
                     catalog_entry.stream,
@@ -833,19 +834,21 @@
 
         state = singer.set_currently_syncing(state, None)
         singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def do_sync(mssql_conn, config, catalog, state):
     LOGGER.info("Beginning sync")
+    replication_method = config.get("replication_method")
     non_cdc_catalog = get_non_cdc_streams(mssql_conn, catalog, config, state)
-    cdc_catalog = get_cdc_streams(mssql_conn, catalog, config, state)
+    cdc_catalog = catalog if replication_method == "LOG_BASED" else get_cdc_streams(mssql_conn, catalog, config, state)
 
     for entry in non_cdc_catalog.streams:
         LOGGER.info(f"Need to sync {entry.table}")
+
     sync_non_cdc_streams(mssql_conn, non_cdc_catalog, config, state)
     sync_cdc_streams(mssql_conn, cdc_catalog, config, state)
 
 
 def log_server_params(mssql_conn):
     with connect_with_backoff(mssql_conn) as open_conn:
         try:
```

### Comparing `macrometa-source-mssql-0.0.7/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-0.0.8/macrometa_source_mssql/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.7/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.7/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-0.0.8/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.7/pyproject.toml` & `macrometa-source-mssql-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.7'
+version='0.0.8'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mssql-0.0.7/setup.py` & `macrometa-source-mssql-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.7/PKG-INFO` & `macrometa-source-mssql-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.7
+Version: 0.0.8
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

