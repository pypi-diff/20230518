# Comparing `tmp/turbine-py-1.9.0.tar.gz` & `tmp/turbine-py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbine-py-1.9.0.tar", last modified: Thu May 18 16:52:32 2023, max compression
+gzip compressed data, was "turbine-py-2.0.0.tar", last modified: Thu May 18 20:11:23 2023, max compression
```

## Comparing `turbine-py-1.9.0.tar` & `turbine-py-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.956105 turbine-py-1.9.0/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 16:52:22.000000 turbine-py-1.9.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 16:52:22.000000 turbine-py-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 16:52:32.956105 turbine-py-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8098 2023-05-18 16:52:22.000000 turbine-py-1.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.944105 turbine-py-1.9.0/pkg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/
--rw-r--r--   0 root         (0) root         (0)      125 2023-05-18 16:52:23.000000 turbine-py-1.9.0/pkg/turbine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2206 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/src/
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/src/function_deploy/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/Dockerfile
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/README.md
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3048 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/function_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.952105 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/record.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.952105 turbine-py-1.9.0/pkg/turbine/src/turbine_app/
--rw-r--r--   0 root         (0) root         (0)      425 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/app.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.952105 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8831 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15253 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13062 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/resource.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/types.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.956105 turbine-py-1.9.0/pkg/turbine_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1148 2023-05-18 16:52:32.956105 turbine-py-1.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.956105 turbine-py-1.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-18 16:52:22.000000 turbine-py-1.9.0/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.472128 turbine-py-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 20:11:11.000000 turbine-py-2.0.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 20:11:11.000000 turbine-py-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 20:11:23.472128 turbine-py-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8098 2023-05-18 20:11:11.000000 turbine-py-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.460128 turbine-py-2.0.0/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.460128 turbine-py-2.0.0/pkg/turbine/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-18 20:11:12.000000 turbine-py-2.0.0/pkg/turbine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.460128 turbine-py-2.0.0/pkg/turbine/src/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.464128 turbine-py-2.0.0/pkg/turbine/src/function_deploy/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.464128 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/README.md
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/function_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.464128 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/record.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/function_deploy/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.468128 turbine-py-2.0.0/pkg/turbine/src/turbine_app/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/app.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.468128 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15253 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13062 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/resource.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/types.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pkg/turbine/src/turbine_app/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.472128 turbine-py-2.0.0/pkg/turbine_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:11:23.000000 turbine-py-2.0.0/pkg/turbine_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 20:11:11.000000 turbine-py-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-18 20:11:23.472128 turbine-py-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:11:23.472128 turbine-py-2.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-18 20:11:11.000000 turbine-py-2.0.0/tests/test_cli.py
```

### Comparing `turbine-py-1.9.0/PKG-INFO` & `turbine-py-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.9.0
+Version: 2.0.0
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.9.0/README.md` & `turbine-py-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/cli.py` & `turbine-py-2.0.0/pkg/turbine/cli.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/README.md` & `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/function_server.py` & `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/function_server.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py` & `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi` & `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py` & `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/record.py` & `turbine-py-2.0.0/pkg/turbine/src/function_deploy/function_app/record.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/app.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/app.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/client.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/client.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/resource.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/resource.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/types.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/types.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine/src/turbine_app/utils.py` & `turbine-py-2.0.0/pkg/turbine/src/turbine_app/utils.py`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/pkg/turbine_py.egg-info/PKG-INFO` & `turbine-py-2.0.0/pkg/turbine_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.9.0
+Version: 2.0.0
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.9.0/pkg/turbine_py.egg-info/SOURCES.txt` & `turbine-py-2.0.0/pkg/turbine_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `turbine-py-1.9.0/setup.cfg` & `turbine-py-2.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 packages = find:
 package_dir = = pkg
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	aiohttp>=3.8
 	grpcio>=1.44.0
-	meroxa-py>=1.3.1
+	google>=3.0.0
+	google-api-python-client>=2.86.0
+	grpcio-tools>=1.44.0
+	protobuf>=3.20.0
+	grpcio-reflection>=1.44.0
+	grpcio-health-checking>=1.44.0
 
 [options.entry_points]
 console_scripts = 
 	turbine-py = turbine.cli:main
 
 [options.packages.find]
 where = pkg
```

### Comparing `turbine-py-1.9.0/tests/test_cli.py` & `turbine-py-2.0.0/tests/test_cli.py`

 * *Files identical despite different names*

