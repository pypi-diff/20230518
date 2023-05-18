# Comparing `tmp/py-bigquery-mock-0.2.3.tar.gz` & `tmp/py-bigquery-mock-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bigquery-mock-0.2.3.tar", last modified: Thu May 18 19:54:37 2023, max compression
+gzip compressed data, was "py-bigquery-mock-0.2.4.tar", last modified: Thu May 18 20:41:27 2023, max compression
```

## Comparing `py-bigquery-mock-0.2.3.tar` & `py-bigquery-mock-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.371737 py-bigquery-mock-0.2.3/
--rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.3/LICENSE
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-18 19:54:37.371531 py-bigquery-mock-0.2.3/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      464 2023-05-16 19:55:28.000000 py-bigquery-mock-0.2.3/README.md
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.370005 py-bigquery-mock-0.2.3/data_mock/
--rw-r--r--   0 phtremblay (2028354092) 932231305      226 2023-05-18 18:28:45.000000 py-bigquery-mock-0.2.3/data_mock/__init__.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.369218 py-bigquery-mock-0.2.3/data_mock/google/
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.370603 py-bigquery-mock-0.2.3/data_mock/google/cloud/
--rw-r--r--   0 phtremblay (2028354092) 932231305        2 2023-05-18 18:58:16.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     1590 2023-05-18 19:47:52.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/client.py
--rw-r--r--   0 phtremblay (2028354092) 932231305       39 2023-05-18 18:28:00.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/exceptions.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      169 2023-05-18 18:28:18.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/schema.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     1662 2023-05-18 19:08:48.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/table.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.370718 py-bigquery-mock-0.2.3/data_mock/scripts/
--rw-r--r--   0 phtremblay (2028354092) 932231305     1856 2023-05-18 19:26:25.000000 py-bigquery-mock-0.2.3/data_mock/scripts/mkmock.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.371233 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      421 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/SOURCES.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/dependency_links.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       24 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/top_level.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-18 19:54:37.371781 py-bigquery-mock-0.2.3/setup.cfg
--rw-r--r--   0 phtremblay (2028354092) 932231305      463 2023-05-18 19:28:28.000000 py-bigquery-mock-0.2.3/setup.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.371353 py-bigquery-mock-0.2.3/tests/
--rw-r--r--   0 phtremblay (2028354092) 932231305     1167 2023-05-18 19:43:05.000000 py-bigquery-mock-0.2.3/tests/test1.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.713497 py-bigquery-mock-0.2.4/
+-rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.4/LICENSE
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-18 20:41:27.713309 py-bigquery-mock-0.2.4/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305     2027 2023-05-18 20:37:26.000000 py-bigquery-mock-0.2.4/README.md
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.711011 py-bigquery-mock-0.2.4/data_mock/
+-rw-r--r--   0 phtremblay (2028354092) 932231305       53 2023-05-18 20:12:32.000000 py-bigquery-mock-0.2.4/data_mock/__init__.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.709679 py-bigquery-mock-0.2.4/data_mock/google/
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.712036 py-bigquery-mock-0.2.4/data_mock/google/cloud/
+-rw-r--r--   0 phtremblay (2028354092) 932231305        2 2023-05-18 18:58:16.000000 py-bigquery-mock-0.2.4/data_mock/google/cloud/__init__.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1625 2023-05-18 20:07:36.000000 py-bigquery-mock-0.2.4/data_mock/google/cloud/client.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305       39 2023-05-18 18:28:00.000000 py-bigquery-mock-0.2.4/data_mock/google/cloud/exceptions.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305      169 2023-05-18 18:28:18.000000 py-bigquery-mock-0.2.4/data_mock/google/cloud/schema.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1662 2023-05-18 19:08:48.000000 py-bigquery-mock-0.2.4/data_mock/google/cloud/table.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.712265 py-bigquery-mock-0.2.4/data_mock/scripts/
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1856 2023-05-18 19:26:25.000000 py-bigquery-mock-0.2.4/data_mock/scripts/mkmock.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.712905 py-bigquery-mock-0.2.4/py_bigquery_mock.egg-info/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-18 20:41:27.000000 py-bigquery-mock-0.2.4/py_bigquery_mock.egg-info/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      421 2023-05-18 20:41:27.000000 py-bigquery-mock-0.2.4/py_bigquery_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-18 20:41:27.000000 py-bigquery-mock-0.2.4/py_bigquery_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       24 2023-05-18 20:41:27.000000 py-bigquery-mock-0.2.4/py_bigquery_mock.egg-info/top_level.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-18 20:41:27.713538 py-bigquery-mock-0.2.4/setup.cfg
+-rw-r--r--   0 phtremblay (2028354092) 932231305      463 2023-05-18 20:12:11.000000 py-bigquery-mock-0.2.4/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 20:41:27.713022 py-bigquery-mock-0.2.4/tests/
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1167 2023-05-18 19:43:05.000000 py-bigquery-mock-0.2.4/tests/test1.py
```

### Comparing `py-bigquery-mock-0.2.3/LICENSE` & `py-bigquery-mock-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.2.3/data_mock/google/cloud/client.py` & `py-bigquery-mock-0.2.4/data_mock/google/cloud/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from . import exceptions
 from .  import table
 
 class Client:
 
-    def __init__(self, project = None, data = [], *args, **kwargs):
-        self._test_valid_data(data)
-        self.__data = data
+    def __init__(self, project = None, mock_data = [], *args, **kwargs):
+        self._test_valid_data(mock_data)
+        self.__data = mock_data
         self.project = project
         self.__registered_data = {}
 
-    def register_data(self, key, data):
-        self._test_valid_data(data)
-        self.__registered_data[key] = data
+    def register_mock_data(self, key, mock_data):
+        self._test_valid_data(mock_data)
+        self.__registered_data[key] = mock_data
 
     def query(self, query, *args, **kwargs):
         key = self._get_sql_key(query)
         if key:
             data = self.__registered_data.get(key)
             if not data:
                 raise exceptions.InvalidData(f'{key} not found in registered_data')
```

### Comparing `py-bigquery-mock-0.2.3/data_mock/google/cloud/table.py` & `py-bigquery-mock-0.2.4/data_mock/google/cloud/table.py`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.2.3/data_mock/scripts/mkmock.py` & `py-bigquery-mock-0.2.4/data_mock/scripts/mkmock.py`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.2.3/tests/test1.py` & `py-bigquery-mock-0.2.4/tests/test1.py`

 * *Files identical despite different names*

