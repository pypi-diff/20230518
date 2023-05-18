# Comparing `tmp/stability-sdk-0.8.0.tar.gz` & `tmp/stability-sdk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.8.0.tar", last modified: Thu May 11 16:00:36 2023, max compression
+gzip compressed data, was "stability-sdk-0.8.1.tar", last modified: Thu May 18 21:37:10 2023, max compression
```

## Comparing `stability-sdk-0.8.0.tar` & `stability-sdk-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.770250 stability-sdk-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.778250 stability-sdk-0.8.0/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54884 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38386 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/animation_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37427 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-05-11 16:00:16.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.774250 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.786250 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-11 16:00:17.000000 stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.782250 stability-sdk-0.8.0/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 16:00:36.000000 stability-sdk-0.8.0/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:36.790250 stability-sdk-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_animator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-11 16:00:15.000000 stability-sdk-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.166363 stability-sdk-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55273 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37904 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/animation_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28265 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37427 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.166363 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-18 21:36:52.000000 stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-18 21:36:49.000000 stability-sdk-0.8.1/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.170363 stability-sdk-0.8.1/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-18 21:37:10.000000 stability-sdk-0.8.1/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-18 21:37:10.000000 stability-sdk-0.8.1/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:37:10.000000 stability-sdk-0.8.1/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 21:37:10.000000 stability-sdk-0.8.1/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 21:37:10.000000 stability-sdk-0.8.1/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:37:10.174363 stability-sdk-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/tests/test_animator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-18 21:36:50.000000 stability-sdk-0.8.1/tests/test_utils.py
```

### Comparing `stability-sdk-0.8.0/LICENSE` & `stability-sdk-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/PKG-INFO` & `stability-sdk-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
```

### Comparing `stability-sdk-0.8.0/README.md` & `stability-sdk-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/setup.py` & `stability-sdk-0.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.8.0',
+    version='0.8.1',
     author='Stability AI',
     author_email='support@stability.ai',
     maintainer='Stability AI',
     maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
     description='Python SDK for interacting with stability.ai APIs',
```

### Comparing `stability-sdk-0.8.0/src/stability_sdk/__main__.py` & `stability-sdk-0.8.1/src/stability_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/animation.py` & `stability-sdk-0.8.1/src/stability_sdk/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import math
 import numpy as np
 import os
 import param
 import random
 import shutil
-import subprocess
 
 from collections import OrderedDict, deque
 from dataclasses import dataclass, fields
 from keyframed.dsl import curve_from_cn_string
 from PIL import Image, ImageOps
 from types import SimpleNamespace
 from typing import Callable, cast, Deque, Dict, Generator, List, Optional, Tuple, Union
@@ -801,31 +800,36 @@
         # change request for random seed into explicit value so it is saved to settings
         if args.seed <= 0:
             args.seed = random.randint(0, 2**32 - 1)
 
         # select image generation model
         self.api._generate.engine_id = args.custom_model if args.model == "custom" else args.model
 
+        # validate dimensions
+        if args.width % 64 != 0 or args.height % 64 != 0:
+            args.width, args.height = map(lambda x: x - x % 64, (args.width, args.height))
+            logger.warning(f"Adjusted dimensions to {args.width}x{args.height} to be multiples of 64.")
+
         # validate border settings
         if args.border == 'wrap' and args.animation_mode != '2D':
             args.border = 'reflect'
             logger.warning(f"Border 'wrap' is only supported in 2D mode, switching to '{args.border}'.")
+        if args.border == 'prefill' and args.animation_mode in ('2D', '3D warp') and not args.inpaint_border:
+            args.border = 'reflect'
+            logger.warning(f"Border 'prefill' is only supported when 'inpaint_border' is enabled, switching to '{args.border}'.")
 
         # validate clip guidance setting against selected model and sampler
         if args.clip_guidance.lower() != 'none':
             if not (model_supports_clip_guidance(args.model) and sampler_supports_clip_guidance(args.sampler)):
                 unsupported = args.model if not model_supports_clip_guidance(args.model) else args.sampler
                 logger.warning(f"CLIP guidance is not supported by {unsupported}, disabling guidance.")
                 args.clip_guidance = 'None'
 
-        def curve_to_series(curve: str) -> List[float]:
-            return curve_from_cn_string(curve)
-
         # expand key frame strings to per frame series
-        frame_args_dict = {f.name: curve_to_series(getattr(args, f.name)) for f in fields(FrameArgs)}
+        frame_args_dict = {f.name: curve_from_cn_string(getattr(args, f.name)) for f in fields(FrameArgs)}
         self.frame_args = FrameArgs(**frame_args_dict)        
 
         # prepare sorted list of key frames
         self.key_frame_values = sorted(list(self.animation_prompts.keys()))
         if self.key_frame_values[0] != 0:
             raise ValueError("First keyframe must be 0")
         if len(self.key_frame_values) != len(set(self.key_frame_values)):
@@ -949,15 +953,14 @@
                 next_b64 = base64.b64encode(image_to_png_bytes(video_next_frame)).decode('utf-8')
                 extras = { "warp_flow": { "prev_frame": prev_b64, "next_frame": next_b64, "export_mask": args.inpaint_border } }
                 transformed_prior_frames, masks = self.api.transform(self.prior_frames, generation.TransformParameters(), extras=extras)
                 if masks is not None:
                     mask = masks[0]
                 self.prior_frames.extend(transformed_prior_frames)
             self.video_prev_frame = video_next_frame
-            self.color_match_image = video_next_frame
             return mask
         return None
 
     def _postprocess_inpainting_mask(
         self,
         mask: Union[Image.Image, np.ndarray],
         mask_pow: Optional[float] = None,
```

### Comparing `stability-sdk-0.8.0/src/stability_sdk/animation_ui.py` & `stability-sdk-0.8.1/src/stability_sdk/animation_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,35 +284,34 @@
             with gr.Row():
                 upscale = gr.Checkbox(label="Upscale 2X", value=False, interactive=True)
         with gr.Column():
             image_out = gr.Image(label="image", visible=True)
             video_out = gr.Video(label="video", visible=False)
             process_button = gr.Button("Process")
             stop_button = gr.Button("Stop", visible=False)
-            error_log = gr.Textbox(label="Error", lines=3, visible=False)
+            status = gr.Textbox(lines=3, visible=False)
 
     def postprocess_video(fps: int, reverse: bool, interp_mode: str, interp_factor: int, upscale: bool,
                           use_video_instead: bool, video_to_postprocess: str):
         global interrupt, last_interp_factor, last_interp_mode, last_upscale
         interrupt = False
         if not use_video_instead and last_project_settings_path is None:
             raise gr.Error("Please render an animation first or specify a videofile to postprocess")
         if use_video_instead and not os.path.exists(video_to_postprocess):
             raise gr.Error("Videofile does not exist")
 
         yield {
-            header: gr.update(),
-            image_out: gr.update(visible=True, label=""),
+            image_out: gr.update(visible=True, label="", value=None),
             video_out: gr.update(visible=False),
             process_button: gr.update(visible=False),
             stop_button: gr.update(visible=True),
-            error_log: gr.update(visible=False),
+            status: gr.update(visible=False),
         }
 
-        error = None
+        error, output_video = None, None
         try:
             outdir = os.path.dirname(last_project_settings_path) \
                 if not use_video_instead \
                 else extract_frames_from_video(video_to_postprocess)
             suffix = ""
 
             can_skip_upscale = last_upscale == upscale
@@ -329,18 +328,14 @@
                     for frame_idx in tqdm(range(num_frames)):
                         frame = Image.open(frame_paths[frame_idx])
                         frame = context.upscale(frame)
                         frame.save(os.path.join(upscale_dir, os.path.basename(frame_paths[frame_idx])))
                         yield {
                             header: gr.update(value=format_header_html()) if frame_idx % 12 == 0 else gr.update(),
                             image_out: gr.update(value=frame, label=f"upscale {frame_idx}/{num_frames}", visible=True),
-                            video_out: gr.update(visible=False),
-                            process_button: gr.update(visible=False),
-                            stop_button: gr.update(visible=True),
-                            error_log: gr.update(visible=False),
                         }
                         if interrupt:
                             break
                     last_upscale = upscale
                 outdir = upscale_dir
 
             if interp_mode != 'None':
@@ -350,53 +345,52 @@
                 if not can_skip_interp:
                     remove_frames_from_path(interp_dir)
                     num_frames = interp_factor * len(glob.glob(os.path.join(outdir, "frame_*.png")))
                     for frame_idx, frame in enumerate(tqdm(interpolate_frames(context, outdir, interp_dir, interp_mode, interp_factor), total=num_frames)):
                         yield {
                             header: gr.update(value=format_header_html()) if frame_idx % 12 == 0 else gr.update(),
                             image_out: gr.update(value=frame, label=f"interpolate {frame_idx}/{num_frames}", visible=True),
-                            video_out: gr.update(visible=False),
-                            process_button: gr.update(visible=False),
-                            stop_button: gr.update(visible=True),
-                            error_log: gr.update(visible=False),
                         }
                         if interrupt:
                             break
                     last_interp_mode, last_interp_factor = interp_mode, interp_factor
                 outdir = interp_dir
 
             if not use_video_instead:
                 output_video = last_project_settings_path.replace(".json", f"{suffix}.mp4")
             else:
                 _, video_ext = os.path.splitext(video_to_postprocess)
                 output_video = video_to_postprocess.replace(video_ext, f"{suffix}.mp4")
+
+            yield { status: gr.update(label="Status", value="Compiling frames to MP4...", visible=True) }
             create_video_from_frames(outdir, output_video, fps=fps, reverse=reverse)
         except Exception as e:
             traceback.print_exc()
             error = f"Post-processing terminated early due to exception: {e}"
 
         yield {
             header: gr.update(value=format_header_html()),
             image_out: gr.update(visible=False),
             video_out: gr.update(value=output_video, visible=True),
             process_button: gr.update(visible=True),
             stop_button: gr.update(visible=False),
-            error_log: gr.update(value=error, visible=bool(error))
+            status: gr.update(label="Error", value=error, visible=bool(error))
         }
 
     process_button.click(
         postprocess_video, 
         inputs=[fps, reverse, frame_interp_mode, frame_interp_factor, upscale, use_video_instead, video_to_postprocess], 
-        outputs=[header, image_out, video_out, process_button, stop_button, error_log]
+        outputs=[header, image_out, video_out, process_button, stop_button, status]
     )    
 
-    def stop_button_click():
+    def stop():
         global interrupt
         interrupt = True
-    stop_button.click(stop_button_click)
+        return { status: gr.update(label="Status", value="Stopping...", visible=True)}
+    stop_button.click(stop, outputs=[status])
 
 
 def project_create(title, preset):
     ensure_api_context()
     global project, projects
     titles = [p.title for p in projects]
     if title in titles:
@@ -552,15 +546,15 @@
         with gr.Column():
             ui_layout_tabs()
         with gr.Column():
             image_out = gr.Image(label="image", visible=True)
             video_out = gr.Video(label="video", visible=False)
             button = gr.Button("Render")
             button_stop = gr.Button("Stop", visible=False)
-            error_log = gr.Textbox(label="Error", lines=3, visible=False)
+            status = gr.Textbox(lines=3, visible=False)
 
     def render(resume: bool, resume_from: int, *render_args):
         global interrupt, last_interp_factor, last_interp_mode, last_project_settings_path, last_upscale, project
         interrupt = False
 
         if not project:
             raise gr.Error("No project active!")
@@ -607,18 +601,17 @@
         with open(project_settings_path, 'w', encoding='utf-8') as f:
             json.dump(save_dict, f, indent=4)
 
         # initial yield to switch render button to stop button
         yield {
             button: gr.update(visible=False),
             button_stop: gr.update(visible=True),
-            image_out: gr.update(visible=True, label=""),
+            image_out: gr.update(visible=True, label="", value=None),
             video_out: gr.update(visible=False),
-            header: gr.update(),
-            error_log: gr.update(visible=False),
+            status: gr.update(visible=False),
         }
 
         # delete frames from previous animation
         if resume:
             if resume_from > 0:
                 remove_frames_from_path(outdir, resume_from)
             elif resume_from == 0 or resume_from < -1:
@@ -637,24 +630,17 @@
                 negative_prompt_weight=negative_prompt_weight,
                 resume=resume,
             )
             for frame_idx, frame in enumerate(tqdm(animator.render(), initial=animator.start_frame_idx, total=args.max_frames), start=animator.start_frame_idx):
                 if interrupt:
                     break
 
-                # saving frames to project
-                #frame_uuid = project.put_image_asset(frame)
-
                 yield {
-                    button: gr.update(visible=False),
-                    button_stop: gr.update(visible=True),
                     image_out: gr.update(value=frame, label=f"frame {frame_idx}/{args.max_frames}", visible=True),
-                    video_out: gr.update(visible=False),
                     header: gr.update(value=format_header_html()) if frame_idx % 12 == 0 else gr.update(),
-                    error_log: gr.update(visible=False),
                 }
         except ClassifierException as e:
             error = "Animation terminated early due to NSFW classifier."
             if e.prompt is not None:
                 error += "\nPlease revise your prompt: " + e.prompt
         except OutOfCreditsException as e:
             error = f"Animation terminated early, out of credits.\n{e.details}"
@@ -662,41 +648,45 @@
             traceback.print_exc()
             error = f"Animation terminated early due to exception: {e}"
 
         if frame_idx:
             last_project_settings_path = project_settings_path
             last_interp_factor, last_interp_mode, last_upscale = None, None, None
             output_video = project_settings_path.replace(".json", ".mp4")
+            yield {
+                status: gr.update(label="Status", value="Compiling frames to MP4...", visible=True),
+            }
             try:
                 create_video_from_frames(outdir, output_video, fps=args.fps, reverse=args.reverse)
             except RuntimeError as e:
                 error = f"Error creating video: {e}"
                 output_video = None
         else:
             output_video = None
         yield {
             button: gr.update(visible=True),
             button_stop: gr.update(visible=False),
             image_out: gr.update(visible=False),
             video_out: gr.update(value=output_video, visible=True),
             header: gr.update(value=format_header_html()),
-            error_log: gr.update(value=error, visible=bool(error)),
+            status: gr.update(label="Error", value=error, visible=bool(error)),
         }
 
     button.click(
         render,
         inputs=[resume_checkbox, resume_from_number] + list(controls.values()),
-        outputs=[button, button_stop, image_out, video_out, header, error_log]
+        outputs=[button, button_stop, image_out, video_out, header, status]
     )
 
     # stop animation in progress 
     def stop():
         global interrupt
         interrupt = True
-    button_stop.click(stop)
+        return { status: gr.update(label="Status", value="Stopping...", visible=True) }
+    button_stop.click(stop, outputs=[status])
 
 def ui_for_animation_settings(args: AnimationSettings):
     with gr.Row():
         controls["steps_strength_adj"] = gr.Checkbox(label="Steps strength adj", value=args.param.steps_strength_adj.default, interactive=True)
         controls["interpolate_prompts"] = gr.Checkbox(label="Interpolate prompts", value=args.param.interpolate_prompts.default, interactive=True)
         controls["locked_seed"] = gr.Checkbox(label="Locked seed", value=args.param.locked_seed.default, interactive=True)
     controls["noise_add_curve"] = gr.Text(label="Noise add curve", value=args.param.noise_add_curve.default, interactive=True)
```

### Comparing `stability-sdk-0.8.0/src/stability_sdk/api.py` & `stability-sdk-0.8.1/src/stability_sdk/api.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/client.py` & `stability-sdk-0.8.1/src/stability_sdk/client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/project/project_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.8.1/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/matrix.py` & `stability-sdk-0.8.1/src/stability_sdk/matrix.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk/utils.py` & `stability-sdk-0.8.1/src/stability_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.8.1/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
 Author: Stability AI
 Author-email: support@stability.ai
 Maintainer: Stability AI
 Maintainer-email: support@stability.ai
```

### Comparing `stability-sdk-0.8.0/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.8.1/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/tests/test_animator.py` & `stability-sdk-0.8.1/tests/test_animator.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/tests/test_api.py` & `stability-sdk-0.8.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/tests/test_client.py` & `stability-sdk-0.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.8.0/tests/test_utils.py` & `stability-sdk-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

