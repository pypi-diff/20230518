# Comparing `tmp/adafruit-circuitpython-ssd1325-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-ssd1325-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1325-1.4.8.tar", last modified: Mon Nov 28 18:07:29 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1325-1.4.9.tar", last modified: Thu May 18 15:19:44 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1325-1.4.8.tar` & `adafruit-circuitpython-ssd1325-1.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.157898 adafruit-circuitpython-ssd1325-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.157898 adafruit-circuitpython-ssd1325-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.157898 adafruit-circuitpython-ssd1325-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3813 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3048 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3813 2022-11-28 18:07:29.000000 adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      990 2022-11-28 18:07:29.000000 adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:07:29.000000 adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       28 2022-11-28 18:07:29.000000 adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:07:29.000000 adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2022-11-28 18:07:21.000000 adafruit-circuitpython-ssd1325-1.4.8/adafruit_ssd1325.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5645 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2022-11-28 18:07:21.000000 adafruit-circuitpython-ssd1325-1.4.8/examples/ssd1325_gamma.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2022-11-28 18:07:21.000000 adafruit-circuitpython-ssd1325-1.4.8/examples/ssd1325_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2022-11-28 18:07:21.000000 adafruit-circuitpython-ssd1325-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      125 2022-11-28 18:07:13.000000 adafruit-circuitpython-ssd1325-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:07:29.161898 adafruit-circuitpython-ssd1325-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.502850 adafruit-circuitpython-ssd1325-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.502850 adafruit-circuitpython-ssd1325-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-18 15:19:44.000000 adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 15:19:44.000000 adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:19:44.000000 adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:19:44.000000 adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:19:44.000000 adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-18 15:19:35.000000 adafruit-circuitpython-ssd1325-1.4.9/adafruit_ssd1325.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-18 15:19:35.000000 adafruit-circuitpython-ssd1325-1.4.9/examples/ssd1325_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-18 15:19:35.000000 adafruit-circuitpython-ssd1325-1.4.9/examples/ssd1325_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-18 15:19:35.000000 adafruit-circuitpython-ssd1325-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:19:20.000000 adafruit-circuitpython-ssd1325-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:19:44.506850 adafruit-circuitpython-ssd1325-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1325-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/.gitignore` & `adafruit-circuitpython-ssd1325-1.4.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1325-1.4.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/.pylintrc` & `adafruit-circuitpython-ssd1325-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1325-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/LICENSE` & `adafruit-circuitpython-ssd1325-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1325-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1325-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1325-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/PKG-INFO` & `adafruit-circuitpython-ssd1325-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1325
-Version: 1.4.8
+Version: 1.4.9
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1325
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1325
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1325,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/README.rst` & `adafruit-circuitpython-ssd1325-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1325
-Version: 1.4.8
+Version: 1.4.9
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1325
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1325
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1325,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/adafruit_circuitpython_ssd1325.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1325-1.4.9/adafruit_circuitpython_ssd1325.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/adafruit_ssd1325.py` & `adafruit-circuitpython-ssd1325-1.4.9/adafruit_ssd1325.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Adafruit CircuitPython 5+ firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1325.git"
 
 _INIT_SEQUENCE = (
     b"\xAE\x00"  # DISPLAY_OFF
     b"\xb3\x01\xa1"  # Set clock
     b"\xa8\x01\x3f"  # Mux ratio is 1/64
     b"\xa1\x01\x00"  # Display start line is 0
@@ -48,14 +48,15 @@
     b"\xbc\x01\x3f"  # Set pre-charge voltage
     b"\xbe\x01\x1c"  # Set vcom voltage
     b"\xbf\x01\x0f"  # set Low Voltage Level of SEG Pin
     b"\xa4\x00"  # Normal display
     b"\xaf\x00"  # DISPLAY_ON
 )
 
+
 # pylint: disable=too-few-public-methods
 class SSD1325(displayio.Display):
     """
     SSD1325 driver
 
     :param int width: The width of the display
     :param int height: The height of the display
```

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1325-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/docs/conf.py` & `adafruit-circuitpython-ssd1325-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/docs/index.rst` & `adafruit-circuitpython-ssd1325-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/examples/ssd1325_gamma.py` & `adafruit-circuitpython-ssd1325-1.4.9/examples/ssd1325_gamma.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/examples/ssd1325_simpletest.py` & `adafruit-circuitpython-ssd1325-1.4.9/examples/ssd1325_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1325-1.4.8/pyproject.toml` & `adafruit-circuitpython-ssd1325-1.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1325"
 description = "DisplayIO driver for grayscale OLEDs drive by SSD1325"
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1325"}
 keywords = [
     "adafruit",
```

