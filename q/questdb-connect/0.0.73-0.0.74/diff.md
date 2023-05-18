# Comparing `tmp/questdb-connect-0.0.73.tar.gz` & `tmp/questdb-connect-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.73.tar", last modified: Thu May 18 15:02:43 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.74.tar", last modified: Thu May 18 15:18:54 2023, max compression
```

## Comparing `questdb-connect-0.0.73.tar` & `questdb-connect-0.0.74.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.684349 questdb-connect-0.0.73/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.73/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:02:43.684220 questdb-connect-0.0.73/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.73/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 15:02:26.000000 questdb-connect-0.0.73/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 15:02:43.684390 questdb-connect-0.0.73/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.678477 questdb-connect-0.0.73/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.680933 questdb-connect-0.0.73/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.73/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.73/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.73/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.73/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.73/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.73/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.682350 questdb-connect-0.0.73/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.73/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11858 2023-05-18 15:00:07.000000 questdb-connect-0.0.73/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.73/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12264 2023-05-18 15:00:47.000000 questdb-connect-0.0.73/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)    10302 2023-05-18 15:01:46.000000 questdb-connect-0.0.73/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.683248 questdb-connect-0.0.73/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.683849 questdb-connect-0.0.73/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.73/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.73/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.73/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.146063 questdb-connect-0.0.74/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.74/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:18:54.145902 questdb-connect-0.0.74/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.74/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 15:17:05.000000 questdb-connect-0.0.74/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 15:18:54.146109 questdb-connect-0.0.74/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.138987 questdb-connect-0.0.74/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.141593 questdb-connect-0.0.74/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.74/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.74/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.74/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.74/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.74/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.74/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.143295 questdb-connect-0.0.74/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.74/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11858 2023-05-18 15:00:07.000000 questdb-connect-0.0.74/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.74/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13668 2023-05-18 15:17:05.000000 questdb-connect-0.0.74/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10141 2023-05-18 15:17:11.000000 questdb-connect-0.0.74/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.144306 questdb-connect-0.0.74/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.145437 questdb-connect-0.0.74/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.74/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.74/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.74/tests/test_types.py
```

### Comparing `questdb-connect-0.0.73/LICENSE` & `questdb-connect-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/PKG-INFO` & `questdb-connect-0.0.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.73
+Version: 0.0.74
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.73/README.md` & `questdb-connect-0.0.74/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/pyproject.toml` & `questdb-connect-0.0.74/pyproject.toml`

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
-version = '0.0.73'
+version = '0.0.74'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.73/src/examples/__init__.py` & `questdb-connect-0.0.74/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/examples/hello_world.py` & `questdb-connect-0.0.74/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.74/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/examples/server_utilisation.py` & `questdb-connect-0.0.74/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.74/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.74/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/questdb_connect/__init__.py` & `questdb-connect-0.0.74/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/questdb_connect/dialect.py` & `questdb-connect-0.0.74/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/questdb_connect/function_names.py` & `questdb-connect-0.0.74/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.74/src/questdb_connect/superset_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 from . import remove_public_schema, types
 from .dialect import connection_uri
 from .function_names import FUNCTION_NAMES
 
-# https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
+# https://superset.apache.org/docs/databases/installing-database-drivers
 # https://preset.io/blog/building-database-connector/
 # https://preset.io/blog/improving-apache-superset-integration-database-sqlalchemy/
 
 
 class QDBParametersSchema(Schema):
     username = fields.String(allow_none=True, description=__('user'))
     password = fields.String(allow_none=True, description=__('password'))
@@ -127,15 +127,15 @@
             int(parameters.get("port")),
             parameters.get("username"),
             parameters.get("password"),
             parameters.get("database"))
 
     @classmethod
     def get_default_schema_for_query(cls, database, query) -> Optional[str]:
-        return ['public']
+        return 'public'
 
     @classmethod
     def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
         return False
 
     @classmethod
     def get_view_names(cls, database, inspector, schema: Optional[str]):
@@ -280,7 +280,37 @@
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
+
+    @classmethod
+    def get_column_spec(
+            cls,
+            native_type: Optional[str],
+            db_extra: Optional[Dict[str, Any]] = None,
+            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
+    ) -> Optional[utils.ColumnSpec]:
+        """Get generic type related specs regarding a native column type.
+        :param native_type: Native database type
+        :param db_extra: The database extra object
+        :param source: Type coming from the database table or cursor description
+        :return: ColumnSpec object
+        """
+        if not native_type:
+            return None
+        sqla_type = types.resolve_type_from_name(native_type)
+        name_u = sqla_type.__visit_name__
+        generic_type = None
+        if name_u == 'BOOLEAN':
+            generic_type = GenericDataType.BOOLEAN
+        elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
+            generic_type = GenericDataType.NUMERIC
+        elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
+            generic_type = GenericDataType.STRING
+        elif name_u in ('DATE', 'TIMESTAMP'):
+            generic_type = GenericDataType.TEMPORAL
+        elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
+            generic_type = GenericDataType.STRING
+        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
```

### Comparing `questdb-connect-0.0.73/src/questdb_connect/types.py` & `questdb-connect-0.0.74/src/questdb_connect/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,14 @@
     if not type_class:
         raise ArgumentError(f'unsupported type: {type_name}')
     return type_class
 
 
 class QDBTypeCompiler(GenericTypeCompiler):
     ensure_kwarg = None
-    def visit_BOOLEAN(self, type_, **kw):
-        return Boolean.__visit_name__
 
     def visit_GEOHASHINT(self, type_, **kw):
         return GeohashInt.__visit_name__
 
     def visit_GeohashInt(self, type_, **kw):
         return GeohashInt.__visit_name__
 
@@ -292,17 +290,14 @@
             UnsupportedCompilationError(self, element),
             replace_context=err,
         )
 
     def visit_BOOLEAN(self, type_, **kw):
         return Boolean.__visit_name__
 
-    def visit_BOOLEAN(self, type_, **kw):
-        return Boolean.__visit_name__
-
     def visit_boolean(self, type_, **kw):
         return Boolean.__visit_name__
 
     def visit_BYTE(self, type_, **kw):
         return Byte.__visit_name__
 
     def visit_byte(self, type_, **kw):
```

### Comparing `questdb-connect-0.0.73/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.74/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.73
+Version: 0.0.74
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.73/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.74/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/tests/test_dialect.py` & `questdb-connect-0.0.74/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/tests/test_superset.py` & `questdb-connect-0.0.74/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.73/tests/test_types.py` & `questdb-connect-0.0.74/tests/test_types.py`

 * *Files identical despite different names*

