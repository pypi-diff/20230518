# Comparing `tmp/questdb-connect-0.0.60.tar.gz` & `tmp/questdb-connect-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.60.tar", last modified: Wed May 17 21:36:52 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.61.tar", last modified: Wed May 17 22:27:23 2023, max compression
```

## Comparing `questdb-connect-0.0.60.tar` & `questdb-connect-0.0.61.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 21:36:52.655858 questdb-connect-0.0.60/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.60/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 21:36:52.655700 questdb-connect-0.0.60/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.60/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-17 21:33:27.000000 questdb-connect-0.0.60/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-17 21:36:52.655897 questdb-connect-0.0.60/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 21:36:52.648793 questdb-connect-0.0.60/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 21:36:52.651356 questdb-connect-0.0.60/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.60/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.60/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.60/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.60/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.60/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.60/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 21:36:52.653222 questdb-connect-0.0.60/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.60/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.60/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.60/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     7350 2023-05-17 21:35:59.000000 questdb-connect-0.0.60/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.60/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 21:36:52.654416 questdb-connect-0.0.60/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 21:36:52.000000 questdb-connect-0.0.60/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-17 21:36:52.000000 questdb-connect-0.0.60/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-17 21:36:52.000000 questdb-connect-0.0.60/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-17 21:36:52.000000 questdb-connect-0.0.60/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-17 21:36:52.000000 questdb-connect-0.0.60/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-17 21:36:52.000000 questdb-connect-0.0.60/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 21:36:52.655294 questdb-connect-0.0.60/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.60/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.60/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.60/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 22:27:23.832058 questdb-connect-0.0.61/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.61/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 22:27:23.831906 questdb-connect-0.0.61/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.61/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-17 22:26:09.000000 questdb-connect-0.0.61/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-17 22:27:23.832097 questdb-connect-0.0.61/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 22:27:23.826516 questdb-connect-0.0.61/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 22:27:23.828683 questdb-connect-0.0.61/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.61/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.61/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.61/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.61/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.61/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.61/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 22:27:23.829923 questdb-connect-0.0.61/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.61/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.61/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.61/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     7350 2023-05-17 21:35:59.000000 questdb-connect-0.0.61/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.61/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 22:27:23.830995 questdb-connect-0.0.61/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-17 22:27:23.000000 questdb-connect-0.0.61/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-17 22:27:23.000000 questdb-connect-0.0.61/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-17 22:27:23.000000 questdb-connect-0.0.61/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-17 22:27:23.000000 questdb-connect-0.0.61/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-17 22:27:23.000000 questdb-connect-0.0.61/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-17 22:27:23.000000 questdb-connect-0.0.61/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-17 22:27:23.831616 questdb-connect-0.0.61/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.61/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.61/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.61/tests/test_types.py
```

### Comparing `questdb-connect-0.0.60/LICENSE` & `questdb-connect-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/PKG-INFO` & `questdb-connect-0.0.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.60
+Version: 0.0.61
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ## QuestDB Connect
 
 This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/),
```

### Comparing `questdb-connect-0.0.60/README.md` & `questdb-connect-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/pyproject.toml` & `questdb-connect-0.0.61/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.60'
+version = '0.0.61'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = "~=3.9"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
```

### Comparing `questdb-connect-0.0.60/src/examples/__init__.py` & `questdb-connect-0.0.61/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/examples/hello_world.py` & `questdb-connect-0.0.61/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.61/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/examples/server_utilisation.py` & `questdb-connect-0.0.61/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.61/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.61/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/questdb_connect/__init__.py` & `questdb-connect-0.0.61/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/questdb_connect/dialect.py` & `questdb-connect-0.0.61/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/questdb_connect/function_names.py` & `questdb-connect-0.0.61/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.61/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/questdb_connect/types.py` & `questdb-connect-0.0.61/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.61/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.60
+Version: 0.0.61
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ## QuestDB Connect
 
 This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/),
```

### Comparing `questdb-connect-0.0.60/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.61/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/tests/test_dialect.py` & `questdb-connect-0.0.61/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/tests/test_superset.py` & `questdb-connect-0.0.61/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.60/tests/test_types.py` & `questdb-connect-0.0.61/tests/test_types.py`

 * *Files identical despite different names*

