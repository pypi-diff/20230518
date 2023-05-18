# Comparing `tmp/adafruit-circuitpython-magtag-2.2.4.tar.gz` & `tmp/adafruit-circuitpython-magtag-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-magtag-2.2.4.tar", last modified: Mon Jan 23 20:47:29 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-magtag-2.2.5.tar", last modified: Thu May 18 15:38:30 2023, max compression
```

## Comparing `adafruit-circuitpython-magtag-2.2.4.tar` & `adafruit-circuitpython-magtag-2.2.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.861559 adafruit-circuitpython-magtag-2.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.861559 adafruit-circuitpython-magtag-2.2.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-01-23 20:47:29.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-23 20:47:29.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 20:47:29.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-23 20:47:29.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-23 20:47:29.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7327 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/magtag.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2595 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5897 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/examples/magtag_btn_sleep_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/examples/magtag_quote_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/examples/magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-01-23 20:47:21.000000 adafruit-circuitpython-magtag-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-23 20:47:11.000000 adafruit-circuitpython-magtag-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 20:47:29.865559 adafruit-circuitpython-magtag-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.731775 adafruit-circuitpython-magtag-2.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.723775 adafruit-circuitpython-magtag-2.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 15:38:30.731775 adafruit-circuitpython-magtag-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7326 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/magtag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2595 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5897 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/examples/magtag_btn_sleep_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/examples/magtag_quote_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/examples/magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:38:30.731775 adafruit-circuitpython-magtag-2.2.5/setup.cfg
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-magtag-2.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/.gitignore` & `adafruit-circuitpython-magtag-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/.pre-commit-config.yaml` & `adafruit-circuitpython-magtag-2.2.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-magtag-2.2.4/.pylintrc` & `adafruit-circuitpython-magtag-2.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-magtag-2.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/LICENSE` & `adafruit-circuitpython-magtag-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-magtag-2.2.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/LICENSES/MIT.txt` & `adafruit-circuitpython-magtag-2.2.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-magtag-2.2.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/PKG-INFO` & `adafruit-circuitpython-magtag-2.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-magtag
-Version: 2.2.4
+Version: 2.2.5
 Summary: Helper library for the Adafruit MagTag
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MagTag
 Keywords: adafruit,magtag,eink,iot,esp32,espressif,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/README.rst` & `adafruit-circuitpython-magtag-2.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/PKG-INFO` & `adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-magtag
-Version: 2.2.4
+Version: 2.2.5
 Summary: Helper library for the Adafruit MagTag
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MagTag
 Keywords: adafruit,magtag,eink,iot,esp32,espressif,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/adafruit_circuitpython_magtag.egg-info/SOURCES.txt` & `adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/graphics.py` & `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from adafruit_portalbase.graphics import GraphicsBase
 
 try:
     from typing import Union, Optional, Tuple
 except ImportError:
     pass
 
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the MagTag Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/magtag.py` & `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/magtag.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 try:
     from typing import Optional, Union, Sequence, Dict, Callable, Any
     import microcontroller
     import neopixel
 except ImportError:
     pass
 
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class MagTag(PortalBase):
     """Class representing the Adafruit MagTag.
 
     :param url: The URL of your data source. Defaults to ``None``.
@@ -78,15 +78,14 @@
         regexp_path: Optional[Sequence[str]] = None,
         default_bg: Union[str, int] = 0xFFFFFF,
         status_neopixel: Optional[Union[microcontroller.Pin, neopixel.NeoPixel]] = None,
         json_transform: Union[Sequence[Callable], Callable] = None,
         rotation: int = 270,
         debug: bool = False,
     ) -> None:
-
         self.peripherals = Peripherals()
 
         if status_neopixel == board.NEOPIXEL:
             status_neopixel = self.peripherals.neopixels
 
         network = Network(
             status_neopixel=status_neopixel,
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/network.py` & `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Optional, Union
     import microcontroller
 except ImportError:
     pass
 
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit MagTag.
 
     :param status_neopixel: The pin for the status NeoPixel. Use ``board.NEOPIXEL`` for the on-board
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/adafruit_magtag/peripherals.py` & `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/peripherals.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import board
 from digitalio import DigitalInOut, Direction, Pull
 from analogio import AnalogIn
 import neopixel
 import simpleio
 
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the MagTag Library"""
 
     # pylint: disable=too-many-instance-attributes, too-many-locals, too-many-branches, too-many-statements
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/docs/_static/favicon.ico` & `adafruit-circuitpython-magtag-2.2.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/docs/conf.py` & `adafruit-circuitpython-magtag-2.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/docs/index.rst` & `adafruit-circuitpython-magtag-2.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/examples/magtag_btn_sleep_demo.py` & `adafruit-circuitpython-magtag-2.2.5/examples/magtag_btn_sleep_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 button_tones = (1047, 1318, 1568, 2093)
 
 now = time.monotonic()
 last_action_time = now
 while True:
     now = time.monotonic()
     if now - last_action_time >= 10.0:
-
         magtag.set_text("Sleeping")
         magtag.peripherals.deinit()
         time.sleep(2)
         # go to sleep
         pin_alarm = alarm.pin.PinAlarm(pin=board.D11, value=False, pull=True)
 
         # Exit the program, and then deep sleep until the alarm wakes us.
```

### Comparing `adafruit-circuitpython-magtag-2.2.4/examples/magtag_quote_demo.py` & `adafruit-circuitpython-magtag-2.2.5/examples/magtag_quote_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/examples/magtag_simpletest.py` & `adafruit-circuitpython-magtag-2.2.5/examples/magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.4/pyproject.toml` & `adafruit-circuitpython-magtag-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-magtag"
 description = "Helper library for the Adafruit MagTag"
-version = "2.2.4"
+version = "2.2.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag"}
 keywords = [
     "adafruit",
```

