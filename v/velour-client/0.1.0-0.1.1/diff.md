# Comparing `tmp/velour-client-0.1.0.tar.gz` & `tmp/velour-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velour-client-0.1.0.tar", last modified: Wed May 17 12:53:45 2023, max compression
+gzip compressed data, was "velour-client-0.1.1.tar", last modified: Thu May 18 14:36:24 2023, max compression
```

## Comparing `velour-client-0.1.0.tar` & `velour-client-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:53:45.690816 velour-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-17 12:53:36.000000 velour-client-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-17 12:53:45.690816 velour-client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 12:53:36.000000 velour-client-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-17 12:53:36.000000 velour-client-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:53:45.690816 velour-client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 12:53:36.000000 velour-client-0.1.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:53:45.686815 velour-client-0.1.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-17 12:53:36.000000 velour-client-0.1.0/unit-tests/test_chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-17 12:53:36.000000 velour-client-0.1.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-17 12:53:36.000000 velour-client-0.1.0/unit-tests/test_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-17 12:53:36.000000 velour-client-0.1.0/unit-tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-17 12:53:36.000000 velour-client-0.1.0/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:53:45.690816 velour-client-0.1.0/velour/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:53:45.690816 velour-client-0.1.0/velour/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/integrations/chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/integrations/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-17 12:53:36.000000 velour-client-0.1.0/velour/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:53:45.690816 velour-client-0.1.0/velour_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-17 12:53:45.000000 velour-client-0.1.0/velour_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 12:53:45.000000 velour-client-0.1.0/velour_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:53:45.000000 velour-client-0.1.0/velour_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 12:53:45.000000 velour-client-0.1.0/velour_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 12:53:45.000000 velour-client-0.1.0/velour_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.493789 velour-client-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 14:36:10.000000 velour-client-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 14:36:24.493789 velour-client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 14:36:10.000000 velour-client-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-18 14:36:10.000000 velour-client-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:36:24.493789 velour-client-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-18 14:36:10.000000 velour-client-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.489789 velour-client-0.1.1/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-18 14:36:10.000000 velour-client-0.1.1/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.489789 velour-client-0.1.1/velour/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27484 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.489789 velour-client-0.1.1/velour/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/integrations/chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/integrations/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-18 14:36:10.000000 velour-client-0.1.1/velour/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:24.493789 velour-client-0.1.1/velour_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 14:36:24.000000 velour-client-0.1.1/velour_client.egg-info/top_level.txt
```

### Comparing `velour-client-0.1.0/LICENSE` & `velour-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/PKG-INFO` & `velour-client-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.1.0/pyproject.toml` & `velour-client-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/unit-tests/test_chariot.py` & `velour-client-0.1.1/unit-tests/test_chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/unit-tests/test_client.py` & `velour-client-0.1.1/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/unit-tests/test_coco.py` & `velour-client-0.1.1/unit-tests/test_coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/unit-tests/test_data_types.py` & `velour-client-0.1.1/unit-tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/unit-tests/test_viz.py` & `velour-client-0.1.1/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/velour/client.py` & `velour-client-0.1.1/velour/client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/velour/data_types.py` & `velour-client-0.1.1/velour/data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/velour/integrations/chariot.py` & `velour-client-0.1.1/velour/integrations/chariot.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,31 +21,26 @@
     PolygonWithHole,
     PredictedDetection,
     ScoredLabel,
 )
 
 try:
     from chariot.config import settings
-    from chariot.datasets.dataset import Dataset
-    from chariot.datasets.dataset_version import (
-        get_latest_vertical_dataset_version,
-    )
-
+    from chariot.datasets import Dataset, get_latest_vertical_dataset_version
 except ModuleNotFoundError:
     "`chariot` package not found. if you have an account on Chariot please see https://production.chariot.striveworks.us/docs/sdk/sdk for how to install the python SDK"
 
 
 def retrieve_chariot_manifest(manifest_url: str):
     """Retrieves and unpacks Chariot dataset annotations from a manifest url."""
 
     chariot_dataset = []
 
     # Create a temporary file
     with tempfile.TemporaryFile(mode="w+b") as f:
-
         # Download compressed jsonl file
         response = requests.get(manifest_url, stream=True)
 
         # Progress bar
         total_size_in_bytes = int(response.headers.get("content-length", 0))
         block_size = 1024  # 1 Kibibyte
         progress_bar = tqdm(
@@ -106,15 +101,14 @@
     """Parses Chariot image segmentation annotation."""
 
     # Strip UID from URL path
     uid = Path(datum["path"]).stem
 
     annotated_regions = {}
     for annotation in datum["annotations"]:
-
         annotation_label = annotation["class_label"]
 
         hole = None
 
         # Create BoundingPolygon
         points = [
             Point(x=point["x"], y=point["y"])
```

### Comparing `velour-client-0.1.0/velour/integrations/coco.py` & `velour-client-0.1.1/velour/integrations/coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/velour/viz.py` & `velour-client-0.1.1/velour/viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.1.0/velour_client.egg-info/PKG-INFO` & `velour-client-0.1.1/velour_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

