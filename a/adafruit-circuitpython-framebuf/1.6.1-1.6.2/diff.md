# Comparing `tmp/adafruit-circuitpython-framebuf-1.6.1.tar.gz` & `tmp/adafruit-circuitpython-framebuf-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-framebuf-1.6.1.tar", last modified: Mon Apr 24 16:04:37 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-framebuf-1.6.2.tar", last modified: Thu May 18 15:44:06 2023, max compression
```

## Comparing `adafruit-circuitpython-framebuf-1.6.1.tar` & `adafruit-circuitpython-framebuf-1.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.884904 adafruit-circuitpython-framebuf-1.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.888904 adafruit-circuitpython-framebuf-1.6.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.888904 adafruit-circuitpython-framebuf-1.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.888904 adafruit-circuitpython-framebuf-1.6.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-24 16:04:37.000000 adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-24 16:04:37.000000 adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:04:37.000000 adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 16:04:37.000000 adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 16:04:37.000000 adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    23905 2023-04-24 16:04:29.000000 adafruit-circuitpython-framebuf-1.6.1/adafruit_framebuf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/examples/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/examples/font5x8.bin.license
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-24 16:04:29.000000 adafruit-circuitpython-framebuf-1.6.1/examples/framebuf_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-24 16:04:29.000000 adafruit-circuitpython-framebuf-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-24 16:04:19.000000 adafruit-circuitpython-framebuf-1.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:04:37.892904 adafruit-circuitpython-framebuf-1.6.1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    38225 2023-04-24 16:04:29.000000 adafruit-circuitpython-framebuf-1.6.1/utils/font_to_bin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.751575 adafruit-circuitpython-framebuf-1.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23905 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_framebuf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/examples/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/examples/font5x8.bin.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/examples/framebuf_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/utils/font_to_bin.py
```

### Comparing `adafruit-circuitpython-framebuf-1.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-framebuf-1.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/.gitignore` & `adafruit-circuitpython-framebuf-1.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/.pre-commit-config.yaml` & `adafruit-circuitpython-framebuf-1.6.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-framebuf-1.6.1/.pylintrc` & `adafruit-circuitpython-framebuf-1.6.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-framebuf-1.6.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/LICENSE` & `adafruit-circuitpython-framebuf-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-framebuf-1.6.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/LICENSES/MIT.txt` & `adafruit-circuitpython-framebuf-1.6.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-framebuf-1.6.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/PKG-INFO` & `adafruit-circuitpython-framebuf-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-framebuf
-Version: 1.6.1
+Version: 1.6.2
 Summary: CircuitPython frambuf module, based on the Python frambuf module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_framebuf
 Keywords: adafruit,display,framebuf,framebuffer,software,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-framebuf-1.6.1/README.rst` & `adafruit-circuitpython-framebuf-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/PKG-INFO` & `adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-framebuf
-Version: 1.6.1
+Version: 1.6.2
 Summary: CircuitPython frambuf module, based on the Python frambuf module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_framebuf
 Keywords: adafruit,display,framebuf,framebuffer,software,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-framebuf-1.6.1/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt` & `adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/adafruit_framebuf.py` & `adafruit-circuitpython-framebuf-1.6.2/adafruit_framebuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_framebuf.git"
 
 import os
 import struct
 
 # Framebuf format constants:
 MVLSB = 0  # Single bit displays (like SSD1306 OLED)
```

### Comparing `adafruit-circuitpython-framebuf-1.6.1/docs/_static/favicon.ico` & `adafruit-circuitpython-framebuf-1.6.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/docs/conf.py` & `adafruit-circuitpython-framebuf-1.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/docs/index.rst` & `adafruit-circuitpython-framebuf-1.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/examples/font5x8.bin` & `adafruit-circuitpython-framebuf-1.6.2/examples/font5x8.bin`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/examples/framebuf_simpletest.py` & `adafruit-circuitpython-framebuf-1.6.2/examples/framebuf_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.1/pyproject.toml` & `adafruit-circuitpython-framebuf-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-framebuf"
 description = "CircuitPython frambuf module, based on the Python frambuf module."
-version = "1.6.1"
+version = "1.6.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_framebuf"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-framebuf-1.6.1/utils/font_to_bin.py` & `adafruit-circuitpython-framebuf-1.6.2/utils/font_to_bin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2568,15 +2568,14 @@
     ".....",
     ".....",
     ".....",
 )
 # fmt: on
 
 if __name__ == "__main__":
-
     # Rotate all character to be able to generate the correct data
     rotated_font = []
     char = []
     for i, col in enumerate(FONT):
         char.append(col)
         # Has all character data been appended
         if (i + 1) % HEIGHT == 0:
```

