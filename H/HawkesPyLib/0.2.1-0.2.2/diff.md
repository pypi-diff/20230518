# Comparing `tmp/HawkesPyLib-0.2.1.tar.gz` & `tmp/HawkesPyLib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawkesPyLib-0.2.1.tar", last modified: Sun Nov 20 18:57:16 2022, max compression
+gzip compressed data, was "HawkesPyLib-0.2.2.tar", last modified: Thu May 18 19:32:21 2023, max compression
```

## Comparing `HawkesPyLib-0.2.1.tar` & `HawkesPyLib-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 18:57:16.276419 HawkesPyLib-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3445 2022-11-20 18:57:16.276419 HawkesPyLib-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-20 18:57:16.276419 HawkesPyLib-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 18:57:16.272419 HawkesPyLib-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 18:57:16.276419 HawkesPyLib-0.2.1/src/HawkesPyLib/
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 18:57:16.276419 HawkesPyLib-0.2.1/src/HawkesPyLib/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/core/compensator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10911 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/core/intensity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3861 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/core/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    11926 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/core/logll.py
--rw-r--r--   0 runner    (1001) docker     (121)    12612 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/core/simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)    45610 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/inference.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19016 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/processes.py
--rw-r--r--   0 runner    (1001) docker     (121)    18420 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-11-20 18:57:05.000000 HawkesPyLib-0.2.1/src/HawkesPyLib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 18:57:16.276419 HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3445 2022-11-20 18:57:16.000000 HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-11-20 18:57:16.000000 HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 18:57:16.000000 HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-20 18:57:16.000000 HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-20 18:57:16.000000 HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:21.718678 HawkesPyLib-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-18 19:32:21.718678 HawkesPyLib-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:32:21.718678 HawkesPyLib-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:21.714677 HawkesPyLib-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:21.714677 HawkesPyLib-0.2.2/src/HawkesPyLib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:21.714677 HawkesPyLib-0.2.2/src/HawkesPyLib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/core/compensator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/core/intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/core/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/core/logll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/core/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45610 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19016 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/src/HawkesPyLib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:21.714677 HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-18 19:32:21.000000 HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-18 19:32:21.000000 HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:32:21.000000 HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-18 19:32:21.000000 HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 19:32:21.000000 HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:32:21.718678 HawkesPyLib-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_estim_approx_powlaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_estim_expo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_estim_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_estim_sum_expo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_logL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-05-18 19:32:09.000000 HawkesPyLib-0.2.2/tests/test_simulation.py
```

### Comparing `HawkesPyLib-0.2.1/LICENSE` & `HawkesPyLib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/PKG-INFO` & `HawkesPyLib-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: HawkesPyLib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for simulation and inference of Hawkes processes
 Author: Simon Grimm
 License: MIT
 Project-URL: Homepage, https://simbold.github.io/HawkesPyLib/
 Project-URL: Source, https://github.com/Simbold/HawkesPyLib
 Keywords: hawkes,hawkes-process,point-process
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `HawkesPyLib-0.2.1/README.md` & `HawkesPyLib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/pyproject.toml` & `HawkesPyLib-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HawkesPyLib"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python library for simulation and inference of Hawkes processes"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.8"
 authors = [
     { name = "Simon Grimm" },
 ]
@@ -22,14 +22,15 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research"
 ]
 dependencies = [
 
     "numba>=0.56",
     "numpy>=1.23",
```

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/__init__.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/__init__.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/core/compensator.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/core/compensator.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/core/intensity.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/core/intensity.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/core/kernel.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/core/kernel.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/core/logll.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/core/logll.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/core/simulation.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/core/simulation.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/inference.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/inference.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/processes.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/processes.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/simulation.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/simulation.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib/util.py` & `HawkesPyLib-0.2.2/src/HawkesPyLib/util.py`

 * *Files identical despite different names*

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/PKG-INFO` & `HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: HawkesPyLib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for simulation and inference of Hawkes processes
 Author: Simon Grimm
 License: MIT
 Project-URL: Homepage, https://simbold.github.io/HawkesPyLib/
 Project-URL: Source, https://github.com/Simbold/HawkesPyLib
 Keywords: hawkes,hawkes-process,point-process
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `HawkesPyLib-0.2.1/src/HawkesPyLib.egg-info/SOURCES.txt` & `HawkesPyLib-0.2.2/src/HawkesPyLib.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,17 @@
 src/HawkesPyLib.egg-info/requires.txt
 src/HawkesPyLib.egg-info/top_level.txt
 src/HawkesPyLib/core/__init__.py
 src/HawkesPyLib/core/compensator.py
 src/HawkesPyLib/core/intensity.py
 src/HawkesPyLib/core/kernel.py
 src/HawkesPyLib/core/logll.py
-src/HawkesPyLib/core/simulation.py
+src/HawkesPyLib/core/simulation.py
+tests/test_estim_approx_powlaw.py
+tests/test_estim_expo.py
+tests/test_estim_poisson.py
+tests/test_estim_sum_expo.py
+tests/test_intensity.py
+tests/test_kernel.py
+tests/test_logL.py
+tests/test_processes.py
+tests/test_simulation.py
```

