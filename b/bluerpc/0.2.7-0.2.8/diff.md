# Comparing `tmp/bluerpc-0.2.7.tar.gz` & `tmp/bluerpc-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluerpc-0.2.7.tar", last modified: Sun May 14 16:17:25 2023, max compression
+gzip compressed data, was "bluerpc-0.2.8.tar", last modified: Thu May 18 15:04:11 2023, max compression
```

## Comparing `bluerpc-0.2.7.tar` & `bluerpc-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:25.666737 bluerpc-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 16:17:25.666737 bluerpc-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:16:17.000000 bluerpc-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:25.666737 bluerpc-0.2.7/bluerpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/ble_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/ble_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:25.666737 bluerpc-0.2.7/bluerpc/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/gatt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/gatt_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/services_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-14 16:17:16.000000 bluerpc-0.2.7/bluerpc/rpc/services_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-14 16:16:17.000000 bluerpc-0.2.7/bluerpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:17:25.666737 bluerpc-0.2.7/bluerpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 16:17:25.000000 bluerpc-0.2.7/bluerpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 16:17:25.000000 bluerpc-0.2.7/bluerpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:17:25.000000 bluerpc-0.2.7/bluerpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-14 16:17:25.000000 bluerpc-0.2.7/bluerpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 16:17:25.000000 bluerpc-0.2.7/bluerpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 16:17:25.000000 bluerpc-0.2.7/bluerpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:17:25.666737 bluerpc-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-14 16:16:17.000000 bluerpc-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:04:11.097549 bluerpc-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 15:04:11.097549 bluerpc-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:03:03.000000 bluerpc-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:04:11.093549 bluerpc-0.2.8/bluerpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19450 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/ble_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/ble_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:04:11.097549 bluerpc-0.2.8/bluerpc/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/gatt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/gatt_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/services_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-18 15:04:02.000000 bluerpc-0.2.8/bluerpc/rpc/services_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-18 15:03:03.000000 bluerpc-0.2.8/bluerpc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:04:11.097549 bluerpc-0.2.8/bluerpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 15:04:11.000000 bluerpc-0.2.8/bluerpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-18 15:04:11.000000 bluerpc-0.2.8/bluerpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:04:11.000000 bluerpc-0.2.8/bluerpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 15:04:11.000000 bluerpc-0.2.8/bluerpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 15:04:11.000000 bluerpc-0.2.8/bluerpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 15:04:11.000000 bluerpc-0.2.8/bluerpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:04:11.097549 bluerpc-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-18 15:03:03.000000 bluerpc-0.2.8/setup.py
```

### Comparing `bluerpc-0.2.7/PKG-INFO` & `bluerpc-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluerpc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python BlueRPC Worker
 Home-page: https://github.com/BlueRPC/BlueRPC
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://bluerpc.github.io/
 Project-URL: Source, https://github.com/BlueRPC/BlueRPC/python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluerpc-0.2.7/bluerpc/ble_conn.py` & `bluerpc-0.2.8/bluerpc/ble_conn.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/ble_scan.py` & `bluerpc-0.2.8/bluerpc/ble_scan.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/cli.py` & `bluerpc-0.2.8/bluerpc/cli.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/discovery.py` & `bluerpc-0.2.8/bluerpc/discovery.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/log.py` & `bluerpc-0.2.8/bluerpc/log.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/rpc/common_pb2.py` & `bluerpc-0.2.8/bluerpc/rpc/common_pb2.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/rpc/gatt_pb2.py` & `bluerpc-0.2.8/bluerpc/rpc/gatt_pb2.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/rpc/services_pb2.py` & `bluerpc-0.2.8/bluerpc/rpc/services_pb2.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/rpc/services_pb2_grpc.py` & `bluerpc-0.2.8/bluerpc/rpc/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/service.py` & `bluerpc-0.2.8/bluerpc/service.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc/utils.py` & `bluerpc-0.2.8/bluerpc/utils.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/bluerpc.egg-info/PKG-INFO` & `bluerpc-0.2.8/bluerpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluerpc
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python BlueRPC Worker
 Home-page: https://github.com/BlueRPC/BlueRPC
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://bluerpc.github.io/
 Project-URL: Source, https://github.com/BlueRPC/BlueRPC/python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluerpc-0.2.7/bluerpc.egg-info/SOURCES.txt` & `bluerpc-0.2.8/bluerpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluerpc-0.2.7/setup.py` & `bluerpc-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="bluerpc",
     packages=find_packages(),
-    version="0.2.7",
+    version="0.2.8",
     author="drosocode",
     license="MIT",
     description="Python BlueRPC Worker",
     url="https://github.com/BlueRPC/BlueRPC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

