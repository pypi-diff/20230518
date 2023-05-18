# Comparing `tmp/openai_pygenerator-0.0.8.tar.gz` & `tmp/openai_pygenerator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_pygenerator-0.0.8.tar", last modified: Thu May 18 08:42:24 2023, max compression
+gzip compressed data, was "openai_pygenerator-0.0.9.tar", last modified: Thu May 18 09:12:12 2023, max compression
```

## Comparing `openai_pygenerator-0.0.8.tar` & `openai_pygenerator-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.814310 openai_pygenerator-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 08:42:24.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/src/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:42:24.818311 openai_pygenerator-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-18 08:42:10.000000 openai_pygenerator-0.0.8/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.925755 openai_pygenerator-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:12:12.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/src/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:12:12.929755 openai_pygenerator-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-18 09:11:53.000000 openai_pygenerator-0.0.9/tests/test_gpt.py
```

### Comparing `openai_pygenerator-0.0.8/.github/workflows/python-package.yml` & `openai_pygenerator-0.0.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.8/.github/workflows/python-publish.yml` & `openai_pygenerator-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.8/LICENSE.txt` & `openai_pygenerator-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.8/PKG-INFO` & `openai_pygenerator-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_pygenerator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_pygenerator-0.0.8/pyproject.toml` & `openai_pygenerator-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.8/src/openai_pygenerator.egg-info/PKG-INFO` & `openai_pygenerator-0.0.9/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_pygenerator-0.0.8/src/openai_pygenerator.py` & `openai_pygenerator-0.0.9/src/openai_pygenerator.py`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.0.8/tests/test_gpt.py` & `openai_pygenerator-0.0.9/tests/test_gpt.py`

 * *Files identical despite different names*

