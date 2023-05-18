# Comparing `tmp/adafruit-circuitpython-floppy-1.0.7.tar.gz` & `tmp/adafruit-circuitpython-floppy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-floppy-1.0.7.tar", last modified: Mon Mar  6 17:00:03 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-floppy-1.0.8.tar", last modified: Thu May 18 15:36:15 2023, max compression
```

## Comparing `adafruit-circuitpython-floppy-1.0.7.tar` & `adafruit-circuitpython-floppy-1.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.180180 adafruit-circuitpython-floppy-1.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.160180 adafruit-circuitpython-floppy-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.168180 adafruit-circuitpython-floppy-1.0.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.168180 adafruit-circuitpython-floppy-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.168180 adafruit-circuitpython-floppy-1.0.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-06 17:00:03.180180 adafruit-circuitpython-floppy-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.172180 adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-06 17:00:03.000000 adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-06 17:00:03.000000 adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 17:00:03.000000 adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-06 17:00:03.000000 adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-06 17:00:03.000000 adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-03-06 16:59:55.000000 adafruit-circuitpython-floppy-1.0.7/adafruit_floppy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.176180 adafruit-circuitpython-floppy-1.0.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.176180 adafruit-circuitpython-floppy-1.0.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:00:03.180180 adafruit-circuitpython-floppy-1.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-06 16:59:55.000000 adafruit-circuitpython-floppy-1.0.7/examples/floppy_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-06 16:59:55.000000 adafruit-circuitpython-floppy-1.0.7/examples/floppy_vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-06 16:59:55.000000 adafruit-circuitpython-floppy-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-06 16:59:46.000000 adafruit-circuitpython-floppy-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 17:00:03.180180 adafruit-circuitpython-floppy-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.675026 adafruit-circuitpython-floppy-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.683026 adafruit-circuitpython-floppy-1.0.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.687026 adafruit-circuitpython-floppy-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.687026 adafruit-circuitpython-floppy-1.0.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.691027 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_floppy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/examples/floppy_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/examples/floppy_vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/setup.cfg
```

### Comparing `adafruit-circuitpython-floppy-1.0.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-floppy-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/.gitignore` & `adafruit-circuitpython-floppy-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/.pre-commit-config.yaml` & `adafruit-circuitpython-floppy-1.0.8/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-floppy-1.0.7/.pylintrc` & `adafruit-circuitpython-floppy-1.0.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-floppy-1.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/LICENSE` & `adafruit-circuitpython-floppy-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-floppy-1.0.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/LICENSES/MIT.txt` & `adafruit-circuitpython-floppy-1.0.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-floppy-1.0.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/PKG-INFO` & `adafruit-circuitpython-floppy-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-floppy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Access floppy drives from CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Floppy
 Keywords: adafruit,floppy,drive,storage,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-floppy-1.0.7/README.rst` & `adafruit-circuitpython-floppy-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/PKG-INFO` & `adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-floppy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Access floppy drives from CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Floppy
 Keywords: adafruit,floppy,drive,storage,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-floppy-1.0.7/adafruit_circuitpython_floppy.egg-info/SOURCES.txt` & `adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/adafruit_floppy.py` & `adafruit-circuitpython-floppy-1.0.8/adafruit_floppy.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import typing
     import microcontroller
     import circuitpython_typing  # pylint: disable=unused-import
 except ImportError:
     pass
 
 
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_floppy.git"
 
 
 def _optionaldigitalinout(
     maybe_pin: typing.Optional[microcontroller.Pin],
 ) -> typing.Optional[DigitalInOut]:
     return None if maybe_pin is None else DigitalInOut(maybe_pin)
@@ -108,15 +108,16 @@
             self._step.value = False
 
     def find_track0(self):
         """Move the head out until the 'track0' signal becomes False
 
         If successful, sets the internal track number to 0.
 
-        If unsuccsessful, sets the internatl track number to None and raises an exception."""
+        If unsuccsessful, sets the internatl track number to None and raises an exception.
+        """
         self._track = None
         # First move off of track0. One of my drives would not function properly
         # without this initial move-off.
         for _ in range(4):
             self._do_step(_STEP_IN, 1)
         for _ in range(250):
             if not self._track0.value:
```

### Comparing `adafruit-circuitpython-floppy-1.0.7/docs/_static/favicon.ico` & `adafruit-circuitpython-floppy-1.0.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/docs/conf.py` & `adafruit-circuitpython-floppy-1.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/docs/index.rst` & `adafruit-circuitpython-floppy-1.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/examples/floppy_simpletest.py` & `adafruit-circuitpython-floppy-1.0.8/examples/floppy_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/examples/floppy_vfs.py` & `adafruit-circuitpython-floppy-1.0.8/examples/floppy_vfs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.7/pyproject.toml` & `adafruit-circuitpython-floppy-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-floppy"
 description = "Access floppy drives from CircuitPython"
-version = "1.0.7"
+version = "1.0.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Floppy"}
 keywords = [
     "adafruit",
```

