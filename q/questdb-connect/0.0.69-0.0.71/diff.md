# Comparing `tmp/questdb-connect-0.0.69.tar.gz` & `tmp/questdb-connect-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.69.tar", last modified: Thu May 18 11:03:02 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.71.tar", last modified: Thu May 18 11:16:15 2023, max compression
```

## Comparing `questdb-connect-0.0.69.tar` & `questdb-connect-0.0.71.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:03:02.797797 questdb-connect-0.0.69/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.69/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:03:02.797654 questdb-connect-0.0.69/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.69/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 11:02:37.000000 questdb-connect-0.0.69/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 11:03:02.797837 questdb-connect-0.0.69/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:03:02.791761 questdb-connect-0.0.69/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:03:02.794242 questdb-connect-0.0.69/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.69/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.69/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.69/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.69/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.69/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.69/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:03:02.795522 questdb-connect-0.0.69/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.69/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11397 2023-05-18 06:15:23.000000 questdb-connect-0.0.69/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.69/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-18 11:02:20.000000 questdb-connect-0.0.69/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.69/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:03:02.796624 questdb-connect-0.0.69/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:03:02.000000 questdb-connect-0.0.69/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 11:03:02.000000 questdb-connect-0.0.69/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 11:03:02.000000 questdb-connect-0.0.69/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 11:03:02.000000 questdb-connect-0.0.69/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 11:03:02.000000 questdb-connect-0.0.69/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 11:03:02.000000 questdb-connect-0.0.69/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:03:02.797332 questdb-connect-0.0.69/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.69/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.69/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.69/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.182792 questdb-connect-0.0.71/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.71/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:16:15.182658 questdb-connect-0.0.71/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.71/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 11:15:52.000000 questdb-connect-0.0.71/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 11:16:15.182832 questdb-connect-0.0.71/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.177625 questdb-connect-0.0.71/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.179732 questdb-connect-0.0.71/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.71/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.71/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.71/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.71/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.71/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.71/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.180936 questdb-connect-0.0.71/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.71/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11398 2023-05-18 11:15:14.000000 questdb-connect-0.0.71/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.71/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10674 2023-05-18 11:11:54.000000 questdb-connect-0.0.71/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.71/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.181791 questdb-connect-0.0.71/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.182397 questdb-connect-0.0.71/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.71/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.71/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.71/tests/test_types.py
```

### Comparing `questdb-connect-0.0.69/LICENSE` & `questdb-connect-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/PKG-INFO` & `questdb-connect-0.0.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.69
+Version: 0.0.71
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.69/README.md` & `questdb-connect-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/pyproject.toml` & `questdb-connect-0.0.71/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.69'
+version = '0.0.71'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.69/src/examples/__init__.py` & `questdb-connect-0.0.71/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/examples/hello_world.py` & `questdb-connect-0.0.71/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.71/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/examples/server_utilisation.py` & `questdb-connect-0.0.71/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.71/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.71/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/questdb_connect/__init__.py` & `questdb-connect-0.0.71/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/questdb_connect/dialect.py` & `questdb-connect-0.0.71/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
 
 def create_engine(host: str, port: int, username: str, password: str, database: str = 'main'):
     return sqlalchemy.create_engine(
         connection_uri(host, port, username, password, database),
         future=False,
-        hide_parameters=True,
+        hide_parameters=False,
         implicit_returning=False,
-        isolation_level="REPEATABLE READ")
+        isolation_level='REPEATABLE READ')
 
 
 # ===== QUESTDB ENGINE =====
 
 class QDBTableEngine(SchemaEventTarget, Traversible):
     def __init__(
             self,
@@ -150,18 +150,18 @@
     def format_table(self, table, use_schema=True, name=None):
         """Prepare a quoted table and schema name."""
         return quote_identifier(name if name else table.name)
 
 
 class QDBDDLCompiler(DDLCompiler, abc.ABC):
     def visit_create_schema(self, create, **kw):
-        raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
+        raise Exception("QuestDB does not support SCHEMAS, there is only 'public'")
 
     def visit_drop_schema(self, drop, **kw):
-        raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
+        raise Exception("QuestDB does not support SCHEMAS, there is only 'public'")
 
     def visit_create_table(self, create, **kw):
         table = create.element
         create_table = f"CREATE TABLE {quote_identifier(table.fullname)} ("
         create_table += ', '.join([self.get_column_specification(c.element) for c in create.columns])
         return create_table + ') ' + table.engine.get_table_suffix()
```

### Comparing `questdb-connect-0.0.69/src/questdb_connect/function_names.py` & `questdb-connect-0.0.71/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.71/src/questdb_connect/superset_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
-    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
+    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname"
     parameters_schema = QDBParametersSchema()
     time_groupby_inline = True
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     try_remove_schema_from_table_name = True
     max_column_name_length = 120
     supports_dynamic_schema = False
@@ -117,15 +117,15 @@
             int(parameters.get("port")),
             parameters.get("username"),
             parameters.get("password"),
             parameters.get("database"))
 
     @classmethod
     def get_default_schema_for_query(cls, database, query) -> Optional[str]:
-        return None
+        return ['public']
 
     @classmethod
     def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
         return False
 
     @classmethod
     def get_view_names(cls, database, inspector, schema: Optional[str]):
```

### Comparing `questdb-connect-0.0.69/src/questdb_connect/types.py` & `questdb-connect-0.0.71/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.71/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.69
+Version: 0.0.71
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.69/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.71/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/tests/test_dialect.py` & `questdb-connect-0.0.71/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/tests/test_superset.py` & `questdb-connect-0.0.71/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.69/tests/test_types.py` & `questdb-connect-0.0.71/tests/test_types.py`

 * *Files identical despite different names*

