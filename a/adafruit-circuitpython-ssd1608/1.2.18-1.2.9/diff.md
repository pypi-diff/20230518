# Comparing `tmp/adafruit-circuitpython-ssd1608-1.2.18.tar.gz` & `tmp/adafruit-circuitpython-ssd1608-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1608-1.2.18.tar", last modified: Thu May 18 15:22:29 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1608-1.2.9.tar", last modified: Mon Aug 16 17:49:23 2021, max compression
```

## Comparing `adafruit-circuitpython-ssd1608-1.2.18.tar` & `adafruit-circuitpython-ssd1608-1.2.9.tar`

### file list

```diff
@@ -1,49 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.654249 adafruit-circuitpython-ssd1608-1.2.18/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.650248 adafruit-circuitpython-ssd1608-1.2.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.650248 adafruit-circuitpython-ssd1608-1.2.18/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.650248 adafruit-circuitpython-ssd1608-1.2.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.650248 adafruit-circuitpython-ssd1608-1.2.18/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-18 15:22:29.654249 adafruit-circuitpython-ssd1608-1.2.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.650248 adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-18 15:22:29.000000 adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-18 15:22:29.000000 adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:22:29.000000 adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:22:29.000000 adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:22:29.000000 adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 15:22:21.000000 adafruit-circuitpython-ssd1608-1.2.18/adafruit_ssd1608.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.654249 adafruit-circuitpython-ssd1608-1.2.18/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.654249 adafruit-circuitpython-ssd1608-1.2.18/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:22:29.654249 adafruit-circuitpython-ssd1608-1.2.18/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   360122 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-18 15:22:21.000000 adafruit-circuitpython-ssd1608-1.2.18/examples/ssd1608_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-18 15:22:21.000000 adafruit-circuitpython-ssd1608-1.2.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:22:10.000000 adafruit-circuitpython-ssd1608-1.2.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:22:29.654249 adafruit-circuitpython-ssd1608-1.2.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.214142 adafruit-circuitpython-ssd1608-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.214142 adafruit-circuitpython-ssd1608-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.214142 adafruit-circuitpython-ssd1608-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16326 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5221 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3450 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5221 2021-08-16 17:49:23.000000 adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-08-16 17:49:23.000000 adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-16 17:49:23.000000 adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-08-16 17:49:23.000000 adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-16 17:49:23.000000 adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/adafruit_ssd1608.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5433 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/examples/ssd1608_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-16 17:49:23.218142 adafruit-circuitpython-ssd1608-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-08-16 17:49:12.000000 adafruit-circuitpython-ssd1608-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1608-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 Thank you for contributing! Before you submit a pull request, please read the following.
 
-Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://docs.circuitpython.org/en/latest/docs/design_guide.html
+Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://circuitpython.readthedocs.io/en/latest/docs/design_guide.html
 
 If your changes are to documentation, please verify that the documentation builds locally by following the steps found here: https://adafru.it/build-docs
 
 Before submitting the pull request, make sure you've run Pylint and Black locally on your code. You can do this manually or using pre-commit. Instructions are available here: https://adafru.it/check-your-code
 
 Please remove all of this text before submitting. Include an explanation or list of changes included in your PR, as well as, if applicable, a link to any related issues.
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1608-1.2.9/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
-  - repo: https://github.com/python/black
-    rev: 23.3.0
+-   repo: https://github.com/python/black
+    rev: 20.8b1
     hooks:
-      - id: black
-  - repo: https://github.com/fsfe/reuse-tool
-    rev: v1.1.2
+    - id: black
+-   repo: https://github.com/fsfe/reuse-tool
+    rev: v0.12.1
     hooks:
-      - id: reuse
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    - id: reuse
+-   repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v2.3.0
     hooks:
-      - id: check-yaml
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
-  - repo: https://github.com/pycqa/pylint
-    rev: v2.17.4
+    -   id: check-yaml
+    -   id: end-of-file-fixer
+    -   id: trailing-whitespace
+-   repo: https://github.com/pycqa/pylint
+    rev: pylint-2.7.1
     hooks:
-      - id: pylint
+    -   id: pylint
         name: pylint (library code)
         types: [python]
-        args:
-          - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
-      - id: pylint
-        name: pylint (example code)
+        exclude: "^(docs/|examples/|setup.py$)"
+-   repo: local
+    hooks:
+    -   id: pylint_examples
+        name: pylint (examples code)
         description: Run pylint rules on "examples/*.py" files
-        types: [python]
-        files: "^examples/"
-        args:
-          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
+        entry: /usr/bin/env bash -c
+        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
+        language: system
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/.pylintrc` & `adafruit-circuitpython-ssd1608-1.2.9/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
+# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+#
+# SPDX-License-Identifier: Unlicense
+
+# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the ignore-list. They should be base names, not
+# Add files or directories to the blacklist. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the ignore-list. The
+# Add files or directories matching the regex patterns to the blacklist. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=pylint.extensions.no_self_use
+load-plugins=
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +54,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
-disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
+# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
+disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,14 +225,20 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
+# List of optional constructs for which whitespace checking is disabled. `dict-
+# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
+# `trailing-comma` allows a space between comma and closing bracket: (a, ).
+# `empty-line` allows space-only lines.
+no-space-check=trailing-comma,dict-separator
+
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -247,53 +257,81 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
+# Naming hint for argument names
+argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
+# Naming hint for attribute names
+attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
+# Naming hint for class attribute names
+class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
+
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
+# Naming hint for class names
+# class-name-hint=[A-Z_][a-zA-Z0-9]+$
+class-name-hint=[A-Z_][a-zA-Z0-9_]+$
+
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
+# Naming hint for constant names
+const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
+
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
+# Naming hint for function names
+function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
+# Naming hint for inline iteration names
+inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
+
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
+# Naming hint for method names
+method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
+# Naming hint for module names
+module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
+
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -301,14 +339,17 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
+# Naming hint for variable names
+variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1608-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/LICENSE` & `adafruit-circuitpython-ssd1608-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1608-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1608-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1608-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/PKG-INFO` & `adafruit-circuitpython-ssd1608-1.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,137 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1608
-Version: 1.2.18
+Version: 1.2.9
 Summary: CircuitPython `displayio` drivers for SSD1608-based ePaper displays
-Author-email: Adafruit Industries <circuitpython@adafruit.com>
+Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608
+Author: Adafruit Industries
+Author-email: circuitpython@adafruit.com
 License: MIT
-Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1608
-Keywords: adafruit,blinka,circuitpython,micropython,ssd1608,displayio,epd,epaper
+Description: Introduction
+        ============
+        
+        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1608/badge/?version=latest
+            :target: https://circuitpython.readthedocs.io/projects/ssd1608/en/latest/
+            :alt: Documentation Status
+        
+        .. image:: https://img.shields.io/discord/327254708534116352.svg
+            :target: https://adafru.it/discord
+            :alt: Discord
+        
+        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/workflows/Build%20CI/badge.svg
+            :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/actions/
+            :alt: Build Status
+        
+        CircuitPython `displayio` driver for SSD1608-based ePaper displays
+        
+        Dependencies
+        =============
+        This driver depends on:
+        
+        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+        
+        Please ensure all dependencies are available on the CircuitPython filesystem.
+        This is easily achieved by downloading
+        `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+        
+        Installing from PyPI
+        =====================
+        
+        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+        PyPI <https://pypi.org/project/adafruit-circuitpython-ssd1608/>`_. To install for current user:
+        
+        .. code-block:: shell
+        
+            pip3 install adafruit-circuitpython-ssd1608
+        
+        To install system-wide (this may be required in some cases):
+        
+        .. code-block:: shell
+        
+            sudo pip3 install adafruit-circuitpython-ssd1608
+        
+        To install in a virtual environment in your current project:
+        
+        .. code-block:: shell
+        
+            mkdir project-name && cd project-name
+            python3 -m venv .env
+            source .env/bin/activate
+            pip3 install adafruit-circuitpython-ssd1608
+        
+        Usage Example
+        =============
+        
+        .. code-block:: python
+        
+            """Simple test script for 1.54" 200x200 monochrome display.
+        
+            Supported products:
+              * Adafruit 1.54" Monochrome ePaper Display Breakout
+                * https://www.adafruit.com/product/4196
+              """
+        
+            import time
+            import board
+            import displayio
+            import adafruit_ssd1608
+        
+            displayio.release_displays()
+        
+            # This pinout works on a Feather M4 and may need to be altered for other boards.
+            spi = board.SPI() # Uses SCK and MOSI
+            epd_cs = board.D9
+            epd_dc = board.D10
+            epd_reset = board.D5
+            epd_busy = board.D6
+        
+            display_bus = displayio.FourWire(spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset,
+                                             baudrate=1000000)
+            time.sleep(1)
+        
+            display = adafruit_ssd1608.SSD1608(display_bus, width=200, height=200, busy_pin=epd_busy)
+        
+            g = displayio.Group()
+        
+            f = open("/display-ruler.bmp", "rb")
+        
+            pic = displayio.OnDiskBitmap(f)
+            # CircuitPython 6 & 7 compatible
+            t = displayio.TileGrid(
+                pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+            )
+            # CircuitPython 7 compatible only
+            # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
+            g.append(t)
+        
+            display.show(g)
+        
+            display.refresh()
+        
+            print("refreshed")
+        
+            time.sleep(120)
+        
+        Contributing
+        ============
+        
+        Contributions are welcome! Please read our `Code of Conduct
+        <https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/blob/main/CODE_OF_CONDUCT.md>`_
+        before contributing to help this project stay welcoming.
+        
+        Documentation
+        =============
+        
+        For information on building library documentation, please check out `this guide
+        <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+        
+Keywords: adafruit blinka circuitpython micropython ssd1608 displayio epd epaper
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
-License-File: LICENSE
-
-Introduction
-============
-
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1608/badge/?version=latest
-    :target: https://docs.circuitpython.org/projects/ssd1608/en/latest/
-    :alt: Documentation Status
-
-.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
-    :target: https://adafru.it/discord
-    :alt: Discord
-
-.. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/workflows/Build%20CI/badge.svg
-    :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/actions/
-    :alt: Build Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Code Style: Black
-
-CircuitPython `displayio` driver for SSD1608-based ePaper displays
-
-Dependencies
-=============
-This driver depends on:
-
-* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-
-Please ensure all dependencies are available on the CircuitPython filesystem.
-This is easily achieved by downloading
-`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-
-Installing from PyPI
-=====================
-
-On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-PyPI <https://pypi.org/project/adafruit-circuitpython-ssd1608/>`_. To install for current user:
-
-.. code-block:: shell
-
-    pip3 install adafruit-circuitpython-ssd1608
-
-To install system-wide (this may be required in some cases):
-
-.. code-block:: shell
-
-    sudo pip3 install adafruit-circuitpython-ssd1608
-
-To install in a virtual environment in your current project:
-
-.. code-block:: shell
-
-    mkdir project-name && cd project-name
-    python3 -m venv .venv
-    source .venv/bin/activate
-    pip3 install adafruit-circuitpython-ssd1608
-
-Usage Example
-=============
-
-.. code-block:: python
-
-    """Simple test script for 1.54" 200x200 monochrome display.
-
-    Supported products:
-      * Adafruit 1.54" Monochrome ePaper Display Breakout
-        * https://www.adafruit.com/product/4196
-      """
-
-    import time
-    import board
-    import displayio
-    import adafruit_ssd1608
-
-    displayio.release_displays()
-
-    # This pinout works on a Feather M4 and may need to be altered for other boards.
-    spi = board.SPI() # Uses SCK and MOSI
-    epd_cs = board.D9
-    epd_dc = board.D10
-    epd_reset = board.D5
-    epd_busy = board.D6
-
-    display_bus = displayio.FourWire(spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset,
-                                     baudrate=1000000)
-    time.sleep(1)
-
-    display = adafruit_ssd1608.SSD1608(display_bus, width=200, height=200, busy_pin=epd_busy)
-
-    g = displayio.Group()
-
-    f = open("/display-ruler.bmp", "rb")
-
-    pic = displayio.OnDiskBitmap(f)
-    # CircuitPython 6 & 7 compatible
-    t = displayio.TileGrid(
-        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
-    )
-    # CircuitPython 7 compatible only
-    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
-    g.append(t)
-
-    display.show(g)
-
-    display.refresh()
-
-    print("refreshed")
-
-    time.sleep(120)
-
-Documentation
-=============
-
-API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1608/en/latest/>`_.
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-Contributing
-============
-
-Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/blob/main/CODE_OF_CONDUCT.md>`_
-before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/README.rst` & `adafruit-circuitpython-ssd1608-1.2.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1608/badge/?version=latest
-    :target: https://docs.circuitpython.org/projects/ssd1608/en/latest/
+    :target: https://circuitpython.readthedocs.io/projects/ssd1608/en/latest/
     :alt: Documentation Status
 
-.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
+.. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/actions/
     :alt: Build Status
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Code Style: Black
-
 CircuitPython `displayio` driver for SSD1608-based ePaper displays
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -46,16 +42,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1608
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .venv
-    source .venv/bin/activate
+    python3 -m venv .env
+    source .env/bin/activate
     pip3 install adafruit-circuitpython-ssd1608
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -103,20 +99,19 @@
 
     display.refresh()
 
     print("refreshed")
 
     time.sleep(120)
 
-Documentation
-=============
-
-API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1608/en/latest/>`_.
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide
+<https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,137 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1608
-Version: 1.2.18
+Version: 1.2.9
 Summary: CircuitPython `displayio` drivers for SSD1608-based ePaper displays
-Author-email: Adafruit Industries <circuitpython@adafruit.com>
+Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608
+Author: Adafruit Industries
+Author-email: circuitpython@adafruit.com
 License: MIT
-Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1608
-Keywords: adafruit,blinka,circuitpython,micropython,ssd1608,displayio,epd,epaper
+Description: Introduction
+        ============
+        
+        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1608/badge/?version=latest
+            :target: https://circuitpython.readthedocs.io/projects/ssd1608/en/latest/
+            :alt: Documentation Status
+        
+        .. image:: https://img.shields.io/discord/327254708534116352.svg
+            :target: https://adafru.it/discord
+            :alt: Discord
+        
+        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/workflows/Build%20CI/badge.svg
+            :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/actions/
+            :alt: Build Status
+        
+        CircuitPython `displayio` driver for SSD1608-based ePaper displays
+        
+        Dependencies
+        =============
+        This driver depends on:
+        
+        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+        
+        Please ensure all dependencies are available on the CircuitPython filesystem.
+        This is easily achieved by downloading
+        `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+        
+        Installing from PyPI
+        =====================
+        
+        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+        PyPI <https://pypi.org/project/adafruit-circuitpython-ssd1608/>`_. To install for current user:
+        
+        .. code-block:: shell
+        
+            pip3 install adafruit-circuitpython-ssd1608
+        
+        To install system-wide (this may be required in some cases):
+        
+        .. code-block:: shell
+        
+            sudo pip3 install adafruit-circuitpython-ssd1608
+        
+        To install in a virtual environment in your current project:
+        
+        .. code-block:: shell
+        
+            mkdir project-name && cd project-name
+            python3 -m venv .env
+            source .env/bin/activate
+            pip3 install adafruit-circuitpython-ssd1608
+        
+        Usage Example
+        =============
+        
+        .. code-block:: python
+        
+            """Simple test script for 1.54" 200x200 monochrome display.
+        
+            Supported products:
+              * Adafruit 1.54" Monochrome ePaper Display Breakout
+                * https://www.adafruit.com/product/4196
+              """
+        
+            import time
+            import board
+            import displayio
+            import adafruit_ssd1608
+        
+            displayio.release_displays()
+        
+            # This pinout works on a Feather M4 and may need to be altered for other boards.
+            spi = board.SPI() # Uses SCK and MOSI
+            epd_cs = board.D9
+            epd_dc = board.D10
+            epd_reset = board.D5
+            epd_busy = board.D6
+        
+            display_bus = displayio.FourWire(spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset,
+                                             baudrate=1000000)
+            time.sleep(1)
+        
+            display = adafruit_ssd1608.SSD1608(display_bus, width=200, height=200, busy_pin=epd_busy)
+        
+            g = displayio.Group()
+        
+            f = open("/display-ruler.bmp", "rb")
+        
+            pic = displayio.OnDiskBitmap(f)
+            # CircuitPython 6 & 7 compatible
+            t = displayio.TileGrid(
+                pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+            )
+            # CircuitPython 7 compatible only
+            # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
+            g.append(t)
+        
+            display.show(g)
+        
+            display.refresh()
+        
+            print("refreshed")
+        
+            time.sleep(120)
+        
+        Contributing
+        ============
+        
+        Contributions are welcome! Please read our `Code of Conduct
+        <https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/blob/main/CODE_OF_CONDUCT.md>`_
+        before contributing to help this project stay welcoming.
+        
+        Documentation
+        =============
+        
+        For information on building library documentation, please check out `this guide
+        <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+        
+Keywords: adafruit blinka circuitpython micropython ssd1608 displayio epd epaper
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
-License-File: LICENSE
-
-Introduction
-============
-
-.. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1608/badge/?version=latest
-    :target: https://docs.circuitpython.org/projects/ssd1608/en/latest/
-    :alt: Documentation Status
-
-.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
-    :target: https://adafru.it/discord
-    :alt: Discord
-
-.. image:: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/workflows/Build%20CI/badge.svg
-    :target: https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/actions/
-    :alt: Build Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Code Style: Black
-
-CircuitPython `displayio` driver for SSD1608-based ePaper displays
-
-Dependencies
-=============
-This driver depends on:
-
-* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-
-Please ensure all dependencies are available on the CircuitPython filesystem.
-This is easily achieved by downloading
-`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-
-Installing from PyPI
-=====================
-
-On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-PyPI <https://pypi.org/project/adafruit-circuitpython-ssd1608/>`_. To install for current user:
-
-.. code-block:: shell
-
-    pip3 install adafruit-circuitpython-ssd1608
-
-To install system-wide (this may be required in some cases):
-
-.. code-block:: shell
-
-    sudo pip3 install adafruit-circuitpython-ssd1608
-
-To install in a virtual environment in your current project:
-
-.. code-block:: shell
-
-    mkdir project-name && cd project-name
-    python3 -m venv .venv
-    source .venv/bin/activate
-    pip3 install adafruit-circuitpython-ssd1608
-
-Usage Example
-=============
-
-.. code-block:: python
-
-    """Simple test script for 1.54" 200x200 monochrome display.
-
-    Supported products:
-      * Adafruit 1.54" Monochrome ePaper Display Breakout
-        * https://www.adafruit.com/product/4196
-      """
-
-    import time
-    import board
-    import displayio
-    import adafruit_ssd1608
-
-    displayio.release_displays()
-
-    # This pinout works on a Feather M4 and may need to be altered for other boards.
-    spi = board.SPI() # Uses SCK and MOSI
-    epd_cs = board.D9
-    epd_dc = board.D10
-    epd_reset = board.D5
-    epd_busy = board.D6
-
-    display_bus = displayio.FourWire(spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset,
-                                     baudrate=1000000)
-    time.sleep(1)
-
-    display = adafruit_ssd1608.SSD1608(display_bus, width=200, height=200, busy_pin=epd_busy)
-
-    g = displayio.Group()
-
-    f = open("/display-ruler.bmp", "rb")
-
-    pic = displayio.OnDiskBitmap(f)
-    # CircuitPython 6 & 7 compatible
-    t = displayio.TileGrid(
-        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
-    )
-    # CircuitPython 7 compatible only
-    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
-    g.append(t)
-
-    display.show(g)
-
-    display.refresh()
-
-    print("refreshed")
-
-    time.sleep(120)
-
-Documentation
-=============
-
-API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ssd1608/en/latest/>`_.
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-Contributing
-============
-
-Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/blob/main/CODE_OF_CONDUCT.md>`_
-before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/adafruit_circuitpython_ssd1608.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1608-1.2.9/adafruit_circuitpython_ssd1608.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yaml
+.readthedocs.yml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_ssd1608.py
-optional_requirements.txt
-pyproject.toml
 requirements.txt
+setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release_gh.yml
-.github/workflows/release_pypi.yml
+.github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ssd1608.egg-info/PKG-INFO
 adafruit_circuitpython_ssd1608.egg-info/SOURCES.txt
 adafruit_circuitpython_ssd1608.egg-info/dependency_links.txt
 adafruit_circuitpython_ssd1608.egg-info/requires.txt
@@ -26,13 +24,10 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
-docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
-examples/display-ruler.bmp
-examples/display-ruler.bmp.license
 examples/ssd1608_simpletest.py
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/adafruit_ssd1608.py` & `adafruit-circuitpython-ssd1608-1.2.9/adafruit_ssd1608.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Adafruit CircuitPython firmware (version 5+) for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.2.18"
+__version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1608.git"
 
 _START_SEQUENCE = (
     b"\x12\x00"  # Software reset
     b"\x01\x03\x00\x00\x00"  # driver output control
     b"\x3a\x01\x1b"  # Set dummy line period
     b"\x3b\x01\x0b"  # Set gate line width
@@ -40,20 +40,19 @@
     b"\x32\x1e\x02\x02\x01\x11\x12\x12\x22\x22\x66\x69\x69\x59\x58\x99\x99\x88\x00\x00\x00\x00\xf8"
     b"\xb4\x13\x51\x35\x51\x51\x19\x01\x00"  # LUT
     b"\x22\x01\xc7"  # Set DISP ctrl2
 )
 
 _STOP_SEQUENCE = b"\x10\x01\x01"  # Enter deep sleep
 
-
 # pylint: disable=too-few-public-methods
 class SSD1608(displayio.EPaperDisplay):
     """SSD1608 driver"""
 
-    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
+    def __init__(self, bus, **kwargs):
         start_sequence = bytearray(_START_SEQUENCE)
         width = kwargs["width"]
         start_sequence[4] = (width - 1) & 0xFF
         start_sequence[5] = (width - 1) >> 8
 
         super().__init__(
             bus,
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1608-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/docs/conf.py` & `adafruit-circuitpython-ssd1608-1.2.9/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
-import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -26,36 +25,29 @@
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 autodoc_mock_imports = ["displayio"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3", None),
-    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
+    "python": ("https://docs.python.org/3.4", None),
+    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit SSD1608 Library"
-creation_year = "2019"
-current_year = str(datetime.datetime.now().year)
-year_duration = (
-    current_year
-    if current_year == creation_year
-    else creation_year + " - " + current_year
-)
-copyright = year_duration + " Scott Shawcroft"
+copyright = "2019 Scott Shawcroft"
 author = "Scott Shawcroft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
@@ -64,15 +56,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = "en"
+language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/docs/index.rst` & `adafruit-circuitpython-ssd1608-1.2.9/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -29,17 +29,16 @@
     :caption: Related Products
 
     Adafruit 1.54" Monochrome ePaper Display Breakout <https://www.adafruit.com/product/4196>
 
 .. toctree::
     :caption: Other Links
 
-    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/releases/latest>
-    Download Library Bundle <https://circuitpython.org/libraries>
-    CircuitPython Reference Documentation <https://docs.circuitpython.org>
+    Download <https://github.com/adafruit/Adafruit_CircuitPython_SSD1608/releases/latest>
+    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ssd1608-1.2.18/examples/ssd1608_simpletest.py` & `adafruit-circuitpython-ssd1608-1.2.9/examples/ssd1608_simpletest.py`

 * *Files identical despite different names*

