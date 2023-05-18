# Comparing `tmp/questdb-connect-0.0.66.tar.gz` & `tmp/questdb-connect-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.66.tar", last modified: Thu May 18 09:51:51 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.67.tar", last modified: Thu May 18 10:17:06 2023, max compression
```

## Comparing `questdb-connect-0.0.66.tar` & `questdb-connect-0.0.67.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.076333 questdb-connect-0.0.66/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.66/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 09:51:51.076155 questdb-connect-0.0.66/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.66/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 09:51:33.000000 questdb-connect-0.0.66/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 09:51:51.076379 questdb-connect-0.0.66/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.069764 questdb-connect-0.0.66/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.072960 questdb-connect-0.0.66/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.66/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.66/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.66/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.66/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.66/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.66/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.074165 questdb-connect-0.0.66/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.66/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11397 2023-05-18 06:15:23.000000 questdb-connect-0.0.66/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.66/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12079 2023-05-17 22:58:38.000000 questdb-connect-0.0.66/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.66/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.075135 questdb-connect-0.0.66/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.075805 questdb-connect-0.0.66/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.66/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.66/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.66/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 10:17:06.828667 questdb-connect-0.0.67/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.67/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 10:17:06.828511 questdb-connect-0.0.67/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.67/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 10:16:12.000000 questdb-connect-0.0.67/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 10:17:06.828712 questdb-connect-0.0.67/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 10:17:06.820414 questdb-connect-0.0.67/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 10:17:06.823704 questdb-connect-0.0.67/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.67/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.67/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.67/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.67/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.67/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.67/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 10:17:06.825661 questdb-connect-0.0.67/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.67/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11397 2023-05-18 06:15:23.000000 questdb-connect-0.0.67/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.67/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7770 2023-05-18 10:16:12.000000 questdb-connect-0.0.67/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.67/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 10:17:06.827128 questdb-connect-0.0.67/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 10:17:06.000000 questdb-connect-0.0.67/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 10:17:06.000000 questdb-connect-0.0.67/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 10:17:06.000000 questdb-connect-0.0.67/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 10:17:06.000000 questdb-connect-0.0.67/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 10:17:06.000000 questdb-connect-0.0.67/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 10:17:06.000000 questdb-connect-0.0.67/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 10:17:06.828076 questdb-connect-0.0.67/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.67/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.67/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.67/tests/test_types.py
```

### Comparing `questdb-connect-0.0.66/LICENSE` & `questdb-connect-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/PKG-INFO` & `questdb-connect-0.0.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.66
+Version: 0.0.67
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.66/README.md` & `questdb-connect-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/pyproject.toml` & `questdb-connect-0.0.67/pyproject.toml`

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
-version = '0.0.66'
+version = '0.0.67'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.66/src/examples/__init__.py` & `questdb-connect-0.0.67/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/examples/hello_world.py` & `questdb-connect-0.0.67/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.67/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/examples/server_utilisation.py` & `questdb-connect-0.0.67/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.67/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.67/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/questdb_connect/__init__.py` & `questdb-connect-0.0.67/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/questdb_connect/dialect.py` & `questdb-connect-0.0.67/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/questdb_connect/function_names.py` & `questdb-connect-0.0.67/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.67/src/questdb_connect/superset_engine.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,26 +18,24 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 from flask_babel import gettext as __
 from marshmallow import Schema, fields
 from sqlalchemy.sql import text
-from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
 )
-from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 from . import remove_public_schema, types
 from .dialect import connection_uri
 from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
@@ -83,15 +81,15 @@
         "PT6H": "date_trunc('hour', {col}) + 21600000000L",
         "PT1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P3M": "date_trunc('quarter', {col})",
     }
-    _default_column_type_mappings = (
+    column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
         (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
         (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
         (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
         (re.compile("^FLOAT", re.IGNORECASE), types.Float, GenericDataType.NUMERIC),
@@ -100,15 +98,14 @@
         (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
         (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
         (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
         (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
         (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
         (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING)
     )
-    column_type_mappings = _default_column_type_mappings
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
@@ -169,108 +166,14 @@
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
         return type_code.upper() if type_code and isinstance(type_code, str) else str(type_code)
 
-    @classmethod
-    def get_column_types(
-            cls,
-            column_type: Optional[str],
-    ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
-        """Return a sqlalchemy native column type and generic data type that
-        corresponds to the column type defined in the data source (return None
-        to use default type inferred by SQLAlchemy). Override `column_type_mappings`
-        for specific needs (see MSSQL for example of NCHAR/NVARCHAR handling).
-        :param column_type: Column type returned by inspector
-        :return: SQLAlchemy and generic Superset column types
-        """
-        if not column_type:
-            return None
-        for regex, sqla_type, generic_type in cls._default_column_type_mappings:
-            matching_name = regex.search(column_type)
-            if matching_name:
-                qdbcd_type = types.resolve_type_from_name(sqla_type.__visit_name__)
-                return qdbcd_type.impl, generic_type
-        return None
-
-    @classmethod
-    def get_sqla_column_type(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
-    ) -> Optional[TypeEngine]:
-        """Converts native database type to sqlalchemy column type.
-        :param native_type: Native database type
-        :param db_extra: The database extra object
-        :param source: Type coming from the database table or cursor description
-        :return: ColumnSpec object
-        """
-        if not native_type:
-            return None
-        return types.resolve_type_from_name(native_type).impl
-
-    @classmethod
-    def get_column_spec(
-            cls,
-            native_type: Optional[str],
-            db_extra: Optional[Dict[str, Any]] = None,
-            source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
-    ) -> Optional[utils.ColumnSpec]:
-        """Get generic type related specs regarding a native column type.
-        :param native_type: Native database type
-        :param db_extra: The database extra object
-        :param source: Type coming from the database table or cursor description
-        :return: ColumnSpec object
-        """
-        if not native_type:
-            return None
-        sqla_type = types.resolve_type_from_name(native_type)
-        name_u = sqla_type.__visit_name__
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
-            generic_type = GenericDataType.STRING
-        return utils.ColumnSpec(sqla_type.impl, generic_type, generic_type == GenericDataType.TEMPORAL)
-
-    @classmethod
-    def select_star(
-            cls,
-            database,
-            table_name: str,
-            engine,
-            schema: Optional[str] = None,
-            limit: int = 100,
-            show_cols: bool = False,
-            indent: bool = True,
-            latest_partition: bool = True,
-            cols: Optional[List[Dict[str, Any]]] = None,
-    ) -> str:
-        """Generate a "SELECT * from table_name" query with appropriate limit.
-        :param database: Database instance
-        :param table_name: Table name, unquoted
-        :param engine: SqlAlchemy Engine instance
-        :param schema: Schema, unquoted
-        :param limit: limit to impose on query
-        :param show_cols: Show columns in query; otherwise use "*"
-        :param indent: Add indentation to query
-        :param latest_partition: Only query the latest partition
-        :param cols: Columns to include in query
-        :return: SQL query
-        """
-        return super().select_star(database, table_name, engine, None, limit, show_cols, indent, latest_partition, cols)
 
     @classmethod
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
```

### Comparing `questdb-connect-0.0.66/src/questdb_connect/types.py` & `questdb-connect-0.0.67/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.67/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.66
+Version: 0.0.67
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.66/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.67/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/tests/test_dialect.py` & `questdb-connect-0.0.67/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/tests/test_superset.py` & `questdb-connect-0.0.67/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.66/tests/test_types.py` & `questdb-connect-0.0.67/tests/test_types.py`

 * *Files identical despite different names*

