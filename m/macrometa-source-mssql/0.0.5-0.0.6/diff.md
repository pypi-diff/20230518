# Comparing `tmp/macrometa-source-mssql-0.0.5.tar.gz` & `tmp/macrometa-source-mssql-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mssql-0.0.5.tar", max compression
+gzip compressed data, was "macrometa-source-mssql-0.0.6.tar", max compression
```

## Comparing `macrometa-source-mssql-0.0.5.tar` & `macrometa-source-mssql-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11899 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/LICENSE
--rw-r--r--   0        0        0    34496 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/__init__.py
--rwxr-xr-x   0        0        0     1476 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/connection.py
--rw-r--r--   0        0        0     2287 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/sample_data.py
--rwxr-xr-x   0        0        0        0 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     8025 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/common.py
--rwxr-xr-x   0        0        0     2206 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/full_table.py
--rw-r--r--   0        0        0    14533 2023-05-17 10:29:09.147018 macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1537 2023-05-17 10:29:09.387022 macrometa-source-mssql-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.5/setup.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/LICENSE
+-rw-r--r--   0        0        0    34605 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/__init__.py
+-rwxr-xr-x   0        0        0     1476 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/connection.py
+-rw-r--r--   0        0        0     2287 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/sample_data.py
+-rwxr-xr-x   0        0        0        0 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     8025 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     2206 2023-05-18 06:04:38.735217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    14533 2023-05-18 06:04:38.739217 macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1537 2023-05-18 06:04:38.991217 macrometa-source-mssql-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.6/setup.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 macrometa-source-mssql-0.0.6/PKG-INFO
```

### Comparing `macrometa-source-mssql-0.0.5/LICENSE` & `macrometa-source-mssql-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.5/macrometa_source_mssql/__init__.py` & `macrometa-source-mssql-0.0.6/macrometa_source_mssql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
                            description='Microsoft SQL Server password.', placeholder_value='password'),
             ConfigProperty('database', 'Database Name', ConfigAttributeType.STRING, True, True,
                            description='Microsoft SQL Server database name.', default_value='master'),
             ConfigProperty('source_schema', 'Source Schema', ConfigAttributeType.STRING, True, True,
                            description='Source Schema to scan.', placeholder_value='my_schema'),
             ConfigProperty('source_table', 'Source Table', ConfigAttributeType.STRING, True, True,
                            description='Source Table to scan.', placeholder_value='my_table'),
-            ConfigProperty('default_replication_method', 'Replication Method', ConfigAttributeType.STRING, True, True,
+            ConfigProperty('replication_method', 'Replication Method', ConfigAttributeType.STRING, True, True,
                            description='Choose from LOG_BASED, FULL_TABLE.', default_value='FULL_TABLE'),
             ConfigProperty('characterset', 'Character Set', ConfigAttributeType.STRING, False, False,
                            description='The characterset of the Microsoft SQL Server database.', default_value='utf8'),
             ConfigProperty('tds_version', 'TDS Version', ConfigAttributeType.STRING, False, False,
                            description='Set the version of TDS to use when communicating with MS SQL Server.',
                            default_value='7.3'),
             ConfigProperty('use_date_datatype', 'Use Date data type', ConfigAttributeType.BOOLEAN, False, False,
@@ -206,15 +206,15 @@
                 'source_schema': integration['source_schema'],
                 'source_table': integration['source_table'],
 
                 # Optional config keys
                 'characterset': integration.get('characterset', "utf8"),
                 'tds_version': integration.get('tds_version', "7.3"),
                 'use_date_datatype': integration.get('use_date_datatype', False),
-                'default_replication_method': integration.get('default_replication_method', "FULL_TABLE")
+                'replication_method': integration.get('replication_method', "FULL_TABLE")
             }
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.') from e
 
 
 Column = collections.namedtuple(
     "Column",
@@ -342,14 +342,15 @@
 
 def discover_catalog(mssql_conn, config):
     """Returns a Catalog describing the structure of the database."""
     LOGGER.info("Preparing Catalog")
     mssql_conn = MSSQLConnection(config)
     source_schema = config.get("source_schema")
     source_table = config.get("source_table")
+    replication_method = config.get("replication_method")
     table_schema_clause = "WHERE c.table_schema = '{}' AND c.table_name='{}'".format(source_schema, source_table)
 
     with connect_with_backoff(mssql_conn) as open_conn:
         cur = open_conn.cursor()
         cur.execute(
             """SELECT table_schema,
                 table_name,
@@ -431,14 +432,16 @@
 
                 md_map = metadata.write(md_map, (), "is-view", is_view)
 
             key_properties = [c.column_name for c in cols if c.is_primary_key == 1]
 
             md_map = metadata.write(md_map, (), "table-key-properties", key_properties)
 
+            md_map = metadata.write(md_map, (), "replication-method", replication_method)
+
             entry = CatalogEntry(
                 table=table_name,
                 stream=table_name,
                 metadata=metadata.to_list(md_map),
                 tap_stream_id=common.generate_tap_stream_id(table_schema, table_name),
                 schema=schema,
             )
@@ -766,16 +769,16 @@
         # Emit a state message to indicate that we've started this stream
         singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
         md_map = metadata.to_map(catalog_entry.metadata)
         replication_method = md_map.get((), {}).get("replication-method")
         start_lsn = md_map.get((), {}).get("lsn")
         LOGGER.info(f"Table {catalog_entry.table} proposes {replication_method} sync")
-        if not replication_method and config.get("default_replication_method"):
-            replication_method = config.get("default_replication_method")
+        if not replication_method and config.get("replication_method"):
+            replication_method = config.get("replication_method")
             LOGGER.info(
                 f"Table {catalog_entry.table} reverting to DEFAULT {replication_method} sync"
             )
 
         if replication_method == "LOG_BASED" and not start_lsn:
             LOGGER.info(f"No initial load for {catalog_entry.table}, using full table replication")
         else:
```

### Comparing `macrometa-source-mssql-0.0.5/macrometa_source_mssql/connection.py` & `macrometa-source-mssql-0.0.6/macrometa_source_mssql/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.5/macrometa_source_mssql/sample_data.py` & `macrometa-source-mssql-0.0.6/macrometa_source_mssql/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/common.py` & `macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/full_table.py` & `macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.5/macrometa_source_mssql/sync_strategies/log_based.py` & `macrometa-source-mssql-0.0.6/macrometa_source_mssql/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mssql-0.0.5/pyproject.toml` & `macrometa-source-mssql-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mssql"
-version='0.0.5'
+version='0.0.6'
 description = "Macrometa Source for extracting data from Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mssql-0.0.5/setup.py` & `macrometa-source-mssql-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'pymssql>=2.2.1']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mssql = macrometa_source_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mssql',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Macrometa Source for extracting data from Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mssql-0.0.5/PKG-INFO` & `macrometa-source-mssql-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mssql
-Version: 0.0.5
+Version: 0.0.6
 Summary: Macrometa Source for extracting data from Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MSSQL,Microsoft SQL Server,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

