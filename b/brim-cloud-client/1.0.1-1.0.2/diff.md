# Comparing `tmp/brim_cloud_client-1.0.1.tar.gz` & `tmp/brim_cloud_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brim_cloud_client-1.0.1.tar", last modified: Thu May  4 00:03:32 2023, max compression
+gzip compressed data, was "brim_cloud_client-1.0.2.tar", last modified: Thu May 18 16:46:54 2023, max compression
```

## Comparing `brim_cloud_client-1.0.1.tar` & `brim_cloud_client-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.022728 brim_cloud_client-1.0.1/
--rw-rw-r--   0 lance     (1001) lance     (1001)    35149 2023-05-03 22:18:27.000000 brim_cloud_client-1.0.1/LICENSE
--rw-rw-r--   0 lance     (1001) lance     (1001)     1108 2023-05-04 00:03:32.018728 brim_cloud_client-1.0.1/PKG-INFO
--rw-rw-r--   0 lance     (1001) lance     (1001)      546 2023-05-03 23:35:48.000000 brim_cloud_client-1.0.1/README.md
--rw-rw-r--   0 lance     (1001) lance     (1001)      635 2023-05-04 00:03:24.000000 brim_cloud_client-1.0.1/pyproject.toml
--rw-rw-r--   0 lance     (1001) lance     (1001)       38 2023-05-04 00:03:32.022728 brim_cloud_client-1.0.1/setup.cfg
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.006728 brim_cloud_client-1.0.1/src/
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.014727 brim_cloud_client-1.0.1/src/brim_cloud_client/
--rw-rw-r--   0 lance     (1001) lance     (1001)     2094 2023-05-04 00:03:06.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/BRIM.py
--rw-rw-r--   0 lance     (1001) lance     (1001)        0 2023-05-03 23:32:45.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/__init__.py
--rw-rw-r--   0 lance     (1001) lance     (1001)     1665 2023-05-03 23:25:17.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/loader.py
--rw-rw-r--   0 lance     (1001) lance     (1001)      254 2023-05-03 23:27:16.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/test.py
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.018728 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/
--rw-rw-r--   0 lance     (1001) lance     (1001)     1108 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/PKG-INFO
--rw-rw-r--   0 lance     (1001) lance     (1001)      338 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/SOURCES.txt
--rw-rw-r--   0 lance     (1001) lance     (1001)        1 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/dependency_links.txt
--rw-rw-r--   0 lance     (1001) lance     (1001)       18 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/top_level.txt
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-18 16:46:54.046495 brim_cloud_client-1.0.2/
+-rw-rw-r--   0 lance     (1001) lance     (1001)    35149 2023-05-04 00:13:19.000000 brim_cloud_client-1.0.2/LICENSE
+-rw-rw-r--   0 lance     (1001) lance     (1001)     1216 2023-05-18 16:46:54.042494 brim_cloud_client-1.0.2/PKG-INFO
+-rw-rw-r--   0 lance     (1001) lance     (1001)      654 2023-05-04 00:47:16.000000 brim_cloud_client-1.0.2/README.md
+-rw-rw-r--   0 lance     (1001) lance     (1001)      635 2023-05-18 16:46:29.000000 brim_cloud_client-1.0.2/pyproject.toml
+-rw-rw-r--   0 lance     (1001) lance     (1001)       38 2023-05-18 16:46:54.046495 brim_cloud_client-1.0.2/setup.cfg
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-18 16:46:54.026494 brim_cloud_client-1.0.2/src/
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-18 16:46:54.038494 brim_cloud_client-1.0.2/src/brim_cloud_client/
+-rw-rw-r--   0 lance     (1001) lance     (1001)     3689 2023-05-18 02:10:31.000000 brim_cloud_client-1.0.2/src/brim_cloud_client/BRIM.py
+-rw-rw-r--   0 lance     (1001) lance     (1001)        0 2023-05-04 00:13:19.000000 brim_cloud_client-1.0.2/src/brim_cloud_client/__init__.py
+-rw-rw-r--   0 lance     (1001) lance     (1001)     1665 2023-05-04 00:13:19.000000 brim_cloud_client-1.0.2/src/brim_cloud_client/loader.py
+-rw-rw-r--   0 lance     (1001) lance     (1001)      314 2023-05-18 02:34:40.000000 brim_cloud_client-1.0.2/src/brim_cloud_client/test.py
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-18 16:46:54.042494 brim_cloud_client-1.0.2/src/brim_cloud_client.egg-info/
+-rw-rw-r--   0 lance     (1001) lance     (1001)     1216 2023-05-18 16:46:54.000000 brim_cloud_client-1.0.2/src/brim_cloud_client.egg-info/PKG-INFO
+-rw-rw-r--   0 lance     (1001) lance     (1001)      338 2023-05-18 16:46:54.000000 brim_cloud_client-1.0.2/src/brim_cloud_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 lance     (1001) lance     (1001)        1 2023-05-18 16:46:54.000000 brim_cloud_client-1.0.2/src/brim_cloud_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 lance     (1001) lance     (1001)       18 2023-05-18 16:46:54.000000 brim_cloud_client-1.0.2/src/brim_cloud_client.egg-info/top_level.txt
```

### Comparing `brim_cloud_client-1.0.1/LICENSE` & `brim_cloud_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brim_cloud_client-1.0.1/PKG-INFO` & `brim_cloud_client-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: brim_cloud_client
-Version: 1.0.1
+Version: 1.0.2
 Summary: BRIM cloud client
 Author-email: Lance1o7 <10292888+Lance1o7@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Lance1o7/brim-cloud-client
 Project-URL: Bug Tracker, https://github.com/Lance1o7/brim-cloud-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # brim-cloud-client
 
+[![PyPI version](https://badge.fury.io/py/brim-cloud-client.svg)](https://badge.fury.io/py/brim-cloud-client)
+
 BRIM Cloud Client is a minimal implementation of the REST interface used
 to communicate with BRIM servers.
 
 ## Quick start
 
 ### Installation
 
 ```bash
 pip install brim-cloud-client
 ```
 
 ### Usage - Solve a CNF file
 
 ```python
-from BRIM import TMB
-
+from brim_cloud_client.BRIM import TMB
 
+# Set parameters
 tmb_client = TMB(cm=0.9, cb=0.6, p='tmb', Rc=31000, C=49e-15, anneal=0.00011, seed=0)
-tmb_client.print_neofetch() # print remote server information provided by neofetch
-state, status, results = tmb_client.solve('../example/cust-u500-01.cnf')
-print(state, status, results)
 
+# Submit cnf file to the server and wait for the results
+state, status, results = tmb_client.solve('cust-u500-01.cnf')
+print(state, status, results)
 ```
```

### Comparing `brim_cloud_client-1.0.1/README.md` & `brim_cloud_client-1.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # brim-cloud-client
 
+[![PyPI version](https://badge.fury.io/py/brim-cloud-client.svg)](https://badge.fury.io/py/brim-cloud-client)
+
 BRIM Cloud Client is a minimal implementation of the REST interface used
 to communicate with BRIM servers.
 
 ## Quick start
 
 ### Installation
 
 ```bash
 pip install brim-cloud-client
 ```
 
 ### Usage - Solve a CNF file
 
 ```python
-from BRIM import TMB
-
+from brim_cloud_client.BRIM import TMB
 
+# Set parameters
 tmb_client = TMB(cm=0.9, cb=0.6, p='tmb', Rc=31000, C=49e-15, anneal=0.00011, seed=0)
-tmb_client.print_neofetch() # print remote server information provided by neofetch
-state, status, results = tmb_client.solve('../example/cust-u500-01.cnf')
-print(state, status, results)
 
+# Submit cnf file to the server and wait for the results
+state, status, results = tmb_client.solve('cust-u500-01.cnf')
+print(state, status, results)
 ```
```

### Comparing `brim_cloud_client-1.0.1/pyproject.toml` & `brim_cloud_client-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brim_cloud_client"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Lance1o7", email="10292888+Lance1o7@users.noreply.github.com" },
 ]
 description = "BRIM cloud client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `brim_cloud_client-1.0.1/src/brim_cloud_client/loader.py` & `brim_cloud_client-1.0.2/src/brim_cloud_client/loader.py`

 * *Files identical despite different names*

