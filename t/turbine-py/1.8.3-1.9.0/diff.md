# Comparing `tmp/turbine-py-1.8.3.tar.gz` & `tmp/turbine-py-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbine-py-1.8.3.tar", last modified: Tue May  9 16:47:05 2023, max compression
+gzip compressed data, was "turbine-py-1.9.0.tar", last modified: Thu May 18 16:52:32 2023, max compression
```

## Comparing `turbine-py-1.8.3.tar` & `turbine-py-1.9.0.tar`

### file list

```diff
@@ -1,59 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-09 16:46:55.000000 turbine-py-1.8.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-09 16:46:55.000000 turbine-py-1.8.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-09 16:47:05.668176 turbine-py-1.8.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8098 2023-05-09 16:46:55.000000 turbine-py-1.8.3/README.md
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-09 16:46:55.000000 turbine-py-1.8.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1148 2023-05-09 16:47:05.668176 turbine-py-1.8.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/turbine/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/turbine/function_deploy/
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.660176 turbine-py-1.8.3/src/turbine/function_deploy/data_app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/data_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/function_deploy/function_app/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/README.md
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/function_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/function_deploy/function_app/protos/
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/protos/service.proto
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/record.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2895 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/runner/
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/app_generate.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/baserunner.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runner/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/runtime/
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/info.py
--rw-r--r--   0 root         (0) root         (0)     3924 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/intermediate.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/local.py
--rw-r--r--   0 root         (0) root         (0)    11804 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/platform.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/runtime/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.656176 turbine-py-1.8.3/src/turbine/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.664176 turbine-py-1.8.3/src/turbine/templates/python/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/.gitignore
--rw-r--r--   0 root         (0) root         (0)     6438 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/README.md
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/app.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/src/turbine/templates/python/fixtures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/fixtures/.gitkeep
--rw-r--r--   0 root         (0) root         (0)     8360 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/fixtures/demo-cdc.json
--rw-r--r--   0 root         (0) root         (0)     4691 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/fixtures/demo-no-cdc.json
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/main.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 16:46:55.000000 turbine-py-1.8.3/src/turbine/templates/python/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/src/turbine_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1637 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 16:47:05.000000 turbine-py-1.8.3/src/turbine_py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:47:05.668176 turbine-py-1.8.3/tests/
--rw-r--r--   0 root         (0) root         (0)     3822 2023-05-09 16:46:55.000000 turbine-py-1.8.3/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.956105 turbine-py-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 16:52:22.000000 turbine-py-1.9.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 16:52:22.000000 turbine-py-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 16:52:32.956105 turbine-py-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8098 2023-05-18 16:52:22.000000 turbine-py-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.944105 turbine-py-1.9.0/pkg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-18 16:52:23.000000 turbine-py-1.9.0/pkg/turbine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/src/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/src/function_deploy/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.948105 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/README.md
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/function_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.952105 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/record.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/function_deploy/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.952105 turbine-py-1.9.0/pkg/turbine/src/turbine_app/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/app.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.952105 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8831 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15253 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/turbine_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13062 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/proto_gen/validate_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/resource.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/types.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pkg/turbine/src/turbine_app/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.956105 turbine-py-1.9.0/pkg/turbine_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 16:52:32.000000 turbine-py-1.9.0/pkg/turbine_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 16:52:22.000000 turbine-py-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-05-18 16:52:32.956105 turbine-py-1.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:52:32.956105 turbine-py-1.9.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-18 16:52:22.000000 turbine-py-1.9.0/tests/test_cli.py
```

### Comparing `turbine-py-1.8.3/PKG-INFO` & `turbine-py-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbine-py
-Version: 1.8.3
+Version: 1.9.0
 Summary: Meroxa Turbine data application framework
 Home-page: https://meroxa.io/
 Author: Eric Cheatham
 Author-email: eric@meroxa.io
 License: MIT
 Project-URL: Source Code, https://github.com/meroxa/turbine-py/
 Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
```

### Comparing `turbine-py-1.8.3/README.md` & `turbine-py-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.3/setup.cfg` & `turbine-py-1.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 classifiers = 
 	Programming Language :: Python
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-package_dir = = src
+package_dir = = pkg
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	aiohttp>=3.8
 	grpcio>=1.44.0
 	meroxa-py>=1.3.1
 
 [options.entry_points]
 console_scripts = 
 	turbine-py = turbine.cli:main
 
 [options.packages.find]
-where = src
+where = pkg
 
 [semantic_release]
-version_variable = src/turbine/__init__.py:__version__
+version_variable = pkg/turbine/__init__.py:__version__
 version_source = commit
 branch = main
 changelog_file = CHANGELOG.md
 upload_to_repository = true
 upload_to_release = true
 build_command = pip install build --user && python -m build
```

### Comparing `turbine-py-1.8.3/src/turbine/function_deploy/function_app/README.md` & `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/README.md`

 * *Files identical despite different names*

### Comparing `turbine-py-1.8.3/src/turbine/function_deploy/function_app/function_server.py` & `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/function_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,73 @@
-import asyncio
 import logging
 import os
 import sys
 
 import grpc.aio
-import service_pb2
-import service_pb2_grpc
 from grpc_health.v1 import health
 from grpc_health.v1 import health_pb2
 from grpc_health.v1 import health_pb2_grpc
 from grpc_reflection.v1alpha import reflection
-from record import proto_records_to_turbine_records
-from record import turbine_records_to_proto_records
+from .proto_gen import add_FunctionServicer_to_server
+from .proto_gen import FunctionServicer
+from .proto_gen import ProcessRecordRequest
+from .proto_gen import ProcessRecordResponse
+from .record import proto_records_to_turbine_records
+from .record import turbine_records_to_proto_records
+
+# from importlib.resources import path
 
 """
 Process function given to GRPC server
 """
 
-FUNCTION_NAME = sys.argv[1]
 FUNCTION_ADDRESS = os.getenv("MEROXA_FUNCTION_ADDR")
-PATH_TO_DATA_APP = os.path.normpath(os.path.dirname(__file__) + "/../data_app/")
+PATH_TO_DATA_APP = os.getcwd()
 
 # Coroutines to be invoked when the event loop is shutting down.
 _cleanup_coroutines = []
 
 
-class Funtime(service_pb2_grpc.FunctionServicer):
+class FunctionServer(FunctionServicer):
+    def __init__(self, function_name) -> None:
+        self.function_name = function_name
+        super().__init__()
+
     @staticmethod
     def _obtain_client_data_app_function(path_to_data_app: str, function_name: str):
         sys.path.append(path_to_data_app)
         import main
 
         return main.__getattribute__(function_name)
 
-    def Process(
+    async def Process(
         self,
-        request: service_pb2.ProcessRecordRequest,
+        request: ProcessRecordRequest,
         context: grpc.aio.ServicerContext,
-    ) -> service_pb2.ProcessRecordResponse:
+    ) -> ProcessRecordResponse:
         # map from rpc => something we can work with
         input_records = proto_records_to_turbine_records(request.records)
 
         # Get the data app function
         data_app_function = self._obtain_client_data_app_function(
-            path_to_data_app=PATH_TO_DATA_APP, function_name=FUNCTION_NAME
+            path_to_data_app=PATH_TO_DATA_APP, function_name=self.function_name
         )
 
         # Generate output
         output_records = data_app_function(input_records)
 
         # Serialize and return
         grpc_records = turbine_records_to_proto_records(output_records)
 
-        return service_pb2.ProcessRecordResponse(records=grpc_records)
+        return ProcessRecordResponse(records=grpc_records)
 
 
-async def serve() -> None:
+async def serve(function_name) -> None:
     server = grpc.aio.server()
-    service_pb2_grpc.add_FunctionServicer_to_server(Funtime(), server)
+    add_FunctionServicer_to_server(FunctionServer(function_name), server)
 
     # Create a health check servicer. We use the non-blocking implementation
     # to avoid thread starvation.
     health_servicer = health.HealthServicer(experimental_non_blocking=True)
 
     # Create a tuple of all the services we want to export via reflection.
     services = tuple(
@@ -81,20 +87,7 @@
 
     async def shutdown():
         logging.info("Shutting python gRPC server down..")
         await server.stop(grace=5)
 
     _cleanup_coroutines.append(shutdown())
     await server.wait_for_termination()
-
-
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.INFO)
-
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-
-    try:
-        loop.run_until_complete(serve())
-    finally:
-        loop.run_until_complete(*_cleanup_coroutines)
-        loop.close()
```

### Comparing `turbine-py-1.8.3/src/turbine/function_deploy/function_app/record.py` & `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 import json
-
-# KTLO: https://github.com/meroxa/turbine-py/issues/151
-try:
-    import service_pb2
-except ModuleNotFoundError:
-    from . import service_pb2
-
-from turbine.runtime import Record
+from ...turbine_app import Record
+from .proto_gen import service_pb2
 
 
 def proto_records_to_turbine_records(p_record: list[service_pb2.Record]):
     return [
         Record(
             key=record.key,
             value=decode_record(record),
```

### Comparing `turbine-py-1.8.3/src/turbine/function_deploy/function_app/service_pb2_grpc.py` & `turbine-py-1.9.0/pkg/turbine/src/function_deploy/function_app/proto_gen/service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
-
-import service_pb2 as service__pb2
+from . import service_pb2 as service__pb2
 
 
 class FunctionStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `turbine-py-1.8.3/src/turbine/templates/python/README.md` & `turbine-py-1.9.0/pkg/turbine_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,63 @@
+Metadata-Version: 2.1
+Name: turbine-py
+Version: 1.9.0
+Summary: Meroxa Turbine data application framework
+Home-page: https://meroxa.io/
+Author: Eric Cheatham
+Author-email: eric@meroxa.io
+License: MIT
+Project-URL: Source Code, https://github.com/meroxa/turbine-py/
+Project-URL: Issue Tracker, https://github.com/meroxa/turbine-py/issues
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Turbine
+
+<p align="center" style="text-align:center;">
+  <img alt="turbine logo" src="https://github.com/meroxa/turbine-py/blob/main/docs/turbine-outline.svg?raw=true" width="500" />
+</p>
+
+
+
+Turbine is a data application framework for building server-side applications that are event-driven, respond to data in real-time, and scale using cloud-native best practices.
+
+The benefits of using Turbine include:
+
+* **Native Developer Tooling:** Turbine doesn't come with any bespoke DSL or patterns. Write software like you normally would!
+
+* **Fits into Existing DevOps Workflows:** Build, test, and deploy. Turbine encourages best practices from the start. Don't test your data app in production ever again.
+
+* **Local Development mirrors Production:** When running locally, you'll immediately see how your app reacts to data. What you get there will be exactly what happens in production but with _scale_ and _speed_.
+
+* **Available in many different programming langauages:** Turbine started out in Go but is available in other languages too:
+    * [Go](https://github.com/meroxa/turbine-go)
+    * [Javascript](https://github.com/meroxa/turbine-js)
+    * [Python](https://github.com/meroxa/turbine-py)
 
-# Meroxa Data App
 
 ## Getting Started
 
-The CLI will create a new folder with the name provided located in the directory where the command was issued. If you want to initialize the app somewhere else, you can append the `--path` flag to the command (`meroxa apps init testapp --lang py --path ~/anotherdir`). Once you enter the `testapp` directory, the contents will look like this:
+To get started, you'll need to install the `turbine-py` dependency via `pip`:
+
+```bash
+pip3 install turbine-py
+```
+
+Next, you'll need to [download the Meroxa CLI](https://github.com/meroxa/cli#installation-guide). Once downloaded and installed, initialize a new project using the following CLI command:
+
+```bash
+$ meroxa apps init testapp --lang py
+```
+
+The CLI will create a new folder called `testapp` located in the directory where the command was issued. If you want to initialize the app somewhere else, you can append the `--path` flag to the command (`meroxa apps init testapp --lang py --path ~/anotherdir`). Once you enter the `testapp` directory, the contents will look like this:
 
 ```bash
 $ tree testapp/
 testapp
 ├── README.md
 ├── main.py
 ├── app.json
@@ -148,10 +198,14 @@
 
 Testing should follow standard Python development practices.
 
 ## Documentation && Reference
 
 The most comprehensive documentation for Turbine and how to work with Turbine apps is on the Meroxa site: [https://docs.meroxa.com/](https://docs.meroxa.com)
 
-## Example apps
+## Contributing
+
+For information on how to contribute to Turbine-py, checkout our contribution guide [HERE](CONTRIBUTING.md)
+
+### Example apps
 
 [See what a sample python data app looks like using our framework](https://github.com/meroxa/turbine-py-examples)
```

