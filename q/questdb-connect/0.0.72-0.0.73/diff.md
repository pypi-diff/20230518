# Comparing `tmp/questdb-connect-0.0.72.tar.gz` & `tmp/questdb-connect-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.72.tar", last modified: Thu May 18 11:35:02 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.73.tar", last modified: Thu May 18 15:02:43 2023, max compression
```

## Comparing `questdb-connect-0.0.72.tar` & `questdb-connect-0.0.73.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.242656 questdb-connect-0.0.72/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.72/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:35:02.242445 questdb-connect-0.0.72/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.72/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 11:34:43.000000 questdb-connect-0.0.72/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 11:35:02.242709 questdb-connect-0.0.72/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.228628 questdb-connect-0.0.72/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.235783 questdb-connect-0.0.72/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.72/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.72/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.72/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.72/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.72/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.72/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.237951 questdb-connect-0.0.72/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.72/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11398 2023-05-18 11:15:14.000000 questdb-connect-0.0.72/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.72/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    11656 2023-05-18 11:34:28.000000 questdb-connect-0.0.72/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.72/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.239273 questdb-connect-0.0.72/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.242063 questdb-connect-0.0.72/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.72/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 11:34:07.000000 questdb-connect-0.0.72/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.72/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.684349 questdb-connect-0.0.73/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.73/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:02:43.684220 questdb-connect-0.0.73/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.73/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 15:02:26.000000 questdb-connect-0.0.73/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 15:02:43.684390 questdb-connect-0.0.73/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.678477 questdb-connect-0.0.73/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.680933 questdb-connect-0.0.73/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.73/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.73/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.73/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.73/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.73/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.73/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.682350 questdb-connect-0.0.73/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.73/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11858 2023-05-18 15:00:07.000000 questdb-connect-0.0.73/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.73/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12264 2023-05-18 15:00:47.000000 questdb-connect-0.0.73/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10302 2023-05-18 15:01:46.000000 questdb-connect-0.0.73/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.683248 questdb-connect-0.0.73/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 15:02:43.000000 questdb-connect-0.0.73/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 15:02:43.683849 questdb-connect-0.0.73/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.73/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.73/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.73/tests/test_types.py
```

### Comparing `questdb-connect-0.0.72/LICENSE` & `questdb-connect-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/PKG-INFO` & `questdb-connect-0.0.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.72
+Version: 0.0.73
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.72/README.md` & `questdb-connect-0.0.73/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/pyproject.toml` & `questdb-connect-0.0.73/pyproject.toml`

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
-version = '0.0.72'
+version = '0.0.73'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.72/src/examples/__init__.py` & `questdb-connect-0.0.73/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/examples/hello_world.py` & `questdb-connect-0.0.73/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.73/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/examples/server_utilisation.py` & `questdb-connect-0.0.73/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.73/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.73/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/questdb_connect/__init__.py` & `questdb-connect-0.0.73/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/questdb_connect/dialect.py` & `questdb-connect-0.0.73/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 #  limitations under the License.
 #
 import abc
 
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
-from sqlalchemy.engine.reflection import Inspector
+from sqlalchemy.engine.reflection import Inspector, cache
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import (
     DDLCompiler,
-    GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
 )
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
 from .types import *
@@ -244,15 +243,15 @@
 
 class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
     psycopg2_version = (2, 9)
     default_schema_name = 'public'
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
-    type_compiler = GenericTypeCompiler
+    type_compiler = QDBTypeCompiler
     inspector = QDBInspector
     preparer = QDBIdentifierPreparer
     supports_schemas = False
     supports_statement_cache = False
     supports_server_side_cursors = False
     supports_native_boolean = True
     supports_views = False
@@ -328,7 +327,20 @@
         raise NotImplementedError
 
     def set_isolation_level(self, dbapi_connection, level):
         pass
 
     def get_isolation_level(self, dbapi_connection):
         return None
+
+    @cache
+    def get_columns(self, connection, table_name, schema=None, **kw):
+        query = f"table_columns('{table_name}')"
+        result_set = connection.execute(text(query))
+        if not result_set:
+            raise NoResultFound(f"Table '{table_name}' does not exist")
+        return [{
+            'name': row[0],
+            'type': resolve_type_from_name(row[1])(),
+            'nullable': True,
+            'autoincrement': False,
+        } for row in result_set]
```

### Comparing `questdb-connect-0.0.72/src/questdb_connect/function_names.py` & `questdb-connect-0.0.73/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.73/src/questdb_connect/superset_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 from flask_babel import gettext as __
 from flask_babel import lazy_gettext as _
 from marshmallow import Schema, fields
+from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
     TimeGrain,
@@ -233,14 +234,26 @@
         :return: ColumnSpec object
         """
         if not native_type:
             return None
         return types.resolve_type_from_name(native_type).impl
 
     @classmethod
+    def column_datatype_to_string(cls, sqla_column_type: TypeEngine, dialect: Dialect) -> str:
+        """Convert sqlalchemy column type to string representation.
+        By default, removes collation and character encoding info to avoid
+        unnecessarily long datatypes.
+        :param sqla_column_type: SqlAlchemy column type
+        :param dialect: Sqlalchemy dialect
+        :return: Compiled column type
+        """
+        sqla_column_type = sqla_column_type.copy()
+        return sqla_column_type.compile(dialect=dialect).upper()
+
+    @classmethod
     def select_star(
             cls,
             database,
             table_name: str,
             engine,
             schema: Optional[str] = None,
             limit: int = 100,
```

### Comparing `questdb-connect-0.0.72/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.73/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.72
+Version: 0.0.73
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.72/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.73/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/tests/test_dialect.py` & `questdb-connect-0.0.73/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/tests/test_superset.py` & `questdb-connect-0.0.73/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.72/tests/test_types.py` & `questdb-connect-0.0.73/tests/test_types.py`

 * *Files identical despite different names*

