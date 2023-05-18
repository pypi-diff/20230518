# Comparing `tmp/questdb-connect-0.0.77.tar.gz` & `tmp/questdb-connect-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.77.tar", last modified: Thu May 18 19:10:56 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.78.tar", last modified: Thu May 18 19:44:39 2023, max compression
```

## Comparing `questdb-connect-0.0.77.tar` & `questdb-connect-0.0.78.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.606083 questdb-connect-0.0.77/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.77/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:10:56.605908 questdb-connect-0.0.77/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.77/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 19:09:46.000000 questdb-connect-0.0.77/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 19:10:56.606198 questdb-connect-0.0.77/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.597991 questdb-connect-0.0.77/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.600892 questdb-connect-0.0.77/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.77/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.77/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.77/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.77/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.77/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.77/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.602684 questdb-connect-0.0.77/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.77/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11890 2023-05-18 18:09:19.000000 questdb-connect-0.0.77/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.77/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    14296 2023-05-18 19:10:24.000000 questdb-connect-0.0.77/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     8532 2023-05-18 19:10:24.000000 questdb-connect-0.0.77/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.603897 questdb-connect-0.0.77/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.605239 questdb-connect-0.0.77/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.77/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.77/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.77/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.381457 questdb-connect-0.0.78/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.78/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:44:39.381321 questdb-connect-0.0.78/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.78/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 19:43:35.000000 questdb-connect-0.0.78/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 19:44:39.381496 questdb-connect-0.0.78/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.376042 questdb-connect-0.0.78/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.377991 questdb-connect-0.0.78/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.78/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.78/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.78/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.78/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.78/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.78/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.379637 questdb-connect-0.0.78/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.78/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11793 2023-05-18 19:29:38.000000 questdb-connect-0.0.78/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.78/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12639 2023-05-18 19:43:05.000000 questdb-connect-0.0.78/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10129 2023-05-18 19:43:05.000000 questdb-connect-0.0.78/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.380505 questdb-connect-0.0.78/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 19:44:39.000000 questdb-connect-0.0.78/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:44:39.381127 questdb-connect-0.0.78/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.78/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.78/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.78/tests/test_types.py
```

### Comparing `questdb-connect-0.0.77/LICENSE` & `questdb-connect-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/PKG-INFO` & `questdb-connect-0.0.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.77
+Version: 0.0.78
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.77/README.md` & `questdb-connect-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/pyproject.toml` & `questdb-connect-0.0.78/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.77'
+version = '0.0.78'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.77/src/examples/__init__.py` & `questdb-connect-0.0.78/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/examples/hello_world.py` & `questdb-connect-0.0.78/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.78/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/examples/server_utilisation.py` & `questdb-connect-0.0.78/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.78/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.78/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/questdb_connect/__init__.py` & `questdb-connect-0.0.78/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/questdb_connect/dialect.py` & `questdb-connect-0.0.78/src/questdb_connect/dialect.py`

 * *Files 5% similar despite different names*

```diff
@@ -228,26 +228,29 @@
             else:
                 table.append_column(Column(col_name, col_type))
         table.engine = QDBTableEngine(table_name, col_ts_name, partition_by, is_wal)
         table.metadata = MetaData()
 
     def get_columns(self, table_name, schema=None, **kw):
         result_set = self.bind.execute(f"table_columns('{table_name}')")
+        return self.format_table_columns(table_name, result_set)
+
+    def get_schema_names(self):
+        return ['public']
+
+    def format_table_columns(self, table_name, result_set):
         if not result_set:
             raise NoResultFound(f"Table '{table_name}' does not exist")
         return [{
             'name': row[0],
             'type': resolve_type_from_name(row[1])(),
             'nullable': True,
             'autoincrement': False,
         } for row in result_set]
 
-    def get_schema_names(self):
-        return ['public']
-
 
 class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
@@ -276,14 +279,24 @@
 
     def get_schema_names(self, connection, **kw):
         return ['public']
 
     def get_table_names(self, connection, schema=None, **kw):
         return [row.table for row in connection.execute(text('SHOW TABLES'))]
 
+    def has_table(self, connection, table_name, schema=None):
+        query = f"tables() WHERE name='{table_name}'"
+        result = connection.execute(text(query))
+        return result.rowcount == 1
+
+    @cache
+    def get_columns(self, connection, table_name, schema=None, **kw):
+        result_set = connection.execute(text(f"table_columns('{table_name}')"))
+        return self.inspector.format_table_columns(table_name, result_set)
+
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         return []
 
     def get_foreign_keys(self, connection, table_name, schema=None, postgresql_ignore_search_path=False, **kw):
         return []
 
     def get_temp_table_names(self, connection, **kw):
@@ -303,19 +316,14 @@
 
     def get_unique_constraints(self, connection, table_name, schema=None, **kw):
         return []
 
     def get_check_constraints(self, connection, table_name, schema=None, **kw):
         return []
 
-    def has_table(self, connection, table_name, schema=None):
-        query = f"tables() WHERE name='{table_name}'"
-        result = connection.execute(text(query))
-        return result.rowcount == 1
-
     def has_sequence(self, connection, sequence_name, schema=None, **_kw):
         return False
 
     def do_begin_twophase(self, connection, xid):
         raise NotImplementedError
 
     def do_prepare_twophase(self, connection, xid):
@@ -331,19 +339,7 @@
         raise NotImplementedError
 
     def set_isolation_level(self, dbapi_connection, level):
         pass
 
     def get_isolation_level(self, dbapi_connection):
         return None
-
-    @cache
-    def get_columns(self, connection, table_name, schema=None, **kw):
-        result_set = connection.execute(text(f"table_columns('{table_name}')"))
-        if not result_set:
-            raise NoResultFound(f"Table '{table_name}' does not exist")
-        return [{
-            'name': row[0],
-            'type': resolve_type_from_name(row[1])(),
-            'nullable': True,
-            'autoincrement': False,
-        } for row in result_set]
```

### Comparing `questdb-connect-0.0.77/src/questdb_connect/function_names.py` & `questdb-connect-0.0.78/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.78/src/questdb_connect/superset_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,47 +94,30 @@
     }
     ret_list = []
     for duration, func in _time_grain_expressions.items():
         if duration:
             name = builtin_time_grains[duration]
             ret_list.append(TimeGrain(name, _(name), func, duration))
     _engine_time_grains = tuple(ret_list)
-    _default_column_type_mappings = (
-        (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
-        (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
-        (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
-        (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
-        (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
-        (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
-        (re.compile("^FLOAT", re.IGNORECASE), types.Float, GenericDataType.NUMERIC),
-        (re.compile("^DOUBLE'", re.IGNORECASE), types.Double, GenericDataType.NUMERIC),
-        (re.compile("^SYMBOL", re.IGNORECASE), types.Symbol, GenericDataType.STRING),
-        (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
-        (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
-        (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
-        (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
-        (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
-        (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING)
-    )
-    column_type_mappings = _default_column_type_mappings
-    _column_type_to_generic_type_mapping = {  # GEOHASH is treated separately
+    _column_type_to_generic_type_mapping = {
         types.Boolean.__visit_name__: GenericDataType.BOOLEAN,
         types.Byte.__visit_name__: GenericDataType.NUMERIC,
         types.Short.__visit_name__: GenericDataType.NUMERIC,
         types.Int.__visit_name__: GenericDataType.NUMERIC,
         types.Long.__visit_name__: GenericDataType.NUMERIC,
         types.Float.__visit_name__: GenericDataType.NUMERIC,
         types.Double.__visit_name__: GenericDataType.NUMERIC,
         types.Symbol.__visit_name__: GenericDataType.STRING,
         types.String.__visit_name__: GenericDataType.STRING,
         types.Char.__visit_name__: GenericDataType.STRING,
         types.Long256.__visit_name__: GenericDataType.STRING,
         types.UUID.__visit_name__: GenericDataType.STRING,
         types.Timestamp.__visit_name__: GenericDataType.TEMPORAL,
         types.Date.__visit_name__: GenericDataType.TEMPORAL,
+        # GEOHASH (GenericDataType.STRING) is treated separately
     }
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
@@ -224,24 +207,16 @@
         """Return a sqlalchemy native column type and generic data type that
         corresponds to the column type defined in the data source (return None
         to use default type inferred by SQLAlchemy). Override `column_type_mappings`
         for specific needs (see MSSQL for example of NCHAR/NVARCHAR handling).
         :param column_type: Column type returned by inspector
         :return: SQLAlchemy and generic Superset column types
         """
-        if not column_type:
-            return None
-        for regex, sqla_type, generic_type in cls._default_column_type_mappings:
-            matching_name = regex.search(column_type)
-            if matching_name:
-                return (
-                    types.resolve_type_from_name(sqla_type.__visit_name__).impl,
-                    generic_type,
-                )
-        return None
+        column_spec = cls.get_column_spec()
+        return column_spec.sqla_type, column_spec.generic_type
 
     @classmethod
     def get_sqla_column_type(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
```

### Comparing `questdb-connect-0.0.77/src/questdb_connect/types.py` & `questdb-connect-0.0.78/src/questdb_connect/types.py`

 * *Files 25% similar despite different names*

```diff
@@ -251,23 +251,35 @@
 
 class QDBTypeCompiler(GenericTypeCompiler):
     ensure_kwarg = None
 
     def visit_GEOHASHINT(self, type_, **kw):
         return GeohashInt.__visit_name__
 
+    def visit_GeohashInt(self, type_, **kw):
+        return GeohashInt.__visit_name__
+
     def visit_GEOHASHLONG(self, type_, **kw):
         return GeohashLong.__visit_name__
 
+    def visit_GeohashLong(self, type_, **kw):
+        return GeohashLong.__visit_name__
+
     def visit_GEOHASHBYTE(self, type_, **kw):
         return GeohashByte.__visit_name__
 
+    def visit_GeohashByte(self, type_, **kw):
+        return GeohashByte.__visit_name__
+
     def visit_GEOHASHSHORT(self, type_, **kw):
         return GeohashShort.__visit_name__
 
+    def visit_GeohashShort(self, type_, **kw):
+        return GeohashShort.__visit_name__
+
     def visit_unsupported_compilation(self, element, err, **kw):
         if isinstance(element, GeohashLong):
             return GeohashLong.__visit_name__
         if isinstance(element, GeohashInt):
             return GeohashInt.__visit_name__
         if isinstance(element, GeohashShort):
             return GeohashShort.__visit_name__
@@ -277,59 +289,107 @@
             UnsupportedCompilationError(self, element),
             replace_context=err,
         )
 
     def visit_BOOLEAN(self, type_, **kw):
         return Boolean.__visit_name__
 
+    def visit_boolean(self, type_, **kw):
+        return Boolean.__visit_name__
+
     def visit_BOOL(self, type_, **kw):
         return Boolean.__visit_name__
 
+    def visit_bool(self, type_, **kw):
+        return Boolean.__visit_name__
+
     def visit_BYTE(self, type_, **kw):
         return Byte.__visit_name__
 
+    def visit_byte(self, type_, **kw):
+        return Byte.__visit_name__
+
     def visit_SHORT(self, type_, **kw):
         return Short.__visit_name__
 
+    def visit_short(self, type_, **kw):
+        return Short.__visit_name__
+
     def visit_CHAR(self, type_, **kw):
         return Char.__visit_name__
 
+    def visit_char(self, type_, **kw):
+        return Char.__visit_name__
+
     def visit_INT(self, type_, **kw):
         return Int.__visit_name__
 
+    def visit_int(self, type_, **kw):
+        return Int.__visit_name__
+
     def visit_INTEGER(self, type_, **kw):
         return Int.__visit_name__
 
+    def visit_integer(self, type_, **kw):
+        return Int.__visit_name__
+
     def visit_LONG(self, type_, **kw):
         return Long.__visit_name__
 
+    def visit_long(self, type_, **kw):
+        return Long.__visit_name__
+
     def visit_FLOAT(self, type_, **kw):
         return Float.__visit_name__
 
+    def visit_float(self, type_, **kw):
+        return Float.__visit_name__
+
     def visit_TIMESTAMP(self, type_, **kw):
         return Timestamp.__visit_name__
 
+    def visit_timestamp(self, type_, **kw):
+        return Timestamp.__visit_name__
+
     def visit_DATE(self, type_, **kw):
         return Date.__visit_name__
 
+    def visit_date(self, type_, **kw):
+        return Date.__visit_name__
+
     def visit_UUID(self, type_, **kw):
         return UUID.__visit_name__
 
+    def visit_uuid(self, type_, **kw):
+        return UUID.__visit_name__
+
     def visit_LONG256(self, type_, **kw):
         return Long256.__visit_name__
 
+    def visit_long256(self, type_, **kw):
+        return Long256.__visit_name__
+
     def visit_DOUBLE(self, type_, **kw):
         return Double.__visit_name__
 
+    def visit_double(self, type_, **kw):
+        return Double.__visit_name__
+
     def visit_STRING(self, type_, **kw):
         return String.__visit_name__
 
+    def visit_string(self, type_, **kw):
+        return String.__visit_name__
+
     def visit_SYMBOL(self, type_, **kw):
         return Symbol.__visit_name__
 
+    def visit_symbol(self, type_, **kw):
+        return Symbol.__visit_name__
+
     def _render_string_type(self, type_, name):
         return name
 
     def visit_null(self, type_, **kw):
         raise CompileError(f'cannot generate DDL for type: {type_}')
 
     def visit_type_decorator(self, type_, **kw):
```

### Comparing `questdb-connect-0.0.77/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.78/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.77
+Version: 0.0.78
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.77/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.78/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/tests/test_dialect.py` & `questdb-connect-0.0.78/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/tests/test_superset.py` & `questdb-connect-0.0.78/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.77/tests/test_types.py` & `questdb-connect-0.0.78/tests/test_types.py`

 * *Files identical despite different names*

