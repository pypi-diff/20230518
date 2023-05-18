# Comparing `tmp/adafruit-circuitpython-tmp117-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-tmp117-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tmp117-1.1.8.tar", last modified: Tue Mar 14 19:35:56 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-tmp117-1.1.9.tar", last modified: Thu May 18 15:42:57 2023, max compression
```

## Comparing `adafruit-circuitpython-tmp117-1.1.8.tar` & `adafruit-circuitpython-tmp117-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.818399 adafruit-circuitpython-tmp117-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.814399 adafruit-circuitpython-tmp117-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.814399 adafruit-circuitpython-tmp117-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.814399 adafruit-circuitpython-tmp117-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.814399 adafruit-circuitpython-tmp117-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-14 19:35:56.818399 adafruit-circuitpython-tmp117-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.814399 adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-14 19:35:56.000000 adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-14 19:35:56.000000 adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:35:56.000000 adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-14 19:35:56.000000 adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-14 19:35:56.000000 adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21350 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/adafruit_tmp117.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.818399 adafruit-circuitpython-tmp117-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.818399 adafruit-circuitpython-tmp117-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:35:56.818399 adafruit-circuitpython-tmp117-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_limits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_offset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_rate_and_averaging_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_single_measurement_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-14 19:35:49.000000 adafruit-circuitpython-tmp117-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-14 19:35:39.000000 adafruit-circuitpython-tmp117-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:35:56.818399 adafruit-circuitpython-tmp117-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.823019 adafruit-circuitpython-tmp117-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.815019 adafruit-circuitpython-tmp117-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.819019 adafruit-circuitpython-tmp117-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.819019 adafruit-circuitpython-tmp117-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:42:35.000000 adafruit-circuitpython-tmp117-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.819019 adafruit-circuitpython-tmp117-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-18 15:42:57.823019 adafruit-circuitpython-tmp117-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.819019 adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-18 15:42:57.000000 adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-18 15:42:57.000000 adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:42:57.000000 adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:42:57.000000 adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:42:57.000000 adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/adafruit_tmp117.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.823019 adafruit-circuitpython-tmp117-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.823019 adafruit-circuitpython-tmp117-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:57.823019 adafruit-circuitpython-tmp117-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_offset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_rate_and_averaging_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_single_measurement_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-18 15:42:48.000000 adafruit-circuitpython-tmp117-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:42:36.000000 adafruit-circuitpython-tmp117-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:42:57.823019 adafruit-circuitpython-tmp117-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-tmp117-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tmp117-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/.gitignore` & `adafruit-circuitpython-tmp117-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tmp117-1.1.9/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

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
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-tmp117-1.1.8/.pylintrc` & `adafruit-circuitpython-tmp117-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tmp117-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/LICENSE` & `adafruit-circuitpython-tmp117-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tmp117-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tmp117-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tmp117-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/PKG-INFO` & `adafruit-circuitpython-tmp117-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tmp117
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the TI TMP117 Temperature sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TMP117
 Keywords: adafruit,blinka,circuitpython,micropython,tmp117,temp,temperature,TMP,accurate,EEPROM
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tmp117-1.1.8/README.rst` & `adafruit-circuitpython-tmp117-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/PKG-INFO` & `adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tmp117
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the TI TMP117 Temperature sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TMP117
 Keywords: adafruit,blinka,circuitpython,micropython,tmp117,temp,temperature,TMP,accurate,EEPROM
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tmp117-1.1.8/adafruit_circuitpython_tmp117.egg-info/SOURCES.txt` & `adafruit-circuitpython-tmp117-1.1.9/adafruit_circuitpython_tmp117.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/adafruit_tmp117.py` & `adafruit-circuitpython-tmp117-1.1.9/adafruit_tmp117.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 try:
     from typing import Sequence, Tuple, Optional, Union
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __repo__ = "https:#github.com/adafruit/Adafruit_CircuitPython_TMP117.git"
 
 
 _I2C_ADDR = 0x48  # default I2C Address
 _TEMP_RESULT = const(0x00)
 _CONFIGURATION = const(0x01)
 _T_HIGH_LIMIT = const(0x02)
@@ -187,15 +187,14 @@
 
     _raw_alert_mode = RWBit(_CONFIGURATION, 4, 2, False)  # T/nA bits in the datasheet
     _int_active_high = RWBit(_CONFIGURATION, 3, 2, False)
     _data_ready_int_en = RWBit(_CONFIGURATION, 2, 2, False)
     _soft_reset = RWBit(_CONFIGURATION, 1, 2, False)
 
     def __init__(self, i2c_bus: I2C, address: int = _I2C_ADDR):
-
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         if self._part_id != _DEVICE_ID_VALUE:
             raise AttributeError("Cannot find a TMP117")
         # currently set when `alert_status` is read, but not exposed
         self.reset()
         self.initialize()
 
@@ -515,15 +514,14 @@
                 eeprom3_data[1],
             ]
         )
         # Convert to an integer
         return _convert_to_integer(combined_id)
 
     def _set_mode_and_wait_for_measurement(self, mode: int) -> float:
-
         self._mode = mode
         # poll for data ready
         while not self._read_status()[2]:
             time.sleep(0.001)
 
         return self._read_temperature()
```

### Comparing `adafruit-circuitpython-tmp117-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tmp117-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/docs/conf.py` & `adafruit-circuitpython-tmp117-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/docs/examples.rst` & `adafruit-circuitpython-tmp117-1.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/docs/index.rst` & `adafruit-circuitpython-tmp117-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_limits_test.py` & `adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_limits_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_offset_test.py` & `adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_offset_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_rate_and_averaging_test.py` & `adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_rate_and_averaging_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/examples/tmp117_single_measurement_test.py` & `adafruit-circuitpython-tmp117-1.1.9/examples/tmp117_single_measurement_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp117-1.1.8/pyproject.toml` & `adafruit-circuitpython-tmp117-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-tmp117"
 description = "CircuitPython library for the TI TMP117 Temperature sensor"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TMP117"}
 keywords = [
     "adafruit",
```

