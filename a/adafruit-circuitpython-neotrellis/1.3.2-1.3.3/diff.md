# Comparing `tmp/adafruit-circuitpython-neotrellis-1.3.2.tar.gz` & `tmp/adafruit-circuitpython-neotrellis-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neotrellis-1.3.2.tar", last modified: Thu Jan 12 17:33:30 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-neotrellis-1.3.3.tar", last modified: Thu May 18 15:15:24 2023, max compression
```

## Comparing `adafruit-circuitpython-neotrellis-1.3.2.tar` & `adafruit-circuitpython-neotrellis-1.3.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.436395 adafruit-circuitpython-neotrellis-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.436395 adafruit-circuitpython-neotrellis-1.3.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.436395 adafruit-circuitpython-neotrellis-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.436395 adafruit-circuitpython-neotrellis-1.3.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-01-12 17:33:30.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-01-12 17:33:30.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 17:33:30.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-12 17:33:30.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-12 17:33:30.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/adafruit_neotrellis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:20.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_neotrellis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4260 2023-01-12 17:33:20.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_neotrellis/multitrellis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3621 2023-01-12 17:33:20.000000 adafruit-circuitpython-neotrellis-1.3.2/adafruit_neotrellis/neotrellis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-12 17:33:20.000000 adafruit-circuitpython-neotrellis-1.3.2/examples/neotrellis_multitrellis_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-01-12 17:33:20.000000 adafruit-circuitpython-neotrellis-1.3.2/examples/neotrellis_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-12 17:33:20.000000 adafruit-circuitpython-neotrellis-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-12 17:33:08.000000 adafruit-circuitpython-neotrellis-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 17:33:30.440395 adafruit-circuitpython-neotrellis-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.416101 adafruit-circuitpython-neotrellis-1.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.420101 adafruit-circuitpython-neotrellis-1.3.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.420101 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.420101 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/multitrellis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3621 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/neotrellis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_multitrellis_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/setup.cfg
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neotrellis-1.3.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/.gitignore` & `adafruit-circuitpython-neotrellis-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/.pre-commit-config.yaml` & `adafruit-circuitpython-neotrellis-1.3.3/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/.pylintrc` & `adafruit-circuitpython-neotrellis-1.3.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neotrellis-1.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/LICENSE` & `adafruit-circuitpython-neotrellis-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neotrellis-1.3.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/LICENSES/MIT.txt` & `adafruit-circuitpython-neotrellis-1.3.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neotrellis-1.3.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/PKG-INFO` & `adafruit-circuitpython-neotrellis-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neotrellis
-Version: 1.3.2
+Version: 1.3.3
 Summary: CircuitPython library for using Adafruit NeoTrellis.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoTrellis
 Keywords: adafruit,neotrellis,neopixel,trellis,led,rgbsensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/README.rst` & `adafruit-circuitpython-neotrellis-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO` & `adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neotrellis
-Version: 1.3.2
+Version: 1.3.3
 Summary: CircuitPython library for using Adafruit NeoTrellis.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoTrellis
 Keywords: adafruit,neotrellis,neopixel,trellis,led,rgbsensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt` & `adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/adafruit_neotrellis/multitrellis.py` & `adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/multitrellis.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit Seesaw CircuitPython library
   https://github.com/adafruit/Adafruit_CircuitPython_seesaw/releases
 """
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_neotrellis.git"
 
 
 from time import sleep
 from micropython import const
 from adafruit_seesaw.keypad import KeyEvent
 
@@ -79,15 +79,14 @@
         ykey = int(int(y % 4) * 4 / 4)
         self._trelli[int(y / 4)][int(x / 4)].pixels[ykey * 4 + xkey] = color
 
     def sync(self):
         """Read all trellis boards in the matrix and call any callbacks"""
         for _n in range(self._rows):
             for _m in range(self._cols):
-
                 _t = self._trelli[_n][_m]
                 available = _t.count
                 sleep(0.0005)
                 if available > 0:
                     available = available + 2
                     buf = _t.read_keypad(available)
                     for raw in buf:
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/adafruit_neotrellis/neotrellis.py` & `adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/neotrellis.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit Seesaw CircuitPython library
   https://github.com/adafruit/Adafruit_CircuitPython_seesaw/releases
 """
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_neotrellis.git"
 
 from time import sleep
 from micropython import const
 from adafruit_seesaw.keypad import Keypad, KeyEvent
 from adafruit_seesaw.neopixel import NeoPixel, GRB
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/docs/_static/favicon.ico` & `adafruit-circuitpython-neotrellis-1.3.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/docs/conf.py` & `adafruit-circuitpython-neotrellis-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/docs/index.rst` & `adafruit-circuitpython-neotrellis-1.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/examples/neotrellis_multitrellis_simpletest.py` & `adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_multitrellis_simpletest.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 RED = (255, 0, 0)
 YELLOW = (255, 150, 0)
 GREEN = (0, 255, 0)
 CYAN = (0, 255, 255)
 BLUE = (0, 0, 255)
 PURPLE = (180, 0, 255)
 
+
 # This will be called when button events are received
 def blink(xcoord, ycoord, edge):
     # Turn the LED on when a rising edge is detected
     if edge == NeoTrellis.EDGE_RISING:
         trellis.color(xcoord, ycoord, BLUE)
     # Turn the LED off when a falling edge is detected
     elif edge == NeoTrellis.EDGE_FALLING:
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/examples/neotrellis_simpletest.py` & `adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_simpletest.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 RED = (255, 0, 0)
 YELLOW = (255, 150, 0)
 GREEN = (0, 255, 0)
 CYAN = (0, 255, 255)
 BLUE = (0, 0, 255)
 PURPLE = (180, 0, 255)
 
+
 # this will be called when button events are received
 def blink(event):
     # turn the LED on when a rising edge is detected
     if event.edge == NeoTrellis.EDGE_RISING:
         trellis.pixels[event.number] = CYAN
     # turn the LED off when a falling edge is detected
     elif event.edge == NeoTrellis.EDGE_FALLING:
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.2/pyproject.toml` & `adafruit-circuitpython-neotrellis-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neotrellis"
 description = "CircuitPython library for using Adafruit NeoTrellis."
-version = "1.3.2"
+version = "1.3.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NeoTrellis"}
 keywords = [
     "adafruit",
```

