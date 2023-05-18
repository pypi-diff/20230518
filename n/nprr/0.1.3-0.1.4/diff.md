# Comparing `tmp/nprr-0.1.3.tar.gz` & `tmp/nprr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nprr-0.1.3.tar", last modified: Thu May 18 06:05:45 2023, max compression
+gzip compressed data, was "nprr-0.1.4.tar", last modified: Thu May 18 06:13:30 2023, max compression
```

## Comparing `nprr-0.1.3.tar` & `nprr-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:05:45.019311 nprr-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 06:05:37.000000 nprr-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-18 06:05:45.019311 nprr-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-18 06:05:37.000000 nprr-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:05:45.019311 nprr-0.1.3/nprr/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/cgf.py
--rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/dpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/mechanisms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 06:05:37.000000 nprr-0.1.3/nprr/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:05:45.019311 nprr-0.1.3/nprr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:05:44.000000 nprr-0.1.3/nprr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 06:05:45.000000 nprr-0.1.3/nprr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 06:05:37.000000 nprr-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:05:45.019311 nprr-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 06:05:37.000000 nprr-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:13:30.897881 nprr-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 06:13:23.000000 nprr-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-18 06:13:30.897881 nprr-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-18 06:13:23.000000 nprr-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:13:30.893881 nprr-0.1.4/nprr/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 06:13:23.000000 nprr-0.1.4/nprr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-18 06:13:23.000000 nprr-0.1.4/nprr/cgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-05-18 06:13:23.000000 nprr-0.1.4/nprr/dpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-18 06:13:23.000000 nprr-0.1.4/nprr/mechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-18 06:13:23.000000 nprr-0.1.4/nprr/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 06:13:23.000000 nprr-0.1.4/nprr/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:13:30.897881 nprr-0.1.4/nprr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-18 06:13:30.000000 nprr-0.1.4/nprr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 06:13:30.000000 nprr-0.1.4/nprr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:13:30.000000 nprr-0.1.4/nprr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:13:30.000000 nprr-0.1.4/nprr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 06:13:30.000000 nprr-0.1.4/nprr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 06:13:30.000000 nprr-0.1.4/nprr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 06:13:23.000000 nprr-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:13:30.897881 nprr-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 06:13:23.000000 nprr-0.1.4/setup.py
```

### Comparing `nprr-0.1.3/LICENSE` & `nprr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nprr-0.1.3/PKG-INFO` & `nprr-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: nprr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonparametric randomized response and locally private confidence sets
 Home-page: https://github.com/wannabesmith/nprr
 Author: Ian Waudby-Smith
 Author-email: iwaudbysmith@gmail.com
 License: BSD 3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NPRR: Nonparametric randomized response
 
 This code implements the nonparametric randomized response (NPRR) mechanism as well as methods for computing locally differentially private confidence intervals and sequences from NPRR's output. The methods are based on the paper ["A nonparametric extension of randomized response for private confidence sets"](https://arxiv.org/abs/2202.08728) by Ian Waudby-Smith, Zhiwei Steven Wu, and Aaditya Ramdas (2023).
 
 ## Installation
 
-*This won't work yet — we're going to put it on PyPi soon.*
-
-To install the package, run the following in a terminal: 
-
 ```sh
 pip install nprr
 ```
 
 ## Organization
 
 The package is organized into two main submodules:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nprr-0.1.3/README.md` & `nprr-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # NPRR: Nonparametric randomized response
 
 This code implements the nonparametric randomized response (NPRR) mechanism as well as methods for computing locally differentially private confidence intervals and sequences from NPRR's output. The methods are based on the paper ["A nonparametric extension of randomized response for private confidence sets"](https://arxiv.org/abs/2202.08728) by Ian Waudby-Smith, Zhiwei Steven Wu, and Aaditya Ramdas (2023).
 
 ## Installation
 
-*This won't work yet — we're going to put it on PyPi soon.*
-
-To install the package, run the following in a terminal: 
-
 ```sh
 pip install nprr
 ```
 
 ## Organization
 
 The package is organized into two main submodules:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nprr-0.1.3/nprr/cgf.py` & `nprr-0.1.4/nprr/cgf.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.3/nprr/dpcs.py` & `nprr-0.1.4/nprr/dpcs.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.3/nprr/mechanisms.py` & `nprr-0.1.4/nprr/mechanisms.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.3/nprr/plotting.py` & `nprr-0.1.4/nprr/plotting.py`

 * *Files identical despite different names*

### Comparing `nprr-0.1.3/nprr.egg-info/PKG-INFO` & `nprr-0.1.4/nprr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: nprr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonparametric randomized response and locally private confidence sets
 Home-page: https://github.com/wannabesmith/nprr
 Author: Ian Waudby-Smith
 Author-email: iwaudbysmith@gmail.com
 License: BSD 3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NPRR: Nonparametric randomized response
 
 This code implements the nonparametric randomized response (NPRR) mechanism as well as methods for computing locally differentially private confidence intervals and sequences from NPRR's output. The methods are based on the paper ["A nonparametric extension of randomized response for private confidence sets"](https://arxiv.org/abs/2202.08728) by Ian Waudby-Smith, Zhiwei Steven Wu, and Aaditya Ramdas (2023).
 
 ## Installation
 
-*This won't work yet — we're going to put it on PyPi soon.*
-
-To install the package, run the following in a terminal: 
-
 ```sh
 pip install nprr
 ```
 
 ## Organization
 
 The package is organized into two main submodules:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nprr-0.1.3/setup.py` & `nprr-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nprr",
-    version="0.1.3",
+    version="0.1.4",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Nonparametric randomized response and locally private confidence sets",
     url="https://github.com/wannabesmith/nprr",
     author="Ian Waudby-Smith",
     author_email="iwaudbysmith@gmail.com",
     license="BSD 3-Clause",
```

