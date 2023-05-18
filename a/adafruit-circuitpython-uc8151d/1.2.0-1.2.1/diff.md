# Comparing `tmp/adafruit-circuitpython-uc8151d-1.2.0.tar.gz` & `tmp/adafruit-circuitpython-uc8151d-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-uc8151d-1.2.0.tar", last modified: Fri Nov 18 22:26:50 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-uc8151d-1.2.1.tar", last modified: Thu May 18 15:24:47 2023, max compression
```

## Comparing `adafruit-circuitpython-uc8151d-1.2.0.tar` & `adafruit-circuitpython-uc8151d-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.186373 adafruit-circuitpython-uc8151d-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.178373 adafruit-circuitpython-uc8151d-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.178373 adafruit-circuitpython-uc8151d-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.178373 adafruit-circuitpython-uc8151d-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.178373 adafruit-circuitpython-uc8151d-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-11-18 22:26:50.186373 adafruit-circuitpython-uc8151d-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.182373 adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-11-18 22:26:50.000000 adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-11-18 22:26:50.000000 adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 22:26:50.000000 adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-18 22:26:50.000000 adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-18 22:26:50.000000 adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     4605 2022-11-18 22:26:42.000000 adafruit-circuitpython-uc8151d-1.2.0/adafruit_uc8151d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.182373 adafruit-circuitpython-uc8151d-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.182373 adafruit-circuitpython-uc8151d-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 22:26:50.186373 adafruit-circuitpython-uc8151d-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   360122 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-11-18 22:26:42.000000 adafruit-circuitpython-uc8151d-1.2.0/examples/uc8151d_1.54_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-11-18 22:26:42.000000 adafruit-circuitpython-uc8151d-1.2.0/examples/uc8151d_2.9_color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-11-18 22:26:42.000000 adafruit-circuitpython-uc8151d-1.2.0/examples/uc8151d_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-11-18 22:26:42.000000 adafruit-circuitpython-uc8151d-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 22:26:34.000000 adafruit-circuitpython-uc8151d-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 22:26:50.186373 adafruit-circuitpython-uc8151d-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.009980 adafruit-circuitpython-uc8151d-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.001980 adafruit-circuitpython-uc8151d-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.001980 adafruit-circuitpython-uc8151d-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.005980 adafruit-circuitpython-uc8151d-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.005980 adafruit-circuitpython-uc8151d-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-18 15:24:47.009980 adafruit-circuitpython-uc8151d-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.005980 adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-18 15:24:46.000000 adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-18 15:24:46.000000 adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:24:46.000000 adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 15:24:46.000000 adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:24:46.000000 adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4607 2023-05-18 15:24:38.000000 adafruit-circuitpython-uc8151d-1.2.1/adafruit_uc8151d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.005980 adafruit-circuitpython-uc8151d-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.005980 adafruit-circuitpython-uc8151d-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:24:47.009980 adafruit-circuitpython-uc8151d-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   360122 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-18 15:24:38.000000 adafruit-circuitpython-uc8151d-1.2.1/examples/uc8151d_1.54_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 15:24:38.000000 adafruit-circuitpython-uc8151d-1.2.1/examples/uc8151d_2.9_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-18 15:24:38.000000 adafruit-circuitpython-uc8151d-1.2.1/examples/uc8151d_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-18 15:24:38.000000 adafruit-circuitpython-uc8151d-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 15:24:27.000000 adafruit-circuitpython-uc8151d-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:24:47.009980 adafruit-circuitpython-uc8151d-1.2.1/setup.cfg
```

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-uc8151d-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/.gitignore` & `adafruit-circuitpython-uc8151d-1.2.1/.gitignore`

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

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/.pre-commit-config.yaml` & `adafruit-circuitpython-uc8151d-1.2.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/.pylintrc` & `adafruit-circuitpython-uc8151d-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-uc8151d-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/LICENSE` & `adafruit-circuitpython-uc8151d-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-uc8151d-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/LICENSES/MIT.txt` & `adafruit-circuitpython-uc8151d-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-uc8151d-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/PKG-INFO` & `adafruit-circuitpython-uc8151d-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-uc8151d
-Version: 1.2.0
+Version: 1.2.1
 Summary: CircuitPython `displayio` driver for US8151D-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_UC8151D.git
 Keywords: adafruit,blinka,circuitpython,micropython,uc8151d,uc8151,us8151d,displayio,epd,epaper,flexible
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/README.rst` & `adafruit-circuitpython-uc8151d-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/PKG-INFO` & `adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-uc8151d
-Version: 1.2.0
+Version: 1.2.1
 Summary: CircuitPython `displayio` driver for US8151D-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_UC8151D.git
 Keywords: adafruit,blinka,circuitpython,micropython,uc8151d,uc8151,us8151d,displayio,epd,epaper,flexible
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/adafruit_circuitpython_uc8151d.egg-info/SOURCES.txt` & `adafruit-circuitpython-uc8151d-1.2.1/adafruit_circuitpython_uc8151d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/adafruit_uc8151d.py` & `adafruit-circuitpython-uc8151d-1.2.1/adafruit_uc8151d.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_UC8151D.git"
 
 _START_SEQUENCE = (
     # b"\x01\x05\x03\x00\x2b\x2b\x09"  # power setting
     # b"\x06\x03\x17\x17\x17"  # booster soft start
     b"\x04\x80\xc8"  # power on and wait 200 ms
     b"\x00\x01\x1f"  # panel setting. Further filled in below.
@@ -94,14 +94,16 @@
     b"\x50\x13\x01\x00\x00\x01"
     b"\x00\x00\x00\x00\x00\x00"
     b"\x00\x00\x00\x00\x00\x00"
     b"\x00\x00\x00\x00\x00\x00"
 )
 
 _STOP_SEQUENCE = b"\x50\x01\xf7" b"\x07\x01\xA5"  # CDI setting  # Deep Sleep
+
+
 # pylint: disable=too-few-public-methods
 class UC8151D(displayio.EPaperDisplay):
     r"""UC8151D driver
 
     :param bus: The data bus the display is on
     :param \**kwargs:
         See below
```

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/docs/_static/favicon.ico` & `adafruit-circuitpython-uc8151d-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/docs/conf.py` & `adafruit-circuitpython-uc8151d-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/docs/examples.rst` & `adafruit-circuitpython-uc8151d-1.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/docs/index.rst` & `adafruit-circuitpython-uc8151d-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/examples/display-ruler.bmp` & `adafruit-circuitpython-uc8151d-1.2.1/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/examples/uc8151d_1.54_grayscale.py` & `adafruit-circuitpython-uc8151d-1.2.1/examples/uc8151d_1.54_grayscale.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/examples/uc8151d_2.9_color.py` & `adafruit-circuitpython-uc8151d-1.2.1/examples/uc8151d_2.9_color.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/examples/uc8151d_simpletest.py` & `adafruit-circuitpython-uc8151d-1.2.1/examples/uc8151d_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-uc8151d-1.2.0/pyproject.toml` & `adafruit-circuitpython-uc8151d-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-uc8151d"
 description = "CircuitPython `displayio` driver for US8151D-based ePaper displays"
-version = "1.2.0"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_UC8151D.git"}
 keywords = [
     "adafruit",
```

