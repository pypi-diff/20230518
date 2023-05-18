# Comparing `tmp/adafruit-circuitpython-spd1656-0.8.2.tar.gz` & `tmp/adafruit-circuitpython-spd1656-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-spd1656-0.8.2.tar", last modified: Wed Mar  1 15:37:35 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-spd1656-0.8.3.tar", last modified: Thu May 18 15:41:55 2023, max compression
```

## Comparing `adafruit-circuitpython-spd1656-0.8.2.tar` & `adafruit-circuitpython-spd1656-0.8.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.829762 adafruit-circuitpython-spd1656-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.829762 adafruit-circuitpython-spd1656-0.8.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.829762 adafruit-circuitpython-spd1656-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.829762 adafruit-circuitpython-spd1656-0.8.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-03-01 15:37:35.000000 adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-01 15:37:35.000000 adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:37:35.000000 adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-01 15:37:35.000000 adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-01 15:37:35.000000 adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-01 15:37:28.000000 adafruit-circuitpython-spd1656-0.8.2/adafruit_spd1656.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   921926 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/examples/display-ruler-720p.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/examples/display-ruler-720p.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 15:37:28.000000 adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_4in_acep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-01 15:37:28.000000 adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_color_stripes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-01 15:37:28.000000 adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_colors_and_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-01 15:37:28.000000 adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-01 15:37:28.000000 adafruit-circuitpython-spd1656-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-01 15:37:17.000000 adafruit-circuitpython-spd1656-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 15:37:35.833762 adafruit-circuitpython-spd1656-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.736935 adafruit-circuitpython-spd1656-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.728934 adafruit-circuitpython-spd1656-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.732934 adafruit-circuitpython-spd1656-0.8.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.732934 adafruit-circuitpython-spd1656-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.732934 adafruit-circuitpython-spd1656-0.8.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-18 15:41:55.736935 adafruit-circuitpython-spd1656-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.732934 adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-18 15:41:55.000000 adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-18 15:41:55.000000 adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:41:55.000000 adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 15:41:55.000000 adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:41:55.000000 adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-18 15:41:46.000000 adafruit-circuitpython-spd1656-0.8.3/adafruit_spd1656.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.736935 adafruit-circuitpython-spd1656-0.8.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.736935 adafruit-circuitpython-spd1656-0.8.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:55.736935 adafruit-circuitpython-spd1656-0.8.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   921926 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/examples/display-ruler-720p.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/examples/display-ruler-720p.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-18 15:41:46.000000 adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_4in_acep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-18 15:41:46.000000 adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_color_stripes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 15:41:46.000000 adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_colors_and_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-18 15:41:46.000000 adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 15:41:46.000000 adafruit-circuitpython-spd1656-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-18 15:41:34.000000 adafruit-circuitpython-spd1656-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:41:55.736935 adafruit-circuitpython-spd1656-0.8.3/setup.cfg
```

### Comparing `adafruit-circuitpython-spd1656-0.8.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-spd1656-0.8.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/.gitignore` & `adafruit-circuitpython-spd1656-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/.pre-commit-config.yaml` & `adafruit-circuitpython-spd1656-0.8.3/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-spd1656-0.8.2/.pylintrc` & `adafruit-circuitpython-spd1656-0.8.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-spd1656-0.8.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/LICENSE` & `adafruit-circuitpython-spd1656-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-spd1656-0.8.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/LICENSES/MIT.txt` & `adafruit-circuitpython-spd1656-0.8.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-spd1656-0.8.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/PKG-INFO` & `adafruit-circuitpython-spd1656-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-spd1656
-Version: 0.8.2
+Version: 0.8.3
 Summary: Driver for SPD1656 driven ACeP (7-color) e-paper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SPD1656
 Keywords: adafruit,blinka,circuitpython,micropython,spd1656
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-spd1656-0.8.2/README.rst` & `adafruit-circuitpython-spd1656-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/PKG-INFO` & `adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-spd1656
-Version: 0.8.2
+Version: 0.8.3
 Summary: Driver for SPD1656 driven ACeP (7-color) e-paper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SPD1656
 Keywords: adafruit,blinka,circuitpython,micropython,spd1656
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-spd1656-0.8.2/adafruit_circuitpython_spd1656.egg-info/SOURCES.txt` & `adafruit-circuitpython-spd1656-0.8.3/adafruit_circuitpython_spd1656.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/adafruit_spd1656.py` & `adafruit-circuitpython-spd1656-0.8.3/adafruit_spd1656.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 """
 
 import struct
 
 import displayio
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SPD1656.git"
 
 _START_SEQUENCE = (
     b"\x01\x04\x37\x00\x23\x23"  # power setting
     b"\x00\x02\xef\x08"  # panel setting (PSR)
     b"\x03\x01\x00"  # PFS
     b"\x06\x03\xc7\xc7\x1d"  # booster
@@ -42,14 +42,15 @@
     b"\x04\x80\xc8"  # power on and wait 10 ms
 )
 
 _STOP_SEQUENCE = b"\x02\x01\x00" b"\x07\x01\xA5"  # Power off then deep sleep
 
 # Datasheet is here: https://www.waveshare.com/w/upload/b/bf/SPD1656_1.1.pdf
 
+
 # pylint: disable=too-few-public-methods
 class SPD1656(displayio.EPaperDisplay):
     r"""SPD1656 display driver
 
     :param bus: The data bus the display is on
     :param \**kwargs:
         See below
```

### Comparing `adafruit-circuitpython-spd1656-0.8.2/docs/_static/favicon.ico` & `adafruit-circuitpython-spd1656-0.8.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/docs/conf.py` & `adafruit-circuitpython-spd1656-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/docs/examples.rst` & `adafruit-circuitpython-spd1656-0.8.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/docs/index.rst` & `adafruit-circuitpython-spd1656-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/examples/display-ruler-720p.bmp` & `adafruit-circuitpython-spd1656-0.8.3/examples/display-ruler-720p.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_4in_acep.py` & `adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_4in_acep.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_color_stripes.py` & `adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_color_stripes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_colors_and_text.py` & `adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_colors_and_text.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/examples/spd1656_simpletest.py` & `adafruit-circuitpython-spd1656-0.8.3/examples/spd1656_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-spd1656-0.8.2/pyproject.toml` & `adafruit-circuitpython-spd1656-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-spd1656"
 description = "Driver for SPD1656 driven ACeP (7-color) e-paper displays"
-version = "0.8.2"
+version = "0.8.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SPD1656"}
 keywords = [
     "adafruit",
```

