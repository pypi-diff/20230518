# Comparing `tmp/py-bigquery-mock-0.2.2.tar.gz` & `tmp/py-bigquery-mock-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bigquery-mock-0.2.2.tar", last modified: Wed May 17 21:33:56 2023, max compression
+gzip compressed data, was "py-bigquery-mock-0.2.3.tar", last modified: Thu May 18 19:54:37 2023, max compression
```

## Comparing `py-bigquery-mock-0.2.2.tar` & `py-bigquery-mock-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.226072 py-bigquery-mock-0.2.2/
--rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.2/LICENSE
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-17 21:33:56.225896 py-bigquery-mock-0.2.2/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      464 2023-05-16 19:55:28.000000 py-bigquery-mock-0.2.2/README.md
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.225156 py-bigquery-mock-0.2.2/bigquery_mock/
--rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-17 20:43:14.000000 py-bigquery-mock-0.2.2/bigquery_mock/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     3195 2023-05-16 20:40:11.000000 py-bigquery-mock-0.2.2/bigquery_mock/bigquery_mock.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.225276 py-bigquery-mock-0.2.2/bigquery_mock/scripts/
--rw-r--r--   0 phtremblay (2028354092) 932231305     1856 2023-05-17 20:17:35.000000 py-bigquery-mock-0.2.2/bigquery_mock/scripts/mkmock.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-17 21:33:56.225750 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      275 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/SOURCES.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/dependency_links.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-17 21:33:56.000000 py-bigquery-mock-0.2.2/py_bigquery_mock.egg-info/top_level.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-17 21:33:56.226112 py-bigquery-mock-0.2.2/setup.cfg
--rw-r--r--   0 phtremblay (2028354092) 932231305      456 2023-05-17 20:45:23.000000 py-bigquery-mock-0.2.2/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.371737 py-bigquery-mock-0.2.3/
+-rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.2.3/LICENSE
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-18 19:54:37.371531 py-bigquery-mock-0.2.3/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      464 2023-05-16 19:55:28.000000 py-bigquery-mock-0.2.3/README.md
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.370005 py-bigquery-mock-0.2.3/data_mock/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      226 2023-05-18 18:28:45.000000 py-bigquery-mock-0.2.3/data_mock/__init__.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.369218 py-bigquery-mock-0.2.3/data_mock/google/
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.370603 py-bigquery-mock-0.2.3/data_mock/google/cloud/
+-rw-r--r--   0 phtremblay (2028354092) 932231305        2 2023-05-18 18:58:16.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/__init__.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1590 2023-05-18 19:47:52.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/client.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305       39 2023-05-18 18:28:00.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/exceptions.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305      169 2023-05-18 18:28:18.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/schema.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1662 2023-05-18 19:08:48.000000 py-bigquery-mock-0.2.3/data_mock/google/cloud/table.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.370718 py-bigquery-mock-0.2.3/data_mock/scripts/
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1856 2023-05-18 19:26:25.000000 py-bigquery-mock-0.2.3/data_mock/scripts/mkmock.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.371233 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      421 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       24 2023-05-18 19:54:37.000000 py-bigquery-mock-0.2.3/py_bigquery_mock.egg-info/top_level.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-18 19:54:37.371781 py-bigquery-mock-0.2.3/setup.cfg
+-rw-r--r--   0 phtremblay (2028354092) 932231305      463 2023-05-18 19:28:28.000000 py-bigquery-mock-0.2.3/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-18 19:54:37.371353 py-bigquery-mock-0.2.3/tests/
+-rw-r--r--   0 phtremblay (2028354092) 932231305     1167 2023-05-18 19:43:05.000000 py-bigquery-mock-0.2.3/tests/test1.py
```

### Comparing `py-bigquery-mock-0.2.2/LICENSE` & `py-bigquery-mock-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.2.2/bigquery_mock/scripts/mkmock.py` & `py-bigquery-mock-0.2.3/data_mock/scripts/mkmock.py`

 * *Files identical despite different names*

