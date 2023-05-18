# Comparing `tmp/optumi-api-3.15.7.tar.gz` & `tmp/optumi-api-3.15.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.15.7.tar", last modified: Fri Apr 28 23:43:25 2023, max compression
+gzip compressed data, was "optumi-api-3.15.8.tar", last modified: Tue May 16 18:59:31 2023, max compression
```

## Comparing `optumi-api-3.15.7.tar` & `optumi-api-3.15.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:25.357160 optumi-api-3.15.7/
--rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-04-27 13:56:16.000000 optumi-api-3.15.7/LICENSE
--rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-04-27 13:56:16.000000 optumi-api-3.15.7/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-28 23:43:25.357160 optumi-api-3.15.7/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-27 13:56:16.000000 optumi-api-3.15.7/README.md
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-28 23:43:25.000000 optumi-api-3.15.7/core_version.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:25.357160 optumi-api-3.15.7/optumi_api/
--rw-rw-r--   0 denis     (1001) denis     (1001)     2883 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/CloudFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3677 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/CloudFileVersion.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5171 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/CloudStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4029 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Colab.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5352 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Container.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4402 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/ContainerRegistry.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/EnvironmentVariables.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6574 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Executable.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1006 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/HoldoverTime.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/LocalFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2402 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/LocalStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1515 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Log.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6281 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/LoginServer.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6734 2023-04-28 13:25:45.000000 optumi-api-3.15.7/optumi_api/Machine.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1957 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Machines.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Notebook.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6568 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/NotebookConfig.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2487 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Notifications.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      819 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Packages.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1620 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Program.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Provider.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1360 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Providers.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3283 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Resource.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Script.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4168 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/Server.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1968 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Summary.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    20469 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Workload.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3108 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/Workloads.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-04-27 18:15:41.000000 optumi-api-3.15.7/optumi_api/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    11309 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/api.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/cli.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3523 2023-04-27 13:56:16.000000 optumi-api-3.15.7/optumi_api/utils.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:25.357160 optumi-api-3.15.7/optumi_api.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/entry_points.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)       41 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-04-28 23:43:25.000000 optumi-api-3.15.7/optumi_api.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-28 23:43:25.357160 optumi-api-3.15.7/setup.cfg
--rwxrwxr-x   0 denis     (1001) denis     (1001)     2612 2023-04-27 13:56:16.000000 optumi-api-3.15.7/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-05-16 18:59:31.241001 optumi-api-3.15.8/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-05-16 18:57:48.000000 optumi-api-3.15.8/LICENSE
+-rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-05-16 18:57:48.000000 optumi-api-3.15.8/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-05-16 18:59:31.241001 optumi-api-3.15.8/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-05-16 18:57:48.000000 optumi-api-3.15.8/README.md
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-05-16 18:59:30.000000 optumi-api-3.15.8/core_version.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-05-16 18:59:31.237001 optumi-api-3.15.8/optumi_api/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2883 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/CloudFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3677 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/CloudFileVersion.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5171 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/CloudStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4029 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Colab.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5352 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Container.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4402 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/ContainerRegistry.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/EnvironmentVariables.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6574 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Executable.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1006 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/HoldoverTime.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/LocalFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2402 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/LocalStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1515 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Log.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6281 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/LoginServer.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6734 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Machine.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1957 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Machines.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Notebook.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6788 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/NotebookConfig.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2487 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Notifications.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      819 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Packages.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1620 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Program.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Provider.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1360 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Providers.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3647 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Resource.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Script.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4168 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Server.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1968 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Summary.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    20540 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Workload.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3110 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/Workloads.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    11669 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/api.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/cli.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3807 2023-05-16 18:57:48.000000 optumi-api-3.15.8/optumi_api/utils.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-05-16 18:59:31.241001 optumi-api-3.15.8/optumi_api.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/entry_points.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)       80 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-05-16 18:59:31.000000 optumi-api-3.15.8/optumi_api.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-05-16 18:59:31.241001 optumi-api-3.15.8/setup.cfg
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     2660 2023-05-16 18:57:48.000000 optumi-api-3.15.8/setup.py
```

### Comparing `optumi-api-3.15.7/PKG-INFO` & `optumi-api-3.15.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.7
+Version: 3.15.8
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.7/optumi_api/CloudFile.py` & `optumi-api-3.15.8/optumi_api/CloudFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/CloudFileVersion.py` & `optumi-api-3.15.8/optumi_api/CloudFileVersion.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/CloudStorage.py` & `optumi-api-3.15.8/optumi_api/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Colab.py` & `optumi-api-3.15.8/optumi_api/Colab.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Container.py` & `optumi-api-3.15.8/optumi_api/Container.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/ContainerRegistry.py` & `optumi-api-3.15.8/optumi_api/ContainerRegistry.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/EnvironmentVariables.py` & `optumi-api-3.15.8/optumi_api/EnvironmentVariables.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Executable.py` & `optumi-api-3.15.8/optumi_api/Executable.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/HoldoverTime.py` & `optumi-api-3.15.8/optumi_api/HoldoverTime.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/LocalFile.py` & `optumi-api-3.15.8/optumi_api/LocalFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/LocalStorage.py` & `optumi-api-3.15.8/optumi_api/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Log.py` & `optumi-api-3.15.8/optumi_api/Log.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/LoginServer.py` & `optumi-api-3.15.8/optumi_api/LoginServer.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Machine.py` & `optumi-api-3.15.8/optumi_api/Machine.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Machines.py` & `optumi-api-3.15.8/optumi_api/Machines.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Notebook.py` & `optumi-api-3.15.8/optumi_api/Notebook.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/NotebookConfig.py` & `optumi-api-3.15.8/optumi_api/NotebookConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,16 @@
             "required": False,
             "rating": [-1, -1, -1],
             "score": [-1, -1, -1],
             "cores": [-1, -1, -1],
             "memory": [-1, -1, -1],
             "frequency": [-1, -1, -1],
             "boardType": "U",
+            "memoryPerCard": 0,
+            "boardCount": [-1, -1, -1],
         },
         "memory": {
             "expertise": "component",
             "required": False,
             "rating": [-1, -1, -1],
             "size": [-1, -1, -1],
         },
@@ -171,14 +173,15 @@
         if type(resource.gpu) is bool:
             nb_config["graphics"]["cores"] = [1 if resource.gpu else -1, -1, -1]
         elif type(resource.gpu) is str:
             nb_config["graphics"]["cores"] = [1, -1, -1]
             nb_config["graphics"]["boardType"] = resource.gpu
 
         nb_config["graphics"]["memoryPerCard"] = resource.memory_per_gpu
+        nb_config["graphics"]["boardCount"] = [-1, -1, -1] if resource.num_gpus == 0 else [resource.num_gpus, resource.num_gpus, resource.num_gpus]
 
         check_providers(resource.providers)
         nb_config["providers"] = [provider.name for provider in resource.providers]
 
     # Plug in requirements
     if notifications != None:
         nb_config["notifications"] = {
```

### Comparing `optumi-api-3.15.7/optumi_api/Notifications.py` & `optumi-api-3.15.8/optumi_api/Notifications.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Packages.py` & `optumi-api-3.15.8/optumi_api/Packages.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Program.py` & `optumi-api-3.15.8/optumi_api/Program.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Provider.py` & `optumi-api-3.15.8/optumi_api/Provider.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Providers.py` & `optumi-api-3.15.8/optumi_api/Providers.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Resource.py` & `optumi-api-3.15.8/optumi_api/Resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,21 +15,22 @@
     OptumiException,
 )
 
 
 class Resource:
     """A class for creating resource specifications to be used when running scripts, notebooks or containers."""
 
-    def __init__(self, providers: Union[List[str], List[Provider]] = [], gpu: Union[bool, str] = True, memory_per_gpu: int = 0):
+    def __init__(self, providers: Union[List[str], List[Provider]] = [], gpu: Union[bool, str] = True, memory_per_gpu: int = 0, num_gpus: int = 0):
         """Constructor for the Resource class.
 
         Args:
             providers (list of str or list of Provider): The providers that can be used. Defaults to [], which means any provider can be used.
             gpu (bool or str): The type of graphics card to be used, either True to allow any graphics card, or a specific string value representing one of the types in gpus(). Default is True.
             memory_per_gpu (int): Memory allocated per graphics card. Default is 0.
+            num_gpus (int): The number of gpu cards. Defaults 1 gpu is specified, otherwise 0.
 
         Raises:
             OptumiException: Raised if an unsupported GPU card is specified.
         """
         if type(gpu) is str and not gpu.lower() in [x.lower() for x in Server.gpus()]:
             gpus = Server.gpus()
             if len(gpus) == 0:
@@ -45,14 +46,15 @@
             if type(provider) is Provider:
                 self._providers.append(provider)
             else:
                 self._providers.append(Provider(provider))
 
         self._gpu = gpu
         self._memory_per_gpu = memory_per_gpu
+        self._num_gpus = 1 if num_gpus == 0 and gpu else num_gpus
 
     @property
     def providers(self):
         """Obtain the list of the providers that can be used.
 
         Returns:
             list of Provider: The list of providers that can be used. Defaults to [], which means any provider.
@@ -69,13 +71,22 @@
         return self._gpu
 
     @property
     def memory_per_gpu(self):
         """Obtain the memory required per graphics card.
 
         Returns:
-            int: the memory required per graphics card, specified in GB.
+            int: The memory required per graphics card, specified in GB.
         """
         return self._memory_per_gpu
 
+    @property
+    def num_gpus(self):
+        """Obtain the number of gpu cards.
+
+        Returns:
+            int: The number of gpu cards.
+        """
+        return self._num_gpus
+
     def __str__(self):
         return "gpu=" + str(self.gpu)
```

### Comparing `optumi-api-3.15.7/optumi_api/Script.py` & `optumi-api-3.15.8/optumi_api/Script.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Server.py` & `optumi-api-3.15.8/optumi_api/Server.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Summary.py` & `optumi-api-3.15.8/optumi_api/Summary.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/Workload.py` & `optumi-api-3.15.8/optumi_api/Workload.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,37 +408,42 @@
         if Workload.__message(self._initializing_lines) != "":
             message = Workload.__message(self._initializing_lines)
         if Workload.__message(self._preparing_lines) != "":
             message = Workload.__message(self._preparing_lines)
         if Workload.__message(self._running_lines) != "":
             message = Workload.__message(self._running_lines)
 
-        failed_message = "Failed"
+        return message
+
+    @property
+    def error(self):
+        """Obtain wether this workload encountered an error.
+
+        Returns:
+            bool: Wether this workload encountered an error.
+        """
+        self._refresh()
 
         for update in self._initializing_lines:
             if Workload.__is_error(update):
-                message = failed_message
-            break
+                return True
 
         for update in self._preparing_lines:
             if Workload.__is_error(update):
-                message = failed_message
-            break
+                return True
 
         for update in self._running_lines:
             if Workload.__is_error(update):
-                message = failed_message
-            break
+                return True
 
         for update in self._update_lines:
             if update[1] == "error":
-                message = failed_message
-                break
+                return True
 
-        return message
+        return False
 
     @classmethod
     def __is_error(cls, update: Tuple[str, str]):
         line = update[0]
         modifier = update[1]
         if line == "error":
             return True
```

### Comparing `optumi-api-3.15.7/optumi_api/Workloads.py` & `optumi-api-3.15.8/optumi_api/Workloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         Returns:
             Workload: The Workload object representing the current workload running on an Optumi dynamic machine.
 
         Raises:
             OptumiException: Raised if this method is not called on a machine that was dynamically allocated by Optumi.
         """
-        if not os.environ["OPTUMI_MOD"]:
+        if not "OPTUMI_MOD" in os.environ:
             raise OptumiException("Workloads.current() only supported on Optumi dynamic machines.")
 
         user_information = json.loads(optumi.core.get_user_information(True).text)
 
         # Add apps from user information if they don't already exist
         if "jobs" in user_information:
             for app_map in user_information["jobs"]:
```

### Comparing `optumi-api-3.15.7/optumi_api/__init__.py` & `optumi-api-3.15.8/optumi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/api.py` & `optumi-api-3.15.8/optumi_api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,7 +287,20 @@
     if get_phone_number():
         try:
             optumi.core.send_notification("From " + str(Workloads.current()) + ": " + message if details and optumi.utils.is_dynamic() else message)
         except:
             optumi.core.send_notification(message)
     else:
         print("Unable to send notification - no phone number specified")
+
+
+
+def get_workload_limit():
+    """Obtain the current workload limit.
+
+    The workload limit is the maximum number of workloads that can be running in parallel.
+
+    Returns:
+        The workload limit as an integer.
+    """
+    res = optumi.core.get_user_information(False)
+    return int(json.loads(optumi.core.get_user_information(False).text)["maxJobs"])
```

### Comparing `optumi-api-3.15.7/optumi_api/cli.py` & `optumi-api-3.15.8/optumi_api/cli.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/optumi_api/utils.py` & `optumi-api-3.15.8/optumi_api/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,27 @@
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at https://www.optumi.com.
 ##
 
 import re, copy
 
 from typing import List, Tuple
 
+from contextlib import contextmanager
+import sys, os
+
+@contextmanager
+def suppress_stdout():
+    with open(os.devnull, "w") as devnull:
+        old_stdout = sys.stdout
+        sys.stdout = devnull
+        try:  
+            yield
+        finally:
+            sys.stdout = old_stdout
+
 
 # Remove characters that are overwritten by newline characters
 def fixCarriageReturn(txt: str):
     txt = re.compile(r"\r+\n", re.M).sub("\n", txt)  # \r followed by \n --> newline
     while not re.search(r"\r[^$]", txt) is None:
         base = re.compile(r"^(.*)\r+", re.M).match(txt)[1]
         insert = re.compile(r"\r+(.*)$", re.M).match(txt)[1]
```

### Comparing `optumi-api-3.15.7/optumi_api.egg-info/PKG-INFO` & `optumi-api-3.15.8/optumi_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.7
+Version: 3.15.8
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.7/optumi_api.egg-info/SOURCES.txt` & `optumi-api-3.15.8/optumi_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.7/setup.py` & `optumi-api-3.15.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     author="Optumi Inc Authors",
     author_email="cs@optumi.com",
     description="Optumi api library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"console_scripts": ["optumi = optumi_api.cli:main"]},
-    install_requires=["optumi_core" + core_dependency_string, "phonenumbers", "pwinput"],
+    install_requires=["optumi_core" + core_dependency_string, "phonenumbers", "pwinput", "tornado", "requests==2.28", "python-dateutil"],
     zip_safe=False,
     python_requires=">=3.7",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Optumi"],
     classifiers=[
         "License :: Other/Proprietary License",
         "Development Status :: 4 - Beta",
```

