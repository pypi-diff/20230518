# Comparing `tmp/NREL-gaps-0.3.1.tar.gz` & `tmp/NREL-gaps-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-gaps-0.3.1.tar", last modified: Thu Apr 27 16:42:35 2023, max compression
+gzip compressed data, was "NREL-gaps-0.3.2.tar", last modified: Thu May 18 02:11:49 2023, max compression
```

## Comparing `NREL-gaps-0.3.1.tar` & `NREL-gaps-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:42:35.912321 NREL-gaps-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:42:35.908321 NREL-gaps-0.3.1/NREL_gaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-27 16:42:35.000000 NREL-gaps-0.3.1/NREL_gaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-27 16:42:35.000000 NREL-gaps-0.3.1/NREL_gaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:42:35.000000 NREL-gaps-0.3.1/NREL_gaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:42:35.000000 NREL-gaps-0.3.1/NREL_gaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 16:42:35.000000 NREL-gaps-0.3.1/NREL_gaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 16:42:35.000000 NREL-gaps-0.3.1/NREL_gaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-27 16:42:35.912321 NREL-gaps-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:42:35.908321 NREL-gaps-0.3.1/gaps/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:42:35.912321 NREL-gaps-0.3.1/gaps/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/project_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/gaps/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:42:35.912321 NREL-gaps-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-27 16:42:22.000000 NREL-gaps-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.411793 NREL-gaps-0.3.2/NREL_gaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 02:11:49.000000 NREL-gaps-0.3.2/NREL_gaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.415794 NREL-gaps-0.3.2/gaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/gaps/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/project_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/gaps/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:11:49.419793 NREL-gaps-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-18 02:11:37.000000 NREL-gaps-0.3.2/setup.py
```

### Comparing `NREL-gaps-0.3.1/LICENSE` & `NREL-gaps-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/NREL_gaps.egg-info/PKG-INFO` & `NREL-gaps-0.3.2/NREL_gaps.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.3.1
+Version: 0.3.2
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 ================================================
 Welcome to Geospatial Analysis Pipelines (GAPs)!
 ================================================
 
+.. image:: https://github.com/NREL/gaps/workflows/Documentation/badge.svg
+    :target: https://nrel.github.io/gaps/
 
 .. image:: https://github.com/NREL/gaps/workflows/Pytests/badge.svg
     :target: https://github.com/NREL/gaps/actions?query=workflow%3A%22Pytests%22
 
 .. image:: https://github.com/NREL/gaps/workflows/Lint%20Code%20Base/badge.svg
     :target: https://github.com/NREL/gaps/actions?query=workflow%3A%22Lint+Code+Base%22
 
@@ -51,14 +53,17 @@
 over a large geospatial extent (e.g. CONUS) across many parallel
 HPC nodes. Born from the open-source `reV <https://github.com/NREL/reV>`_ model, GAPs is a
 robust and easy-to-use engine that provides a rich set of features
 such as configuration file generation, job status monitoring,
 CLI Documentation, and more.
 
 
+To get started, take a look at the `documentation <https://nrel.github.io/gaps/>`_ (examples coming soon!)
+
+
 Installing gaps
 ===============
 
 NOTE: The installation instruction below assume that you have python installed
 on your machine and are using `conda <https://docs.conda.io/en/latest/index.html>`_
 as your package/environment manager.
 
@@ -85,10 +90,12 @@
 `black <https://black.readthedocs.io/en/stable/index.html>`_ to format it (check out the
 `black formatting style <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_).
 If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
 
 
 Acknowledgments
 ===============
+.. inclusion-ack
+
 Paul Pinchuk and Grant Buster. Geospatial Analysis Pipelines. 2023. https://doi.org/10.11578/dc.20230426.7
 
 The authors of this code would like to thank ExxonMobil Corporation for their contributions to this effort.
```

### Comparing `NREL-gaps-0.3.1/NREL_gaps.egg-info/SOURCES.txt` & `NREL-gaps-0.3.2/NREL_gaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/PKG-INFO` & `NREL-gaps-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.3.1
+Version: 0.3.2
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,16 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 ================================================
 Welcome to Geospatial Analysis Pipelines (GAPs)!
 ================================================
 
+.. image:: https://github.com/NREL/gaps/workflows/Documentation/badge.svg
+    :target: https://nrel.github.io/gaps/
 
 .. image:: https://github.com/NREL/gaps/workflows/Pytests/badge.svg
     :target: https://github.com/NREL/gaps/actions?query=workflow%3A%22Pytests%22
 
 .. image:: https://github.com/NREL/gaps/workflows/Lint%20Code%20Base/badge.svg
     :target: https://github.com/NREL/gaps/actions?query=workflow%3A%22Lint+Code+Base%22
 
@@ -51,14 +53,17 @@
 over a large geospatial extent (e.g. CONUS) across many parallel
 HPC nodes. Born from the open-source `reV <https://github.com/NREL/reV>`_ model, GAPs is a
 robust and easy-to-use engine that provides a rich set of features
 such as configuration file generation, job status monitoring,
 CLI Documentation, and more.
 
 
+To get started, take a look at the `documentation <https://nrel.github.io/gaps/>`_ (examples coming soon!)
+
+
 Installing gaps
 ===============
 
 NOTE: The installation instruction below assume that you have python installed
 on your machine and are using `conda <https://docs.conda.io/en/latest/index.html>`_
 as your package/environment manager.
 
@@ -85,10 +90,12 @@
 `black <https://black.readthedocs.io/en/stable/index.html>`_ to format it (check out the
 `black formatting style <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_).
 If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
 
 
 Acknowledgments
 ===============
+.. inclusion-ack
+
 Paul Pinchuk and Grant Buster. Geospatial Analysis Pipelines. 2023. https://doi.org/10.11578/dc.20230426.7
 
 The authors of this code would like to thank ExxonMobil Corporation for their contributions to this effort.
```

### Comparing `NREL-gaps-0.3.1/README.rst` & `NREL-gaps-0.3.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 ================================================
 Welcome to Geospatial Analysis Pipelines (GAPs)!
 ================================================
 
+.. image:: https://github.com/NREL/gaps/workflows/Documentation/badge.svg
+    :target: https://nrel.github.io/gaps/
 
 .. image:: https://github.com/NREL/gaps/workflows/Pytests/badge.svg
     :target: https://github.com/NREL/gaps/actions?query=workflow%3A%22Pytests%22
 
 .. image:: https://github.com/NREL/gaps/workflows/Lint%20Code%20Base/badge.svg
     :target: https://github.com/NREL/gaps/actions?query=workflow%3A%22Lint+Code+Base%22
 
@@ -29,14 +31,17 @@
 over a large geospatial extent (e.g. CONUS) across many parallel
 HPC nodes. Born from the open-source `reV <https://github.com/NREL/reV>`_ model, GAPs is a
 robust and easy-to-use engine that provides a rich set of features
 such as configuration file generation, job status monitoring,
 CLI Documentation, and more.
 
 
+To get started, take a look at the `documentation <https://nrel.github.io/gaps/>`_ (examples coming soon!)
+
+
 Installing gaps
 ===============
 
 NOTE: The installation instruction below assume that you have python installed
 on your machine and are using `conda <https://docs.conda.io/en/latest/index.html>`_
 as your package/environment manager.
 
@@ -63,10 +68,12 @@
 `black <https://black.readthedocs.io/en/stable/index.html>`_ to format it (check out the
 `black formatting style <https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html>`_).
 If you wish to contribute to this repository, your code will have to adhere to both of these guidelines and pass all existing tests.
 
 
 Acknowledgments
 ===============
+.. inclusion-ack
+
 Paul Pinchuk and Grant Buster. Geospatial Analysis Pipelines. 2023. https://doi.org/10.11578/dc.20230426.7
 
 The authors of this code would like to thank ExxonMobil Corporation for their contributions to this effort.
```

### Comparing `NREL-gaps-0.3.1/gaps/batch.py` & `NREL-gaps-0.3.2/gaps/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/batch.py` & `NREL-gaps-0.3.2/gaps/cli/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/cli.py` & `NREL-gaps-0.3.2/gaps/cli/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/collect.py` & `NREL-gaps-0.3.2/gaps/cli/collect.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/command.py` & `NREL-gaps-0.3.2/gaps/cli/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,19 +37,23 @@
 
     def __init__(
         self,
         name,
         add_collect=False,
         split_keys=None,
         config_preprocessor=None,
+        skip_doc_params=None,
     ):
         self.name = name
         self.add_collect = add_collect
         self.split_keys = set() if split_keys is None else set(split_keys)
         self.config_preprocessor = config_preprocessor or _passthrough
+        self.skip_doc_params = (
+            set() if skip_doc_params is None else set(skip_doc_params)
+        )
         preprocessor_sig = signature(self.config_preprocessor)
         self.preprocessor_args = preprocessor_sig.parameters.keys()
         self.preprocessor_defaults = {
             name: param.default
             for name, param in preprocessor_sig.parameters.items()
             if param.default != param.empty
         }
@@ -91,14 +95,15 @@
     def __init__(
         self,
         function,
         name=None,
         add_collect=False,
         split_keys=None,
         config_preprocessor=None,
+        skip_doc_params=None,
     ):
         """
 
         Parameters
         ----------
         function : callable
             The function to run on individual nodes. This function will
@@ -119,28 +124,30 @@
                 tag : str
                     Short string unique to this job run that can be used
                     to generate unique output filenames, thereby
                     avoiding clashing output files with jobs on other
                     nodes. This string  contains a leading underscore,
                     so the file name can easily be generated:
                     ``f"{out_file_name}{tag}.{extension}"``.
-                    See :func:`gaps.cli.collect.collect` for an example.
                 command_name : str
                     Name of the command being run. This is equivalent to
-                    the ``name`` input above.
+                    the ``name`` input argument.
                 config_file : Path
                     Path to the configuration file specified by the
                     user.
                 project_dir : Path
                     Path to the project directory (parent directory of
                     the configuration file).
                 job_name : str
                     Name of the job being run. This is typically a
-                    combination of the project directory and the command
-                    name.
+                    combination of the project directory, the command
+                    name, and a tag unique to a job. Note that the tag
+                    will not be included if you request this argument
+                    in a config preprocessing function, as the execution
+                    has not been split into multiple jobs by that point.
                 out_dir : Path
                     Path to output directory - typically equivalent to
                     the project directory.
 
             If your function is capable of multiprocessing, you should
             also include ``max_workers`` in the function signature.
             ``gaps`` will pass an integer equal to the number of
@@ -150,17 +157,20 @@
             keys/inputs directly. This function can also request
             "private" arguments by including a leading underscore in the
             argument name. These arguments are NOT exposed to users in
             the documentation or template configuration files. Instead,
             it is expected that the ``config_preprocessor`` function
             fills these arguments in programmatically before the
             function is distributed across nodes. See the implementation
-            of :func:`gaps.cli.preprocessing.preprocess_collect_config`
-            and :func:`gaps.cli.collect.collect` for an example of this
-            pattern.
+            of :func:`gaps.cli.collect.collect` and
+            :func:`gaps.cli.preprocessing.preprocess_collect_config`
+            for an example of this pattern. You can use the
+            ``skip_doc_params`` input below to achieve the same results
+            without the underscore syntax (helpful for public-facing
+            functions).
         name : str, optional
             Name of the command. This will be the name used to call the
             command on the terminal. This name does not have to match
             the function name. It is encouraged to use lowercase names
             with dashes ("-") instead of underscores ("_") to stay
             consistent with click's naming conventions. By default,
             ``None``, which uses the function name as the command name
@@ -252,30 +262,39 @@
             :func:`gaps.cli.preprocessing.preprocess_collect_config` and
             :func:`gaps.cli.collect.collect` for an example of this
             pattern. Do not request parameters with the same names as
             any of your model function (i.e. if ``res_file`` is a model
             parameter, do not request it in the preprocessing function
             docstring - extract it from the config dictionary instead).
             By default, ``None``.
+        skip_doc_params : iterable of str, optional
+            Optional iterable of parameter names that should be excluded
+            from the documentation/template configuration files. This
+            can be useful if your pre-processing function automatically
+            sets some parameters based on other user input. This option
+            is an alternative to the "private" arguments discussed in
+            the ``function`` parameter documentation above. By default,
+            ``None``.
         """
         super().__init__(
             name or function.__name__.strip("_").replace("_", "-"),
             add_collect,
             split_keys,
             config_preprocessor,
+            skip_doc_params,
         )
         self.runner = function
 
     @cached_property
     def documentation(self):
         """CommandDocumentation: Documentation object."""
         return CommandDocumentation(
             self.runner,
             self.config_preprocessor,
-            skip_params=GAPS_SUPPLIED_ARGS,
+            skip_params=GAPS_SUPPLIED_ARGS | self.skip_doc_params,
             is_split_spatially=self.is_split_spatially,
         )
 
 
 # pylint: disable=invalid-name,import-outside-toplevel
 def CLICommandConfiguration(
     name, function, split_keys=None, config_preprocessor=None
@@ -320,14 +339,15 @@
         self,
         init,
         method,
         name=None,
         add_collect=False,
         split_keys=None,
         config_preprocessor=None,
+        skip_doc_params=None,
     ):
         """
 
         Parameters
         ----------
         init : class initializer
             The class to be initialized and used to to run on individual
@@ -353,48 +373,53 @@
                 tag : str
                     Short string unique to this job run that can be used
                     to generate unique output filenames, thereby
                     avoiding clashing output files with jobs on other
                     nodes. This string  contains a leading underscore,
                     so the file name can easily be generated:
                     ``f"{out_file_name}{tag}.{extension}"``.
-                    See :func:`gaps.cli.collect.collect` for an example.
                 command_name : str
                     Name of the command being run. This is equivalent to
-                    the ``name`` input above.
+                    the ``name`` input argument.
                 config_file : Path
                     Path to the configuration file specified by the
                     user.
                 project_dir : Path
                     Path to the project directory (parent directory of
                     the configuration file).
                 job_name : str
                     Name of the job being run. This is typically a
-                    combination of the project directory and the command
-                    name.
+                    combination of the project directory, the command
+                    name, and a tag unique to a job. Note that the tag
+                    will not be included if you request this argument
+                    in a config preprocessing function, as the execution
+                    has not been split into multiple jobs by that point.
                 out_dir : Path
                     Path to output directory - typically equivalent to
                     the project directory.
 
-            If your method is capable of multiprocessing, you should
-            also include ``max_workers`` in the method signature.
+            If your function is capable of multiprocessing, you should
+            also include ``max_workers`` in the function signature.
             ``gaps`` will pass an integer equal to the number of
             processes the user wants to run on a single node for this
             value. Note that the ``config`` parameter is not allowed as
-            a method signature item. Please request all the required
-            keys/inputs directly. This method can also request
+            a function signature item. Please request all the required
+            keys/inputs directly. This function can also request
             "private" arguments by including a leading underscore in the
             argument name. These arguments are NOT exposed to users in
             the documentation or template configuration files. Instead,
             it is expected that the ``config_preprocessor`` function
             fills these arguments in programmatically before the
-            method is distributed across nodes. See the implementation
-            of :func:`gaps.cli.preprocessing.preprocess_collect_config`
-            and :func:`gaps.cli.collect.collect` for an example of this
-            pattern.
+            function is distributed across nodes. See the implementation
+            of :func:`gaps.cli.collect.collect` and
+            :func:`gaps.cli.preprocessing.preprocess_collect_config`
+            for an example of this pattern. You can use the
+            ``skip_doc_params`` input below to achieve the same results
+            without the underscore syntax (helpful for public-facing
+            functions).
         name : str, optional
             Name of the command. This will be the name used to call the
             command on the terminal. This name does not have to match
             the function name. It is encouraged to use lowercase names
             with dashes ("-") instead of underscores ("_") to stay
             consistent with click's naming conventions. By default,
             ``None``, which uses the ``method`` name (with minor
@@ -485,20 +510,29 @@
             :func:`gaps.cli.preprocessing.preprocess_collect_config` and
             :func:`gaps.cli.collect.collect` for an example of this
             pattern. Do not request parameters with the same names as
             any of your model function (i.e. if ``res_file`` is a model
             parameter, do not request it in the preprocessing function
             docstring - extract it from the config dictionary instead).
             By default, ``None``.
+        skip_doc_params : iterable of str, optional
+            Optional iterable of parameter names that should be excluded
+            from the documentation/template configuration files. This
+            can be useful if your pre-processing function automatically
+            sets some parameters based on other user input. This option
+            is an alternative to the "private" arguments discussed in
+            the ``function`` parameter documentation above. By default,
+            ``None``.
         """
         super().__init__(
             name or method.strip("_").replace("_", "-"),
             add_collect,
             split_keys,
             config_preprocessor,
+            skip_doc_params,
         )
         self.runner = init
         self.run_method = method
         self._validate_run_method_exists()
 
     def _validate_run_method_exists(self):
         """Validate that the ``run_method`` is implemented."""
@@ -507,15 +541,15 @@
     @cached_property
     def documentation(self):
         """CommandDocumentation: Documentation object."""
         return CommandDocumentation(
             self.runner,
             getattr(self.runner, self.run_method),
             self.config_preprocessor,
-            skip_params=GAPS_SUPPLIED_ARGS,
+            skip_params=GAPS_SUPPLIED_ARGS | self.skip_doc_params,
             is_split_spatially=self.is_split_spatially,
         )
 
 
 def _passthrough(config):
     """Pass the input config through with no modifications."""
     return config
```

### Comparing `NREL-gaps-0.3.1/gaps/cli/config.py` & `NREL-gaps-0.3.2/gaps/cli/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/documentation.py` & `NREL-gaps-0.3.2/gaps/cli/documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,15 @@
         :qos: (str) Quality-of-service specifier. By default, ``"normal"``.
         :memory: (int, optional) Node memory request in GB. Default is not to
                  specify.{n}{mw}
         :queue: (str, optional; PBS ONLY) HPC queue to submit job to.
                 Examples include: 'debug', 'short', 'batch', 'batch-h',
                 'long', etc. By default, `None`, which uses `test_queue`.
         :feature: (str, optional) Additional flags for SLURM job
-                  (e.g. "--qos=high", "-p debug", etc). Default is not
-                  to specify.
+                  (e.g. "-p debug"). Default is not to specify.
         :conda_env: (str, optional) Name of conda environment to activate.
                     Default is not to load any environments.
         :module: (str, optional) Module to load. Default is not to load any
                  modules.
         :sh_script: (str, optional) Extra shell script to run before
                     command call. Default is not to run any scripts.
```

### Comparing `NREL-gaps-0.3.1/gaps/cli/execution.py` & `NREL-gaps-0.3.2/gaps/cli/execution.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/pipeline.py` & `NREL-gaps-0.3.2/gaps/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/preprocessing.py` & `NREL-gaps-0.3.2/gaps/cli/preprocessing.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/status.py` & `NREL-gaps-0.3.2/gaps/cli/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/cli/templates.py` & `NREL-gaps-0.3.2/gaps/cli/templates.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/collection.py` & `NREL-gaps-0.3.2/gaps/collection.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/config.py` & `NREL-gaps-0.3.2/gaps/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/exceptions.py` & `NREL-gaps-0.3.2/gaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/hpc.py` & `NREL-gaps-0.3.2/gaps/hpc.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/legacy.py` & `NREL-gaps-0.3.2/gaps/legacy.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/log.py` & `NREL-gaps-0.3.2/gaps/log.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/pipeline.py` & `NREL-gaps-0.3.2/gaps/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/project_points.py` & `NREL-gaps-0.3.2/gaps/project_points.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/status.py` & `NREL-gaps-0.3.2/gaps/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/utilities.py` & `NREL-gaps-0.3.2/gaps/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/gaps/warnings.py` & `NREL-gaps-0.3.2/gaps/warnings.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.1/setup.py` & `NREL-gaps-0.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 
 DEV_REQUIREMENTS = ["black", "pylint", "jupyter", "pipreqs"]
 TEST_REQUIREMENTS = ["pytest", "pytest-cov", "h5py"]
 DOC_REQUIREMENTS = [
     "make",
     "ghp-import",
     "numpydoc",
-    "pandoc",
-    "sphinx_rtd_theme>=0.5.1",
+    "pandoc"
 ]
 DESCRIPTION = (
     "National Renewable Energy Laboratory's (NREL's) Geospatial Analysis "
     "Pipelines (GAPs) framework"
 )
```

