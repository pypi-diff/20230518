# Comparing `tmp/adafruit-circuitpython-sharpmemorydisplay-1.4.7.tar.gz` & `tmp/adafruit-circuitpython-sharpmemorydisplay-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-sharpmemorydisplay-1.4.7.tar", last modified: Fri Apr 28 00:15:03 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-sharpmemorydisplay-1.4.8.tar", last modified: Thu May 18 15:41:37 2023, max compression
```

## Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7.tar` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.800783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.804783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.804783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 00:15:03.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_sharpmemorydisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/font5x8.bin.license
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-28 00:14:54.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 00:14:40.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:15:03.808783 adafruit-circuitpython-sharpmemorydisplay-1.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.396075 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.400076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_sharpmemorydisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/font5x8.bin.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/setup.cfg
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.gitignore` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pre-commit-config.yaml` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/.pylintrc` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSE` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/MIT.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/PKG-INFO` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sharpmemorydisplay
-Version: 1.4.7
+Version: 1.4.8
 Summary: CircuitPython display control library for Sharp memory displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay
 Keywords: adafruit,sharp,memory,display,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/README.rst` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sharpmemorydisplay
-Version: 1.4.7
+Version: 1.4.8
 Summary: CircuitPython display control library for Sharp memory displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay
 Keywords: adafruit,sharp,memory,display,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/adafruit_sharpmemorydisplay.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_sharpmemorydisplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from micropython import const
 
 try:
     import numpy
 except ImportError:
     numpy = None
 
-__version__ = "1.4.7"
+__version__ = "1.4.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay.git"
 
 _SHARPMEM_BIT_WRITECMD = const(0x80)  # in lsb
 _SHARPMEM_BIT_VCOM = const(0x40)  # in lsb
 _SHARPMEM_BIT_CLEAR = const(0x20)  # in lsb
 
 
@@ -99,15 +99,14 @@
 
     def show(self) -> None:
         """write out the frame buffer via SPI, we use MSB SPI only so some
         bit-swapping is required.
         """
 
         with self.spi_device as spi:
-
             image_buffer = bytearray()
             # toggle the VCOM bit
             self._buf[0] = _SHARPMEM_BIT_WRITECMD
             if self._vcom:
                 self._buf[0] |= _SHARPMEM_BIT_VCOM
             self._vcom = not self._vcom
             image_buffer.extend(self._buf)
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/_static/favicon.ico` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/conf.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/docs/index.rst` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/font5x8.bin` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/font5x8.bin`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_pillow_demo.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/examples/sharpmemorydisplay_simpletest.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.7/pyproject.toml` & `adafruit-circuitpython-sharpmemorydisplay-1.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-sharpmemorydisplay"
 description = "CircuitPython display control library for Sharp memory displays."
-version = "1.4.7"
+version = "1.4.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay"}
 keywords = [
     "adafruit",
```

