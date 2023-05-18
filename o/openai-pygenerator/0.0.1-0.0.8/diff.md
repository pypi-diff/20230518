# Comparing `tmp/openai_pygenerator-0.0.1.tar.gz` & `tmp/openai_pygenerator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_pygenerator-0.0.1.tar", last modified: Wed May 17 14:20:16 2023, max compression
+gzip compressed data, was "openai_pygenerator-0.0.8.tar", last modified: Thu May 18 08:42:24 2023, max compression
```

## Comparing `openai_pygenerator-0.0.1.tar` & `openai_pygenerator-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.787457 openai_pygenerator-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-17 14:20:16.787457 openai_pygenerator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 14:20:04.000000 openai_pygenerator-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-17 14:20:04.000000 openai_pygenerator-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:20:16.791457 openai_pygenerator-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.787457 openai_pygenerator-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:04.000000 openai_pygenerator-0.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.787457 openai_pygenerator-0.0.1/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:04.000000 openai_pygenerator-0.0.1/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-17 14:20:04.000000 openai_pygenerator-0.0.1/src/openai_pygenerator/gpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.787457 openai_pygenerator-0.0.1/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-17 14:20:16.000000 openai_pygenerator-0.0.1/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-17 14:20:16.000000 openai_pygenerator-0.0.1/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:20:16.000000 openai_pygenerator-0.0.1/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 14:20:16.000000 openai_pygenerator-0.0.1/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:20:16.787457 openai_pygenerator-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-17 14:20:04.000000 openai_pygenerator-0.0.1/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.814310 openai_pygenerator-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/tests/test_gpt.py
```

### Comparing `openai_pygenerator-0.0.1/PKG-INFO` & `openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: openai_pygenerator
-Version: 0.0.1
+Name: openai-pygenerator
+Version: 0.0.8
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # openai-pygenerator
 
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
```

### Comparing `openai_pygenerator-0.0.1/pyproject.toml` & `openai_pygenerator-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0", "openai>=0.27"]
+requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2", "openai>=0.27"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+write_to = "src/version.py"
+
 [project]
 name = "openai_pygenerator"
-version = "0.0.1"
+dynamic = ["version"]
+
 authors = [
   { name="Steve Phelps", email="sphelps@sphelps.net" },
 ]
 description = "Simple generator wrapper for OpenAI Python API with retry"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `openai_pygenerator-0.0.1/src/openai_pygenerator/gpt.py` & `openai_pygenerator-0.0.8/src/openai_pygenerator.py`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.1/src/openai_pygenerator.egg-info/PKG-INFO` & `openai_pygenerator-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: openai-pygenerator
-Version: 0.0.1
+Name: openai_pygenerator
+Version: 0.0.8
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # openai-pygenerator
 
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
```

### Comparing `openai_pygenerator-0.0.1/tests/test_gpt.py` & `openai_pygenerator-0.0.8/tests/test_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable
 
 import pytest
 from openai.error import APIError, RateLimitError
 from openai.openai_object import OpenAIObject
 
-from src.openai_pygenerator.gpt import GPT_MAX_RETRIES, generate_completions
+from src.openai_pygenerator import GPT_MAX_RETRIES, generate_completions
 
 
 def aio(text: str) -> OpenAIObject:
     result = OpenAIObject()
     result["message"] = text
     return result
```

