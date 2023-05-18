# Comparing `tmp/questdb-connect-0.0.76.tar.gz` & `tmp/questdb-connect-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.76.tar", last modified: Thu May 18 18:10:32 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.77.tar", last modified: Thu May 18 19:10:56 2023, max compression
```

## Comparing `questdb-connect-0.0.76.tar` & `questdb-connect-0.0.77.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 18:10:32.452584 questdb-connect-0.0.76/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.76/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 18:10:32.452445 questdb-connect-0.0.76/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.76/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 18:09:11.000000 questdb-connect-0.0.76/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 18:10:32.452623 questdb-connect-0.0.76/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 18:10:32.446542 questdb-connect-0.0.76/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 18:10:32.449146 questdb-connect-0.0.76/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.76/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.76/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.76/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.76/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.76/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.76/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 18:10:32.450529 questdb-connect-0.0.76/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.76/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11890 2023-05-18 18:09:19.000000 questdb-connect-0.0.76/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.76/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    13668 2023-05-18 18:09:11.000000 questdb-connect-0.0.76/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     8454 2023-05-18 18:09:19.000000 questdb-connect-0.0.76/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 18:10:32.451372 questdb-connect-0.0.76/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 18:10:32.000000 questdb-connect-0.0.76/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 18:10:32.000000 questdb-connect-0.0.76/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 18:10:32.000000 questdb-connect-0.0.76/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 18:10:32.000000 questdb-connect-0.0.76/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 18:10:32.000000 questdb-connect-0.0.76/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 18:10:32.000000 questdb-connect-0.0.76/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 18:10:32.452064 questdb-connect-0.0.76/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.76/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.76/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.76/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.606083 questdb-connect-0.0.77/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.77/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:10:56.605908 questdb-connect-0.0.77/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.77/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 19:09:46.000000 questdb-connect-0.0.77/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 19:10:56.606198 questdb-connect-0.0.77/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.597991 questdb-connect-0.0.77/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.600892 questdb-connect-0.0.77/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.77/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.77/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.77/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.77/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.77/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.77/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.602684 questdb-connect-0.0.77/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.77/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11890 2023-05-18 18:09:19.000000 questdb-connect-0.0.77/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.77/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    14296 2023-05-18 19:10:24.000000 questdb-connect-0.0.77/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     8532 2023-05-18 19:10:24.000000 questdb-connect-0.0.77/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.603897 questdb-connect-0.0.77/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 19:10:56.000000 questdb-connect-0.0.77/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 19:10:56.605239 questdb-connect-0.0.77/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.77/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.77/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.77/tests/test_types.py
```

### Comparing `questdb-connect-0.0.76/LICENSE` & `questdb-connect-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/PKG-INFO` & `questdb-connect-0.0.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.76
+Version: 0.0.77
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.76/README.md` & `questdb-connect-0.0.77/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/pyproject.toml` & `questdb-connect-0.0.77/pyproject.toml`

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
-version = '0.0.76'
+version = '0.0.77'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.76/src/examples/__init__.py` & `questdb-connect-0.0.77/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/examples/hello_world.py` & `questdb-connect-0.0.77/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.77/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/examples/server_utilisation.py` & `questdb-connect-0.0.77/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.77/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.77/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/questdb_connect/__init__.py` & `questdb-connect-0.0.77/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/questdb_connect/dialect.py` & `questdb-connect-0.0.77/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/questdb_connect/function_names.py` & `questdb-connect-0.0.77/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.77/src/questdb_connect/superset_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,36 +68,37 @@
     time_groupby_inline = True
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     try_remove_schema_from_table_name = True
     max_column_name_length = 120
     supports_dynamic_schema = False
     top_keywords = {}
+    # https://en.wikipedia.org/wiki/ISO_8601#Durations
     # https://questdb.io/docs/reference/function/date-time/#date_trunc
     _time_grain_expressions = {
         None: '{col}',
         "PT1S": "date_trunc('second', {col})",
         "PT5S": "date_trunc('second', {col}) + 5000000L",
         "PT30S": "date_trunc('second', {col}) + 30000000L",
         "PT1M": "date_trunc('minute', {col})",
         "PT5M": "date_trunc('minute', {col}) + 300000000L",
         "PT10M": "date_trunc('minute', {col}) + 600000000L",
         "PT15M": "date_trunc('minute', {col}) + 900000000L",
         "PT30M": "date_trunc('minute', {col}) + 1800000000L",
         "PT1H": "date_trunc('hour', {col})",
         "PT6H": "date_trunc('hour', {col}) + 21600000000L",
-        "PT1D": "date_trunc('day', {col})",
+        "P1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P3M": "date_trunc('quarter', {col})",
     }
     ret_list = []
     for duration, func in _time_grain_expressions.items():
-        if duration in builtin_time_grains:
+        if duration:
             name = builtin_time_grains[duration]
             ret_list.append(TimeGrain(name, _(name), func, duration))
     _engine_time_grains = tuple(ret_list)
     _default_column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
@@ -111,14 +112,30 @@
         (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
         (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
         (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
         (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
         (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING)
     )
     column_type_mappings = _default_column_type_mappings
+    _column_type_to_generic_type_mapping = {  # GEOHASH is treated separately
+        types.Boolean.__visit_name__: GenericDataType.BOOLEAN,
+        types.Byte.__visit_name__: GenericDataType.NUMERIC,
+        types.Short.__visit_name__: GenericDataType.NUMERIC,
+        types.Int.__visit_name__: GenericDataType.NUMERIC,
+        types.Long.__visit_name__: GenericDataType.NUMERIC,
+        types.Float.__visit_name__: GenericDataType.NUMERIC,
+        types.Double.__visit_name__: GenericDataType.NUMERIC,
+        types.Symbol.__visit_name__: GenericDataType.STRING,
+        types.String.__visit_name__: GenericDataType.STRING,
+        types.Char.__visit_name__: GenericDataType.STRING,
+        types.Long256.__visit_name__: GenericDataType.STRING,
+        types.UUID.__visit_name__: GenericDataType.STRING,
+        types.Timestamp.__visit_name__: GenericDataType.TEMPORAL,
+        types.Date.__visit_name__: GenericDataType.TEMPORAL,
+    }
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
@@ -212,16 +229,18 @@
         :return: SQLAlchemy and generic Superset column types
         """
         if not column_type:
             return None
         for regex, sqla_type, generic_type in cls._default_column_type_mappings:
             matching_name = regex.search(column_type)
             if matching_name:
-                qdbcd_type = types.resolve_type_from_name(sqla_type.__visit_name__)
-                return qdbcd_type.impl, generic_type
+                return (
+                    types.resolve_type_from_name(sqla_type.__visit_name__).impl,
+                    generic_type,
+                )
         return None
 
     @classmethod
     def get_sqla_column_type(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
@@ -298,19 +317,11 @@
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         if not native_type:
             return None
         sqla_type = types.resolve_type_from_name(native_type)
         name_u = sqla_type.__visit_name__
-        generic_type = None
-        if name_u == 'BOOLEAN':
-            generic_type = GenericDataType.BOOLEAN
-        elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
-            generic_type = GenericDataType.NUMERIC
-        elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
-            generic_type = GenericDataType.STRING
-        elif name_u in ('DATE', 'TIMESTAMP'):
-            generic_type = GenericDataType.TEMPORAL
-        elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+        generic_type = cls._column_type_to_generic_type_mapping.get(name_u)
+        if not generic_type and 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
             generic_type = GenericDataType.STRING
         return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
```

### Comparing `questdb-connect-0.0.76/src/questdb_connect/types.py` & `questdb-connect-0.0.77/src/questdb_connect/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,17 @@
             UnsupportedCompilationError(self, element),
             replace_context=err,
         )
 
     def visit_BOOLEAN(self, type_, **kw):
         return Boolean.__visit_name__
 
+    def visit_BOOL(self, type_, **kw):
+        return Boolean.__visit_name__
+
     def visit_BYTE(self, type_, **kw):
         return Byte.__visit_name__
 
     def visit_SHORT(self, type_, **kw):
         return Short.__visit_name__
 
     def visit_CHAR(self, type_, **kw):
```

### Comparing `questdb-connect-0.0.76/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.77/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.76
+Version: 0.0.77
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.76/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.77/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/tests/test_dialect.py` & `questdb-connect-0.0.77/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/tests/test_superset.py` & `questdb-connect-0.0.77/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.76/tests/test_types.py` & `questdb-connect-0.0.77/tests/test_types.py`

 * *Files identical despite different names*

