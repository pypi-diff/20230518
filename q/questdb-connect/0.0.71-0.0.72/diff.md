# Comparing `tmp/questdb-connect-0.0.71.tar.gz` & `tmp/questdb-connect-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.71.tar", last modified: Thu May 18 11:16:15 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.72.tar", last modified: Thu May 18 11:35:02 2023, max compression
```

## Comparing `questdb-connect-0.0.71.tar` & `questdb-connect-0.0.72.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.182792 questdb-connect-0.0.71/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.71/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:16:15.182658 questdb-connect-0.0.71/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.71/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 11:15:52.000000 questdb-connect-0.0.71/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 11:16:15.182832 questdb-connect-0.0.71/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.177625 questdb-connect-0.0.71/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.179732 questdb-connect-0.0.71/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.71/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.71/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.71/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.71/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.71/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.71/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.180936 questdb-connect-0.0.71/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.71/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11398 2023-05-18 11:15:14.000000 questdb-connect-0.0.71/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.71/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10674 2023-05-18 11:11:54.000000 questdb-connect-0.0.71/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.71/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.181791 questdb-connect-0.0.71/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 11:16:15.000000 questdb-connect-0.0.71/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:16:15.182397 questdb-connect-0.0.71/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.71/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.71/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.71/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.242656 questdb-connect-0.0.72/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.72/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:35:02.242445 questdb-connect-0.0.72/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.72/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 11:34:43.000000 questdb-connect-0.0.72/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 11:35:02.242709 questdb-connect-0.0.72/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.228628 questdb-connect-0.0.72/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.235783 questdb-connect-0.0.72/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.72/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.72/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.72/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.72/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.72/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.72/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.237951 questdb-connect-0.0.72/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.72/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11398 2023-05-18 11:15:14.000000 questdb-connect-0.0.72/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.72/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11656 2023-05-18 11:34:28.000000 questdb-connect-0.0.72/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.72/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.239273 questdb-connect-0.0.72/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 11:35:02.000000 questdb-connect-0.0.72/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 11:35:02.242063 questdb-connect-0.0.72/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.72/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 11:34:07.000000 questdb-connect-0.0.72/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.72/tests/test_types.py
```

### Comparing `questdb-connect-0.0.71/LICENSE` & `questdb-connect-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/PKG-INFO` & `questdb-connect-0.0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.71
+Version: 0.0.72
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.71/README.md` & `questdb-connect-0.0.72/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/pyproject.toml` & `questdb-connect-0.0.72/pyproject.toml`

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
-version = '0.0.71'
+version = '0.0.72'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.71/src/examples/__init__.py` & `questdb-connect-0.0.72/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/examples/hello_world.py` & `questdb-connect-0.0.72/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.72/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/examples/server_utilisation.py` & `questdb-connect-0.0.72/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.72/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.72/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/questdb_connect/__init__.py` & `questdb-connect-0.0.72/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/questdb_connect/dialect.py` & `questdb-connect-0.0.72/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/questdb_connect/function_names.py` & `questdb-connect-0.0.72/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.72/src/questdb_connect/superset_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,24 @@
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 from flask_babel import gettext as __
+from flask_babel import lazy_gettext as _
 from marshmallow import Schema, fields
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
+    TimeGrain,
+    builtin_time_grains,
 )
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 from . import remove_public_schema, types
 from .dialect import connection_uri
 from .function_names import FUNCTION_NAMES
@@ -83,14 +86,20 @@
         "PT6H": "date_trunc('hour', {col}) + 21600000000L",
         "PT1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P3M": "date_trunc('quarter', {col})",
     }
+    ret_list = []
+    for duration, func in _time_grain_expressions.items():
+        if duration in builtin_time_grains:
+            name = builtin_time_grains[duration]
+            ret_list.append(TimeGrain(name, _(name), func, duration))
+    _engine_time_grains = tuple(ret_list)
     _default_column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
         (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
         (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
         (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
@@ -138,14 +147,23 @@
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
         return text(remove_public_schema(clause))
 
     @classmethod
+    def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
+        """Return a dict of all supported time grains including any
+        potential added grains but excluding any potentially disabled
+        grains in the config file.
+        :return: All time grain expressions supported by the engine
+        """
+        return cls._time_grain_expressions
+
+    @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used in a
         query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
         return '{col} * 1000000'
@@ -170,14 +188,21 @@
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
         return type_code.upper() if type_code and isinstance(type_code, str) else str(type_code)
 
     @classmethod
+    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
+        """Generate a tuple of supported time grains.
+        :return: All time grains supported by the engine
+        """
+        return cls._engine_time_grains
+
+    @classmethod
     def get_column_types(
             cls,
             column_type: Optional[str],
     ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
         """Return a sqlalchemy native column type and generic data type that
         corresponds to the column type defined in the data source (return None
         to use default type inferred by SQLAlchemy). Override `column_type_mappings`
```

### Comparing `questdb-connect-0.0.71/src/questdb_connect/types.py` & `questdb-connect-0.0.72/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.72/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.71
+Version: 0.0.72
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.71/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.72/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/tests/test_dialect.py` & `questdb-connect-0.0.72/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.71/tests/test_superset.py` & `questdb-connect-0.0.72/tests/test_superset.py`

 * *Files 24% similar despite different names*

```diff
@@ -86,7 +86,32 @@
     assert pg_result == {'table', '"public.table_3"', 'table_2'}
 
 
 def test_time_exp_literal_no_grain():
     col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
     expr = QDBEngineSpec.get_timestamp_expr(col, None, None)
     assert str(expr.compile(None, dialect=QuestDBDialect())) == 'col_ts'
+
+
+def test_time_exp_literal_1y_grain():
+    col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
+    expr = QDBEngineSpec.get_timestamp_expr(col, None, 'P1Y')
+    assert str(expr.compile(None, dialect=QuestDBDialect())) == "date_trunc('year', col_ts)"
+
+
+def test_time_exp_highr():
+    col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
+    expr = QDBEngineSpec.get_timestamp_expr(col, 'epoch_ms', None)
+    assert str(expr.compile(None, dialect=QuestDBDialect())) == '(col_ts/1000) * 1000000'
+
+
+def test_time_exp_lowr_col_sec_1y():
+    col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
+    expr = QDBEngineSpec.get_timestamp_expr(col, "epoch_s", "P1Y")
+    assert str(expr.compile(None, dialect=QuestDBDialect())) == "date_trunc('year', col_ts * 1000000)"
+
+
+def test_time_exp_highr_col_micro_1y():
+    col = sqla.Column('col_ts', types.Timestamp, primary_key=True)
+    expr = QDBEngineSpec.get_timestamp_expr(col, "epoch_ms", "P1Y")
+    assert str(expr.compile(None, dialect=QuestDBDialect())) == "date_trunc('year', (col_ts/1000) * 1000000)"
+
```

### Comparing `questdb-connect-0.0.71/tests/test_types.py` & `questdb-connect-0.0.72/tests/test_types.py`

 * *Files identical despite different names*

