# Comparing `tmp/questdb-connect-0.0.65.tar.gz` & `tmp/questdb-connect-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.65.tar", last modified: Thu May 18 06:15:52 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.66.tar", last modified: Thu May 18 09:51:51 2023, max compression
```

## Comparing `questdb-connect-0.0.65.tar` & `questdb-connect-0.0.66.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 06:15:52.854897 questdb-connect-0.0.65/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.65/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 06:15:52.854758 questdb-connect-0.0.65/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.65/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-18 06:15:23.000000 questdb-connect-0.0.65/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 06:15:52.854945 questdb-connect-0.0.65/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 06:15:52.849953 questdb-connect-0.0.65/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 06:15:52.852087 questdb-connect-0.0.65/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.65/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.65/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.65/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.65/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.65/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.65/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 06:15:52.853148 questdb-connect-0.0.65/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.65/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11397 2023-05-18 06:15:23.000000 questdb-connect-0.0.65/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.65/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12079 2023-05-17 22:58:38.000000 questdb-connect-0.0.65/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.65/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 06:15:52.854009 questdb-connect-0.0.65/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 06:15:52.000000 questdb-connect-0.0.65/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 06:15:52.000000 questdb-connect-0.0.65/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 06:15:52.000000 questdb-connect-0.0.65/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-18 06:15:52.000000 questdb-connect-0.0.65/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 06:15:52.000000 questdb-connect-0.0.65/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 06:15:52.000000 questdb-connect-0.0.65/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 06:15:52.854479 questdb-connect-0.0.65/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.65/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.65/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.65/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.076333 questdb-connect-0.0.66/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.66/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 09:51:51.076155 questdb-connect-0.0.66/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.66/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-18 09:51:33.000000 questdb-connect-0.0.66/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-18 09:51:51.076379 questdb-connect-0.0.66/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.069764 questdb-connect-0.0.66/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.072960 questdb-connect-0.0.66/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.66/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.66/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.66/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.66/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.66/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.66/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.074165 questdb-connect-0.0.66/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.66/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11397 2023-05-18 06:15:23.000000 questdb-connect-0.0.66/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.66/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12079 2023-05-17 22:58:38.000000 questdb-connect-0.0.66/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.66/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.075135 questdb-connect-0.0.66/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-18 09:51:51.000000 questdb-connect-0.0.66/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-18 09:51:51.075805 questdb-connect-0.0.66/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-17 23:13:32.000000 questdb-connect-0.0.66/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.66/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.66/tests/test_types.py
```

### Comparing `questdb-connect-0.0.65/LICENSE` & `questdb-connect-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/PKG-INFO` & `questdb-connect-0.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.65
+Version: 0.0.66
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.65/README.md` & `questdb-connect-0.0.66/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/pyproject.toml` & `questdb-connect-0.0.66/pyproject.toml`

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
-version = '0.0.65'
+version = '0.0.66'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -42,15 +42,15 @@
 'Homepage' = "https://github.com/questdb/questdb-connect/"
 'Bug Tracker' = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
 questdb = 'questdb_connect.dialect:QuestDBDialect'
 
 [project.entry-points.'superset.db_engine_specs']
-questdb = 'questdb_connect.superset:QDBEngineSpec'
+questdb = 'questdb_connect.superset_engine:QDBEngineSpec'
 
 [project.optional-dependencies]
 test = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
```

### Comparing `questdb-connect-0.0.65/src/examples/__init__.py` & `questdb-connect-0.0.66/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/examples/hello_world.py` & `questdb-connect-0.0.66/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.66/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/examples/server_utilisation.py` & `questdb-connect-0.0.66/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.66/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.66/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/questdb_connect/__init__.py` & `questdb-connect-0.0.66/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/questdb_connect/dialect.py` & `questdb-connect-0.0.66/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/questdb_connect/function_names.py` & `questdb-connect-0.0.66/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.66/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/questdb_connect/types.py` & `questdb-connect-0.0.66/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.66/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.65
+Version: 0.0.66
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.65/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.66/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/tests/test_dialect.py` & `questdb-connect-0.0.66/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/tests/test_superset.py` & `questdb-connect-0.0.66/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.65/tests/test_types.py` & `questdb-connect-0.0.66/tests/test_types.py`

 * *Files identical despite different names*

