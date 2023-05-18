# Comparing `tmp/questdb-connect-0.0.74.tar.gz` & `tmp/questdb-connect-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.74.tar", last modified: Thu May 18 15:18:54 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.75.tar", last modified: Thu May 18 17:22:11 2023, max compression
```

## Comparing `questdb-connect-0.0.74.tar` & `questdb-connect-0.0.75.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.146063 questdb-connect-0.0.74/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.74/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:18:54.145902 questdb-connect-0.0.74/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.74/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 15:17:05.000000 questdb-connect-0.0.74/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 15:18:54.146109 questdb-connect-0.0.74/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.138987 questdb-connect-0.0.74/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.141593 questdb-connect-0.0.74/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.74/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.74/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.74/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.74/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.74/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.74/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.143295 questdb-connect-0.0.74/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.74/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11858 2023-05-18 15:00:07.000000 questdb-connect-0.0.74/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.74/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    13668 2023-05-18 15:17:05.000000 questdb-connect-0.0.74/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)    10141 2023-05-18 15:17:11.000000 questdb-connect-0.0.74/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.144306 questdb-connect-0.0.74/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 15:18:54.000000 questdb-connect-0.0.74/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:18:54.145437 questdb-connect-0.0.74/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.74/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.74/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.74/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 17:22:11.721315 questdb-connect-0.0.75/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.75/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 17:22:11.721183 questdb-connect-0.0.75/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.75/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 17:21:58.000000 questdb-connect-0.0.75/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 17:22:11.721354 questdb-connect-0.0.75/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 17:22:11.714321 questdb-connect-0.0.75/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 17:22:11.716932 questdb-connect-0.0.75/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.75/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.75/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.75/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.75/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.75/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.75/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 17:22:11.718712 questdb-connect-0.0.75/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.75/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11889 2023-05-18 17:11:31.000000 questdb-connect-0.0.75/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.75/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13686 2023-05-18 17:21:58.000000 questdb-connect-0.0.75/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     8455 2023-05-18 17:16:43.000000 questdb-connect-0.0.75/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 17:22:11.719877 questdb-connect-0.0.75/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 17:22:11.000000 questdb-connect-0.0.75/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 17:22:11.000000 questdb-connect-0.0.75/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 17:22:11.000000 questdb-connect-0.0.75/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 17:22:11.000000 questdb-connect-0.0.75/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 17:22:11.000000 questdb-connect-0.0.75/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 17:22:11.000000 questdb-connect-0.0.75/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 17:22:11.720784 questdb-connect-0.0.75/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.75/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.75/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.75/tests/test_types.py
```

### Comparing `questdb-connect-0.0.74/LICENSE` & `questdb-connect-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/PKG-INFO` & `questdb-connect-0.0.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.74
+Version: 0.0.75
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.74/README.md` & `questdb-connect-0.0.75/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/pyproject.toml` & `questdb-connect-0.0.75/pyproject.toml`

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
-version = '0.0.74'
+version = '0.0.75'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.74/src/examples/__init__.py` & `questdb-connect-0.0.75/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/examples/hello_world.py` & `questdb-connect-0.0.75/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.75/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/examples/server_utilisation.py` & `questdb-connect-0.0.75/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.75/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.75/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/questdb_connect/__init__.py` & `questdb-connect-0.0.75/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/questdb_connect/dialect.py` & `questdb-connect-0.0.75/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
-
+import logging
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector, cache
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import (
@@ -34,14 +34,17 @@
     SQLCompiler,
 )
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
 from .types import *
 
+logger = logging.getLogger(__name__)
+
+
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
@@ -140,15 +143,15 @@
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
         return _value and _has_special_char(_value)
 
     def format_schema(self, name):
         """Prepare a quoted schema name."""
-        return ""
+        return ''
 
     def format_table(self, table, use_schema=True, name=None):
         """Prepare a quoted table and schema name."""
         return quote_identifier(name if name else table.name)
 
 
 class QDBDDLCompiler(DDLCompiler, abc.ABC):
@@ -330,16 +333,15 @@
         pass
 
     def get_isolation_level(self, dbapi_connection):
         return None
 
     @cache
     def get_columns(self, connection, table_name, schema=None, **kw):
-        query = f"table_columns('{table_name}')"
-        result_set = connection.execute(text(query))
+        result_set = connection.execute(text(f"table_columns('{table_name}')"))
         if not result_set:
             raise NoResultFound(f"Table '{table_name}' does not exist")
         return [{
             'name': row[0],
             'type': resolve_type_from_name(row[1])(),
             'nullable': True,
             'autoincrement': False,
```

### Comparing `questdb-connect-0.0.74/src/questdb_connect/function_names.py` & `questdb-connect-0.0.75/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.75/src/questdb_connect/superset_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,23 +137,23 @@
     def get_allow_cost_estimate(cls, extra: Dict[str, Any]) -> bool:
         return False
 
     @classmethod
     def get_view_names(cls, database, inspector, schema: Optional[str]):
         return []
 
-    @classmethod
-    def get_text_clause(cls, clause):
-        """SQLAlchemy wrapper to ensure text clauses are escaped properly
-        :param clause: string clause with potentially unescaped characters
-        :return: text clause with escaped characters
-        """
-        if cls.allows_escaped_colons:
-            clause = clause.replace(":", "\\:")
-        return text(remove_public_schema(clause))
+    # @classmethod
+    # def get_text_clause(cls, clause):
+    #     """SQLAlchemy wrapper to ensure text clauses are escaped properly
+    #     :param clause: string clause with potentially unescaped characters
+    #     :return: text clause with escaped characters
+    #     """
+    #     if cls.allows_escaped_colons:
+    #         clause = clause.replace(":", "\\:")
+    #     return text(remove_public_schema(clause))
 
     @classmethod
     def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
         """Return a dict of all supported time grains including any
         potential added grains but excluding any potentially disabled
         grains in the config file.
         :return: All time grain expressions supported by the engine
```

### Comparing `questdb-connect-0.0.74/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.75/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.74
+Version: 0.0.75
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.74/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.75/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/tests/test_dialect.py` & `questdb-connect-0.0.75/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/tests/test_superset.py` & `questdb-connect-0.0.75/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.74/tests/test_types.py` & `questdb-connect-0.0.75/tests/test_types.py`

 * *Files identical despite different names*

