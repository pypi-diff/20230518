# Comparing `tmp/stackoperator-0.0.3.tar.gz` & `tmp/stackoperator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackoperator-0.0.3.tar", last modified: Thu May 18 11:48:00 2023, max compression
+gzip compressed data, was "stackoperator-0.1.0.tar", last modified: Thu May 18 12:24:48 2023, max compression
```

## Comparing `stackoperator-0.0.3.tar` & `stackoperator-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wsl       (1000) wsl       (1000)        0 2023-05-18 11:48:00.045963 stackoperator-0.0.3/
--rw-r--r--   0 wsl       (1000) wsl       (1000)     1493 2023-05-18 11:48:00.045171 stackoperator-0.0.3/PKG-INFO
--rw-r--r--   0 wsl       (1000) wsl       (1000)     1035 2023-05-18 11:21:28.000000 stackoperator-0.0.3/README.md
--rw-r--r--   0 wsl       (1000) wsl       (1000)      863 2023-05-18 11:43:27.000000 stackoperator-0.0.3/pyproject.toml
--rw-r--r--   0 wsl       (1000) wsl       (1000)       38 2023-05-18 11:48:00.045963 stackoperator-0.0.3/setup.cfg
-drwxr-xr-x   0 wsl       (1000) wsl       (1000)        0 2023-05-18 11:47:59.982802 stackoperator-0.0.3/src/
-drwxr-xr-x   0 wsl       (1000) wsl       (1000)        0 2023-05-18 11:48:00.031184 stackoperator-0.0.3/src/stackoperator/
--rw-r--r--   0 wsl       (1000) wsl       (1000)     4358 2023-05-18 11:43:37.000000 stackoperator-0.0.3/src/stackoperator/__init__.py
--rwxr--r--   0 wsl       (1000) wsl       (1000)     5132 2023-05-17 19:04:02.000000 stackoperator-0.0.3/src/stackoperator/batchOperator.py
--rw-r--r--   0 wsl       (1000) wsl       (1000)     3883 2023-05-18 04:20:40.000000 stackoperator-0.0.3/src/stackoperator/cfnReader.py
--rw-r--r--   0 wsl       (1000) wsl       (1000)      555 2023-05-17 16:40:50.000000 stackoperator-0.0.3/src/stackoperator/readerFactory.py
--rw-r--r--   0 wsl       (1000) wsl       (1000)     4117 2023-05-18 05:08:04.000000 stackoperator-0.0.3/src/stackoperator/tfReader.py
-drwxr-xr-x   0 wsl       (1000) wsl       (1000)        0 2023-05-18 11:48:00.043960 stackoperator-0.0.3/src/stackoperator.egg-info/
--rw-r--r--   0 wsl       (1000) wsl       (1000)     1493 2023-05-18 11:47:59.000000 stackoperator-0.0.3/src/stackoperator.egg-info/PKG-INFO
--rw-r--r--   0 wsl       (1000) wsl       (1000)      433 2023-05-18 11:47:59.000000 stackoperator-0.0.3/src/stackoperator.egg-info/SOURCES.txt
--rw-r--r--   0 wsl       (1000) wsl       (1000)        1 2023-05-18 11:47:59.000000 stackoperator-0.0.3/src/stackoperator.egg-info/dependency_links.txt
--rw-r--r--   0 wsl       (1000) wsl       (1000)      270 2023-05-18 11:47:59.000000 stackoperator-0.0.3/src/stackoperator.egg-info/entry_points.txt
--rw-r--r--   0 wsl       (1000) wsl       (1000)        6 2023-05-18 11:47:59.000000 stackoperator-0.0.3/src/stackoperator.egg-info/requires.txt
--rw-r--r--   0 wsl       (1000) wsl       (1000)       14 2023-05-18 11:47:59.000000 stackoperator-0.0.3/src/stackoperator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:24:48.078816 stackoperator-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-18 12:24:48.078816 stackoperator-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-18 12:24:39.000000 stackoperator-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 12:24:39.000000 stackoperator-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:24:48.078816 stackoperator-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:24:48.074815 stackoperator-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:24:48.078816 stackoperator-0.1.0/src/stackoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-18 12:24:39.000000 stackoperator-0.1.0/src/stackoperator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5132 2023-05-18 12:24:39.000000 stackoperator-0.1.0/src/stackoperator/batchOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-18 12:24:39.000000 stackoperator-0.1.0/src/stackoperator/cfnReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-18 12:24:39.000000 stackoperator-0.1.0/src/stackoperator/readerFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-18 12:24:39.000000 stackoperator-0.1.0/src/stackoperator/tfReader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:24:48.078816 stackoperator-0.1.0/src/stackoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-18 12:24:48.000000 stackoperator-0.1.0/src/stackoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-18 12:24:48.000000 stackoperator-0.1.0/src/stackoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:24:48.000000 stackoperator-0.1.0/src/stackoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-18 12:24:48.000000 stackoperator-0.1.0/src/stackoperator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 12:24:48.000000 stackoperator-0.1.0/src/stackoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 12:24:48.000000 stackoperator-0.1.0/src/stackoperator.egg-info/top_level.txt
```

### Comparing `stackoperator-0.0.3/PKG-INFO` & `stackoperator-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackoperator
-Version: 0.0.3
+Version: 0.1.0
 Summary: A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.
 Author-email: Henry Huo <happy78@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `stackoperator-0.0.3/README.md` & `stackoperator-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stackoperator-0.0.3/pyproject.toml` & `stackoperator-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stackoperator"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
     {name = "Henry Huo", email = "happy78@live.com"},
 ]
 description = "A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `stackoperator-0.0.3/src/stackoperator/__init__.py` & `stackoperator-0.1.0/src/stackoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `stackoperator-0.0.3/src/stackoperator/batchOperator.py` & `stackoperator-0.1.0/src/stackoperator/batchOperator.py`

 * *Files identical despite different names*

### Comparing `stackoperator-0.0.3/src/stackoperator/cfnReader.py` & `stackoperator-0.1.0/src/stackoperator/cfnReader.py`

 * *Files identical despite different names*

### Comparing `stackoperator-0.0.3/src/stackoperator/readerFactory.py` & `stackoperator-0.1.0/src/stackoperator/readerFactory.py`

 * *Files identical despite different names*

### Comparing `stackoperator-0.0.3/src/stackoperator/tfReader.py` & `stackoperator-0.1.0/src/stackoperator/tfReader.py`

 * *Files identical despite different names*

### Comparing `stackoperator-0.0.3/src/stackoperator.egg-info/PKG-INFO` & `stackoperator-0.1.0/src/stackoperator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackoperator
-Version: 0.0.3
+Version: 0.1.0
 Summary: A small utility to help do start, stop and tag actions in an IaC stack for cost optimization purpose.
 Author-email: Henry Huo <happy78@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

