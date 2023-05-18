# Comparing `tmp/circuitpython-bma220-0.1.0.tar.gz` & `tmp/circuitpython-bma220-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bma220-0.1.0.tar", last modified: Wed May 17 23:51:14 2023, max compression
+gzip compressed data, was "circuitpython-bma220-0.2.0.tar", last modified: Thu May 18 20:39:54 2023, max compression
```

## Comparing `circuitpython-bma220-0.1.0.tar` & `circuitpython-bma220-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.520401 circuitpython-bma220-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.512401 circuitpython-bma220-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.516401 circuitpython-bma220-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-17 23:51:14.516401 circuitpython-bma220-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-17 23:51:07.000000 circuitpython-bma220-0.1.0/bma220.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.516401 circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-17 23:51:14.000000 circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-17 23:51:14.000000 circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:51:14.000000 circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 23:51:14.000000 circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 23:51:14.000000 circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.516401 circuitpython-bma220-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.516401 circuitpython-bma220-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:51:14.516401 circuitpython-bma220-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-17 23:51:07.000000 circuitpython-bma220-0.1.0/examples/bma220_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-17 23:51:07.000000 circuitpython-bma220-0.1.0/examples/bma220_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-17 23:51:07.000000 circuitpython-bma220-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-17 23:50:58.000000 circuitpython-bma220-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:51:14.520401 circuitpython-bma220-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.115404 circuitpython-bma220-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/bma220/
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/bma220/bma220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/bma220/bma220_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/bma220/bma220_slope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 20:39:54.000000 circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.119404 circuitpython-bma220-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_latched_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_sleep_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_slope_slope_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/examples/bma220_slope_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-18 20:39:45.000000 circuitpython-bma220-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 20:39:31.000000 circuitpython-bma220-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:39:54.123404 circuitpython-bma220-0.2.0/setup.cfg
```

### Comparing `circuitpython-bma220-0.1.0/.github/workflows/build.yml` & `circuitpython-bma220-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/.gitignore` & `circuitpython-bma220-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/.pre-commit-config.yaml` & `circuitpython-bma220-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/.pylintrc` & `circuitpython-bma220-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/LICENSE` & `circuitpython-bma220-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/PKG-INFO` & `circuitpython-bma220-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.1.0
+Version: 0.2.0
 Summary: BMA220 Bosch Circuitpython Driver library
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bma220-0.1.0/README.rst` & `circuitpython-bma220-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/circuitpython_bma220.egg-info/PKG-INFO` & `circuitpython-bma220-0.2.0/circuitpython_bma220.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.1.0
+Version: 0.2.0
 Summary: BMA220 Bosch Circuitpython Driver library
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bma220-0.1.0/docs/_static/Logo.png` & `circuitpython-bma220-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/docs/_static/favicon.ico` & `circuitpython-bma220-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/docs/conf.py` & `circuitpython-bma220-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.1.0/examples/bma220_acc_range.py` & `circuitpython-bma220-0.2.0/examples/bma220_acc_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import time
 import board
-import bma220
+from bma220 import bma220
 
 i2c = board.I2C()
 bma = bma220.BMA220(i2c)
 
 bma.acc_range = bma220.ACC_RANGE_16
 
 while True:
```

### Comparing `circuitpython-bma220-0.1.0/pyproject.toml` & `circuitpython-bma220-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bma220"
 description = "BMA220 Bosch Circuitpython Driver library"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMA220"}
 keywords = [
     "sensor",
@@ -37,12 +37,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["bma220"]
+packages = ["bma220"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

