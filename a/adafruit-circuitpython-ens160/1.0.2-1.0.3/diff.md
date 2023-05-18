# Comparing `tmp/adafruit-circuitpython-ens160-1.0.2.tar.gz` & `tmp/adafruit-circuitpython-ens160-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ens160-1.0.2.tar", last modified: Tue Mar 28 00:13:42 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ens160-1.0.3.tar", last modified: Thu May 18 15:35:32 2023, max compression
```

## Comparing `adafruit-circuitpython-ens160-1.0.2.tar` & `adafruit-circuitpython-ens160-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.110775 adafruit-circuitpython-ens160-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.114775 adafruit-circuitpython-ens160-1.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-28 00:13:42.000000 adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-28 00:13:42.000000 adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 00:13:42.000000 adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-28 00:13:42.000000 adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 00:13:42.000000 adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-03-28 00:13:34.000000 adafruit-circuitpython-ens160-1.0.2/adafruit_ens160.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-28 00:13:34.000000 adafruit-circuitpython-ens160-1.0.2/examples/ens160_advancedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-28 00:13:34.000000 adafruit-circuitpython-ens160-1.0.2/examples/ens160_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-28 00:13:34.000000 adafruit-circuitpython-ens160-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-28 00:13:21.000000 adafruit-circuitpython-ens160-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 00:13:42.118775 adafruit-circuitpython-ens160-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_ens160.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/examples/ens160_advancedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/examples/ens160_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/setup.cfg
```

### Comparing `adafruit-circuitpython-ens160-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ens160-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/.gitignore` & `adafruit-circuitpython-ens160-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/.pre-commit-config.yaml` & `adafruit-circuitpython-ens160-1.0.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ens160-1.0.2/.pylintrc` & `adafruit-circuitpython-ens160-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ens160-1.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/LICENSE` & `adafruit-circuitpython-ens160-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ens160-1.0.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/LICENSES/MIT.txt` & `adafruit-circuitpython-ens160-1.0.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ens160-1.0.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/PKG-INFO` & `adafruit-circuitpython-ens160-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ens160
-Version: 1.0.2
+Version: 1.0.3
 Summary: CircuitPython / Python library for ScioSense ENS160 digital multi-gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ENS160
 Keywords: adafruit,blinka,circuitpython,micropython,ens160,ens160,python,circuitpython,gas,tvoc,eco2,mox,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ens160-1.0.2/README.rst` & `adafruit-circuitpython-ens160-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/PKG-INFO` & `adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ens160
-Version: 1.0.2
+Version: 1.0.3
 Summary: CircuitPython / Python library for ScioSense ENS160 digital multi-gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ENS160
 Keywords: adafruit,blinka,circuitpython,micropython,ens160,ens160,python,circuitpython,gas,tvoc,eco2,mox,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ens160-1.0.2/adafruit_circuitpython_ens160.egg-info/SOURCES.txt` & `adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/adafruit_ens160.py` & `adafruit-circuitpython-ens160-1.0.3/adafruit_ens160.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 try:
     from typing import Dict, Optional, Union, List
     from typing_extensions import Literal
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ENS160.git"
 
 
 ENS160_I2CADDR_DEFAULT: int = const(0x53)  # Default I2C address
 
 _ENS160_REG_PARTID = const(0x00)
 _ENS160_REG_OPMODE = const(0x10)
@@ -100,15 +100,14 @@
     interrupt_polarity = RWBit(_ENS160_REG_CONFIG, 6)
     interrupt_pushpull = RWBit(_ENS160_REG_CONFIG, 5)
     interrupt_on_GPR = RWBit(_ENS160_REG_CONFIG, 3)
     interrupt_on_data = RWBit(_ENS160_REG_CONFIG, 1)
     interrupt_enable = RWBit(_ENS160_REG_CONFIG, 0)
 
     def __init__(self, i2c_bus: I2C, address: int = ENS160_I2CADDR_DEFAULT) -> None:
-
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
 
         self.reset()
 
         if self.part_id != 0x160:
             raise RuntimeError("Unable to find ENS160, check your wiring")
         self.mode = MODE_IDLE
```

### Comparing `adafruit-circuitpython-ens160-1.0.2/docs/_static/favicon.ico` & `adafruit-circuitpython-ens160-1.0.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/docs/conf.py` & `adafruit-circuitpython-ens160-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/docs/index.rst` & `adafruit-circuitpython-ens160-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/examples/ens160_advancedtest.py` & `adafruit-circuitpython-ens160-1.0.3/examples/ens160_advancedtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/examples/ens160_simpletest.py` & `adafruit-circuitpython-ens160-1.0.3/examples/ens160_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.2/pyproject.toml` & `adafruit-circuitpython-ens160-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ens160"
 description = "CircuitPython / Python library for ScioSense ENS160 digital multi-gas sensor"
-version = "1.0.2"
+version = "1.0.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ENS160"}
 keywords = [
     "adafruit",
```

