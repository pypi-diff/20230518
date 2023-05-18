# Comparing `tmp/adafruit-circuitpython-pixelbuf-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-pixelbuf-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pixelbuf-2.0.0.tar", last modified: Tue Dec 13 19:57:06 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pixelbuf-2.0.1.tar", last modified: Thu May 18 15:15:42 2023, max compression
```

## Comparing `adafruit-circuitpython-pixelbuf-2.0.0.tar` & `adafruit-circuitpython-pixelbuf-2.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.348694 adafruit-circuitpython-pixelbuf-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2022-12-13 19:57:06.000000 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-13 19:57:06.000000 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 19:57:06.000000 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-13 19:57:06.000000 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-13 19:57:06.000000 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2022-12-13 19:56:58.000000 adafruit-circuitpython-pixelbuf-2.0.0/adafruit_pixelbuf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-13 19:56:58.000000 adafruit-circuitpython-pixelbuf-2.0.0/examples/pixelbuf_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2022-12-13 19:56:58.000000 adafruit-circuitpython-pixelbuf-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-13 19:56:50.000000 adafruit-circuitpython-pixelbuf-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 19:57:06.352694 adafruit-circuitpython-pixelbuf-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.721671 adafruit-circuitpython-pixelbuf-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.709670 adafruit-circuitpython-pixelbuf-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.717671 adafruit-circuitpython-pixelbuf-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.717671 adafruit-circuitpython-pixelbuf-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.717671 adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-18 15:15:42.721671 adafruit-circuitpython-pixelbuf-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.717671 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-18 15:15:42.000000 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-18 15:15:42.000000 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:15:42.000000 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:15:42.000000 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 15:15:42.000000 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-05-18 15:15:33.000000 adafruit-circuitpython-pixelbuf-2.0.1/adafruit_pixelbuf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.721671 adafruit-circuitpython-pixelbuf-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.721671 adafruit-circuitpython-pixelbuf-2.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:42.721671 adafruit-circuitpython-pixelbuf-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-18 15:15:33.000000 adafruit-circuitpython-pixelbuf-2.0.1/examples/pixelbuf_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-18 15:15:33.000000 adafruit-circuitpython-pixelbuf-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:15:21.000000 adafruit-circuitpython-pixelbuf-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:15:42.721671 adafruit-circuitpython-pixelbuf-2.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pixelbuf-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/.gitignore` & `adafruit-circuitpython-pixelbuf-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-pixelbuf-2.0.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/.pylintrc` & `adafruit-circuitpython-pixelbuf-2.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pixelbuf-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/LICENSE` & `adafruit-circuitpython-pixelbuf-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pixelbuf-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/PKG-INFO` & `adafruit-circuitpython-pixelbuf-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pixelbuf
-Version: 2.0.0
+Version: 2.0.1
 Summary: A pure Python implementation of adafruit_pixelbuf for smaller boards.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Pixelbuf.git
 Keywords: adafruit,blinka,circuitpython,micropython,pixelbuf,neopixel,dotstar,leds
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/README.rst` & `adafruit-circuitpython-pixelbuf-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/PKG-INFO` & `adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pixelbuf
-Version: 2.0.0
+Version: 2.0.1
 Summary: A pure Python implementation of adafruit_pixelbuf for smaller boards.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Pixelbuf.git
 Keywords: adafruit,blinka,circuitpython,micropython,pixelbuf,neopixel,dotstar,leds
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/adafruit_circuitpython_pixelbuf.egg-info/SOURCES.txt` & `adafruit-circuitpython-pixelbuf-2.0.1/adafruit_circuitpython_pixelbuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/adafruit_pixelbuf.py` & `adafruit-circuitpython-pixelbuf-2.0.1/adafruit_pixelbuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 try:
     from typing import Optional, Tuple, Union, Sequence
 
     ColorUnion = Union[int, Tuple[int, int, int], Tuple[int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Pixelbuf.git"
 
 DOTSTAR_LED_START_FULL_BRIGHT = 0xFF
 DOTSTAR_LED_START = 0b11100000  # Three "1" bits, followed by 5 brightness bits
 DOTSTAR_LED_BRIGHTNESS = 0b00011111
 
 
@@ -48,15 +48,14 @@
         *,
         byteorder: str = "BGR",
         brightness: float = 1.0,
         auto_write: bool = False,
         header: Optional[bytes] = None,
         trailer: Optional[bytes] = None,
     ):
-
         bpp, byteorder_tuple, has_white, dotstar_mode = self.parse_byteorder(byteorder)
 
         self.auto_write = False
 
         effective_bpp = 4 if dotstar_mode else bpp
         _bytes = effective_bpp * size
         buf = bytearray(_bytes)
```

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-pixelbuf-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/docs/conf.py` & `adafruit-circuitpython-pixelbuf-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/docs/index.rst` & `adafruit-circuitpython-pixelbuf-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/examples/pixelbuf_simpletest.py` & `adafruit-circuitpython-pixelbuf-2.0.1/examples/pixelbuf_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixelbuf-2.0.0/pyproject.toml` & `adafruit-circuitpython-pixelbuf-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pixelbuf"
 description = "A pure Python implementation of adafruit_pixelbuf for smaller boards."
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Pixelbuf.git"}
 keywords = [
     "adafruit",
```

