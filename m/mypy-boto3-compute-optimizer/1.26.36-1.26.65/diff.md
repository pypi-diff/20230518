# Comparing `tmp/mypy-boto3-compute-optimizer-1.26.36.tar.gz` & `tmp/mypy-boto3-compute-optimizer-1.26.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-compute-optimizer-1.26.36.tar", last modified: Thu Dec 22 20:32:39 2022, max compression
+gzip compressed data, was "mypy-boto3-compute-optimizer-1.26.65.tar", last modified: Mon Feb  6 20:47:28 2023, max compression
```

## Comparing `mypy-boto3-compute-optimizer-1.26.36.tar` & `mypy-boto3-compute-optimizer-1.26.65.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.104697 mypy-boto3-compute-optimizer-1.26.36/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2022-12-22 20:32:39.100698 mypy-boto3-compute-optimizer-1.26.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18597 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.100698 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24698 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22818 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40945 2022-12-22 20:32:12.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40922 2022-12-22 20:32:11.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 20:32:39.100698 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2022-12-22 20:32:38.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-22 20:32:38.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:32:38.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 20:32:38.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-22 20:32:38.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-22 20:32:38.000000 mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 20:32:39.104697 mypy-boto3-compute-optimizer-1.26.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2022-12-22 20:32:10.000000 mypy-boto3-compute-optimizer-1.26.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24698 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22921 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22919 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-02-06 20:47:03.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40922 2023-02-06 20:47:03.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-06 20:47:28.000000 mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 20:47:28.149984 mypy-boto3-compute-optimizer-1.26.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-02-06 20:47:02.000000 mypy-boto3-compute-optimizer-1.26.65/setup.py
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/LICENSE` & `mypy-boto3-compute-optimizer-1.26.65/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/PKG-INFO` & `mypy-boto3-compute-optimizer-1.26.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.26.36
-Summary: Type annotations for boto3.ComputeOptimizer 1.26.36 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.65
+Summary: Type annotations for boto3.ComputeOptimizer 1.26.65 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/README.md` & `mypy-boto3-compute-optimizer-1.26.65/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/__init__.py` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/__init__.pyi` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/__main__.py` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComputeOptimizer 1.26.36\nVersion:         1.26.36\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.ComputeOptimizer 1.26.65\nVersion:         1.26.65\nBuilder"
+        " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.36")
+    print("1.26.65")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/client.py` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/client.pyi` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/literals.py` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,22 @@
 GetEnrollmentStatusesForOrganizationPaginatorName = Literal[
     "get_enrollment_statuses_for_organization"
 ]
 GetLambdaFunctionRecommendationsPaginatorName = Literal["get_lambda_function_recommendations"]
 GetRecommendationPreferencesPaginatorName = Literal["get_recommendation_preferences"]
 GetRecommendationSummariesPaginatorName = Literal["get_recommendation_summaries"]
 InferredWorkloadTypeType = Literal[
-    "AmazonEmr", "ApacheCassandra", "ApacheHadoop", "Memcached", "Nginx", "PostgreSql", "Redis"
+    "AmazonEmr",
+    "ApacheCassandra",
+    "ApacheHadoop",
+    "Kafka",
+    "Memcached",
+    "Nginx",
+    "PostgreSql",
+    "Redis",
 ]
 InferredWorkloadTypesPreferenceType = Literal["Active", "Inactive"]
 InstanceRecommendationFindingReasonCodeType = Literal[
     "CPUOverprovisioned",
     "CPUUnderprovisioned",
     "DiskIOPSOverprovisioned",
     "DiskIOPSUnderprovisioned",
@@ -417,24 +424,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -542,14 +551,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/literals.pyi` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,22 @@
 GetEnrollmentStatusesForOrganizationPaginatorName = Literal[
     "get_enrollment_statuses_for_organization"
 ]
 GetLambdaFunctionRecommendationsPaginatorName = Literal["get_lambda_function_recommendations"]
 GetRecommendationPreferencesPaginatorName = Literal["get_recommendation_preferences"]
 GetRecommendationSummariesPaginatorName = Literal["get_recommendation_summaries"]
 InferredWorkloadTypeType = Literal[
-    "AmazonEmr", "ApacheCassandra", "ApacheHadoop", "Memcached", "Nginx", "PostgreSql", "Redis"
+    "AmazonEmr",
+    "ApacheCassandra",
+    "ApacheHadoop",
+    "Kafka",
+    "Memcached",
+    "Nginx",
+    "PostgreSql",
+    "Redis",
 ]
 InferredWorkloadTypesPreferenceType = Literal["Active", "Inactive"]
 InstanceRecommendationFindingReasonCodeType = Literal[
     "CPUOverprovisioned",
     "CPUUnderprovisioned",
     "DiskIOPSOverprovisioned",
     "DiskIOPSUnderprovisioned",
@@ -415,24 +422,26 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -540,14 +549,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/paginator.py` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/paginator.pyi` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/type_defs.py` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer/type_defs.pyi` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/PKG-INFO` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-compute-optimizer
-Version: 1.26.36
-Summary: Type annotations for boto3.ComputeOptimizer 1.26.36 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.65
+Summary: Type annotations for boto3.ComputeOptimizer 1.26.65 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-compute-optimizer.svg?color=blue)](https://pypi.org/project/mypy-boto3-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-compute-optimizer?color=blue)](https://pypistats.org/packages/mypy-boto3-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComputeOptimizer 1.26.36](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[boto3.ComputeOptimizer 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-compute-optimizer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-compute-optimizer-1.26.36/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt` & `mypy-boto3-compute-optimizer-1.26.65/mypy_boto3_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-compute-optimizer-1.26.36/setup.py` & `mypy-boto3-compute-optimizer-1.26.65/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-compute-optimizer",
-    version="1.26.36",
+    version="1.26.65",
     packages=["mypy_boto3_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComputeOptimizer 1.26.36 service generated with"
-        " mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.ComputeOptimizer 1.26.65 service generated with"
+        " mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

