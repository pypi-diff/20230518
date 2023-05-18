# Comparing `tmp/gridstatusio-0.2.1.tar.gz` & `tmp/gridstatusio-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-e08qpimp/gridstatusio-0.2.1.tar", last modified: Mon May  8 23:29:44 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-1gjkv42a/gridstatusio-0.2.2.tar", last modified: Thu May 18 00:13:59 2023, max compression
```

## Comparing `gridstatusio-0.2.1.tar` & `gridstatusio-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8292 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/gs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3258 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2319 2023-05-08 23:29:30.000000 gridstatusio-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 23:29:44.000000 gridstatusio-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8550 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-05-18 00:13:45.000000 gridstatusio-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 00:13:59.000000 gridstatusio-0.2.2/setup.cfg
```

### Comparing `gridstatusio-0.2.1/LICENSE` & `gridstatusio-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.1/PKG-INFO` & `gridstatusio-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.2.1/README.md` & `gridstatusio-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.1/gridstatusio/gs_client.py` & `gridstatusio-0.2.2/gridstatusio/gs_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,42 +134,48 @@
 
         if return_list:
             return matched_datasets
 
     def get_dataset(
         self,
         dataset,
-        start,
-        end,
+        start=None,
+        end=None,
         filter_column=None,
         filter_value=None,
         limit=10000,
         tz=None,
         verbose=False,
     ):
         """Get a dataset from GridStatus.io API
 
         Parameters:
             dataset (str): The name of the dataset to fetch
-            start (str): The start time of the data to fetch
-            end (str): The end time of the data to fetch
+            start (str): The start time of the data to fetch. If not provided,
+                defaults to the earliest available time for the dataset.
+            end (str): The end time of the data to fetch. If not provided,
+                defaults to the latest available time for the dataset.
             filter_column (str): The column to filter on
             filter_value (str): The value to filter on
             limit (int): The maximum number of rows to fetch at time.
             tz (str): The timezone to convert utc timestamps to. Defaults to UTC.
             verbose (bool): If set to True, prints out the number
                 of rows fetched and the time taken to fetch them.
 
         Returns:
             pd.DataFrame: The dataset as a pandas dataframe
         """
         if tz is None:
             tz = "UTC"
-        start = gridstatus.utils._handle_date(start, tz)
-        end = gridstatus.utils._handle_date(end, tz)
+
+        if start is not None:
+            start = gridstatus.utils._handle_date(start, tz)
+
+        if end is not None:
+            end = gridstatus.utils._handle_date(end, tz)
 
         # handle pagination
         page = 1
         has_next_page = True
         dfs = []
         total_time = 0
         while has_next_page:
```

### Comparing `gridstatusio-0.2.1/gridstatusio/tests/test_api.py` & `gridstatusio-0.2.2/gridstatusio/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.2.1/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.2.2/gridstatusio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.2.1/pyproject.toml` & `gridstatusio-0.2.2/pyproject.toml`

 * *Files identical despite different names*

