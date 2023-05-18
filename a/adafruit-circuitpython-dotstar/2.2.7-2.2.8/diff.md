# Comparing `tmp/adafruit-circuitpython-dotstar-2.2.7.tar.gz` & `tmp/adafruit-circuitpython-dotstar-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dotstar-2.2.7.tar", last modified: Sun Mar  5 19:10:05 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-dotstar-2.2.8.tar", last modified: Thu May 18 15:35:31 2023, max compression
```

## Comparing `adafruit-circuitpython-dotstar-2.2.7.tar` & `adafruit-circuitpython-dotstar-2.2.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.345419 adafruit-circuitpython-dotstar-2.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.337418 adafruit-circuitpython-dotstar-2.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.341418 adafruit-circuitpython-dotstar-2.2.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.341418 adafruit-circuitpython-dotstar-2.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.341418 adafruit-circuitpython-dotstar-2.2.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-03-05 19:10:05.345419 adafruit-circuitpython-dotstar-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.341418 adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-03-05 19:10:05.000000 adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-05 19:10:05.000000 adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 19:10:05.000000 adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-05 19:10:05.000000 adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-05 19:10:05.000000 adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-03-05 19:09:57.000000 adafruit-circuitpython-dotstar-2.2.7/adafruit_dotstar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.341418 adafruit-circuitpython-dotstar-2.2.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.341418 adafruit-circuitpython-dotstar-2.2.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 19:10:05.345419 adafruit-circuitpython-dotstar-2.2.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-05 19:09:57.000000 adafruit-circuitpython-dotstar-2.2.7/examples/dotstar_image_paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-03-05 19:09:57.000000 adafruit-circuitpython-dotstar-2.2.7/examples/dotstar_image_pov.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-05 19:09:57.000000 adafruit-circuitpython-dotstar-2.2.7/examples/dotstar_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/examples/hello.png
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/examples/hello.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-05 19:09:57.000000 adafruit-circuitpython-dotstar-2.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-05 19:09:50.000000 adafruit-circuitpython-dotstar-2.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 19:10:05.345419 adafruit-circuitpython-dotstar-2.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.942410 adafruit-circuitpython-dotstar-2.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_dotstar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_pov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/examples/hello.png
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/examples/hello.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/setup.cfg
```

### Comparing `adafruit-circuitpython-dotstar-2.2.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dotstar-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/.gitignore` & `adafruit-circuitpython-dotstar-2.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/.pre-commit-config.yaml` & `adafruit-circuitpython-dotstar-2.2.8/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-dotstar-2.2.7/.pylintrc` & `adafruit-circuitpython-dotstar-2.2.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dotstar-2.2.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/LICENSE` & `adafruit-circuitpython-dotstar-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/LICENSES/MIT.txt` & `adafruit-circuitpython-dotstar-2.2.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dotstar-2.2.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/PKG-INFO` & `adafruit-circuitpython-dotstar-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dotstar
-Version: 2.2.7
+Version: 2.2.8
 Summary: CircuitPython library for DotStar LEDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DotStar
 Keywords: adafruit,dotstar,leds,rgb,spi,addressable,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dotstar-2.2.7/README.rst` & `adafruit-circuitpython-dotstar-2.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/PKG-INFO` & `adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dotstar
-Version: 2.2.7
+Version: 2.2.8
 Summary: CircuitPython library for DotStar LEDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DotStar
 Keywords: adafruit,dotstar,leds,rgb,spi,addressable,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dotstar-2.2.7/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt` & `adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/adafruit_dotstar.py` & `adafruit-circuitpython-dotstar-2.2.8/adafruit_dotstar.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     from typing import Optional, Type
     from types import TracebackType
     from circuitpython_typing import ReadableBuffer
     from microcontroller import Pin
 except ImportError:
     pass
 
-__version__ = "2.2.7"
+__version__ = "2.2.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DotStar.git"
 
 START_HEADER_SIZE = 4
 
 # Pixel color order constants
 RBG = "PRBG"
 """Red Blue Green"""
```

### Comparing `adafruit-circuitpython-dotstar-2.2.7/docs/_static/favicon.ico` & `adafruit-circuitpython-dotstar-2.2.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/docs/conf.py` & `adafruit-circuitpython-dotstar-2.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/docs/index.rst` & `adafruit-circuitpython-dotstar-2.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/examples/dotstar_image_paint.py` & `adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_paint.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 # Calculate gamma correction table, makes mid-range colors look 'right':
 GAMMA = bytearray(256)
 for i in range(256):
     GAMMA[i] = int(pow(float(i) / 255.0, 2.7) * 255.0 + 0.5)
 
 print("Displaying...")
 while True:  # Loop forever
-
     for x in range(WIDTH):  # For each column of image...
         for y in range(HEIGHT):  # For each pixel in column...
             value = PIXELS[x, y]  # Read pixel in image
             DOTS[y] = (  # Set pixel #y in strip
                 GAMMA[value[0]],  # Gamma-corrected red
                 GAMMA[value[1]],  # Gamma-corrected green
                 GAMMA[value[2]],  # Gamma-corrected blue
```

### Comparing `adafruit-circuitpython-dotstar-2.2.7/examples/dotstar_image_pov.py` & `adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_pov.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,11 +63,10 @@
         COLUMN[x][y][0] = GAMMA[value[0]]  # Gamma-corrected R
         COLUMN[x][y][1] = GAMMA[value[1]]  # Gamma-corrected G
         COLUMN[x][y][2] = GAMMA[value[2]]  # Gamma-corrected B
         COLUMN[x][y][3] = 1.0  # Brightness
 
 print("Displaying...")
 while True:  # Loop forever
-
     for x in range(WIDTH):  # For each column of image...
         DOTS[0 : DOTS.n] = COLUMN[x]  # Copy column to DotStar buffer
         DOTS.show()  # Send data to strip
```

### Comparing `adafruit-circuitpython-dotstar-2.2.7/examples/dotstar_simpletest.py` & `adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/examples/hello.png` & `adafruit-circuitpython-dotstar-2.2.8/examples/hello.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.7/pyproject.toml` & `adafruit-circuitpython-dotstar-2.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-dotstar"
 description = "CircuitPython library for DotStar LEDs."
-version = "2.2.7"
+version = "2.2.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DotStar"}
 keywords = [
     "adafruit",
```

