# Comparing `tmp/adafruit-circuitpython-ssd1680-1.1.0.tar.gz` & `tmp/adafruit-circuitpython-ssd1680-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1680-1.1.0.tar", last modified: Tue May  2 17:06:59 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1680-1.1.1.tar", last modified: Thu May 18 15:42:17 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1680-1.1.0.tar` & `adafruit-circuitpython-ssd1680-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.033716 adafruit-circuitpython-ssd1680-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.033716 adafruit-circuitpython-ssd1680-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.033716 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 17:06:59.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3231 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/adafruit_ssd1680.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.037716 adafruit-circuitpython-ssd1680-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   360122 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_2.13_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_2.13_tricolor_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_four_corners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 17:06:47.000000 adafruit-circuitpython-ssd1680-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 17:06:30.000000 adafruit-circuitpython-ssd1680-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:06:59.041716 adafruit-circuitpython-ssd1680-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.901655 adafruit-circuitpython-ssd1680-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.893655 adafruit-circuitpython-ssd1680-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.897655 adafruit-circuitpython-ssd1680-1.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.897655 adafruit-circuitpython-ssd1680-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.897655 adafruit-circuitpython-ssd1680-1.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 15:42:17.901655 adafruit-circuitpython-ssd1680-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.897655 adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 15:42:17.000000 adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-18 15:42:17.000000 adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:42:17.000000 adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:42:17.000000 adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:42:17.000000 adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3233 2023-05-18 15:42:09.000000 adafruit-circuitpython-ssd1680-1.1.1/adafruit_ssd1680.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.897655 adafruit-circuitpython-ssd1680-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.897655 adafruit-circuitpython-ssd1680-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:17.901655 adafruit-circuitpython-ssd1680-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   360122 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-18 15:42:09.000000 adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_2.13_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 15:42:09.000000 adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_2.13_tricolor_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-18 15:42:09.000000 adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_four_corners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-18 15:42:09.000000 adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-18 15:42:09.000000 adafruit-circuitpython-ssd1680-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:41:54.000000 adafruit-circuitpython-ssd1680-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:42:17.901655 adafruit-circuitpython-ssd1680-1.1.1/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1680-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/.gitignore` & `adafruit-circuitpython-ssd1680-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1680-1.1.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/.pylintrc` & `adafruit-circuitpython-ssd1680-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1680-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/LICENSE` & `adafruit-circuitpython-ssd1680-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1680-1.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1680-1.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1680-1.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/PKG-INFO` & `adafruit-circuitpython-ssd1680-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1680
-Version: 1.1.0
+Version: 1.1.1
 Summary: CircuitPython `displayio` drivers for SSD1680-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1680
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1680,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/README.rst` & `adafruit-circuitpython-ssd1680-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1680
-Version: 1.1.0
+Version: 1.1.1
 Summary: CircuitPython `displayio` drivers for SSD1680-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1680
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1680,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1680-1.1.1/adafruit_circuitpython_ssd1680.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/adafruit_ssd1680.py` & `adafruit-circuitpython-ssd1680-1.1.1/adafruit_ssd1680.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1680.git"
 
 _START_SEQUENCE = (
     b"\x12\x80\x14"  # soft reset and wait 20ms
     b"\x11\x01\x03"  # Ram data entry mode
     b"\x3C\x01\x05"  # border color
     b"\x2c\x01\x36"  # Set vcom voltage
@@ -43,14 +43,16 @@
     b"\x4e\x01\x01"  # ram x count
     b"\x4f\x02\x00\x00"  # ram y count
     b"\x01\x03\x00\x00\x00"  # set display size
     b"\x22\x01\xf4"  # display update mode
 )
 
 _STOP_SEQUENCE = b"\x10\x81\x01\x64"  # Deep Sleep
+
+
 # pylint: disable=too-few-public-methods
 class SSD1680(displayio.EPaperDisplay):
     r"""SSD1680 driver
 
     :param bus: The data bus the display is on
     :param \**kwargs:
         See below
```

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1680-1.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/docs/conf.py` & `adafruit-circuitpython-ssd1680-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/docs/examples.rst` & `adafruit-circuitpython-ssd1680-1.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/docs/index.rst` & `adafruit-circuitpython-ssd1680-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/examples/display-ruler.bmp` & `adafruit-circuitpython-ssd1680-1.1.1/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_2.13_featherwing.py` & `adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_2.13_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_2.13_tricolor_breakout.py` & `adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_2.13_tricolor_breakout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_four_corners.py` & `adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_four_corners.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/examples/ssd1680_simpletest.py` & `adafruit-circuitpython-ssd1680-1.1.1/examples/ssd1680_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1680-1.1.0/pyproject.toml` & `adafruit-circuitpython-ssd1680-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1680"
 description = "CircuitPython `displayio` drivers for SSD1680-based ePaper displays"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1680"}
 keywords = [
     "adafruit",
```

