# Comparing `tmp/adafruit-circuitpython-busdevice-5.2.4.tar.gz` & `tmp/adafruit-circuitpython-busdevice-5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-busdevice-5.2.4.tar", last modified: Tue Mar 28 18:14:18 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-busdevice-5.2.5.tar", last modified: Thu May 18 15:32:22 2023, max compression
```

## Comparing `adafruit-circuitpython-busdevice-5.2.4.tar` & `adafruit-circuitpython-busdevice-5.2.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.127596 adafruit-circuitpython-busdevice-5.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.123596 adafruit-circuitpython-busdevice-5.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.123596 adafruit-circuitpython-busdevice-5.2.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.123596 adafruit-circuitpython-busdevice-5.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.123596 adafruit-circuitpython-busdevice-5.2.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-28 18:14:18.127596 adafruit-circuitpython-busdevice-5.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.123596 adafruit-circuitpython-busdevice-5.2.4/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:10.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_bus_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-03-28 18:14:10.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_bus_device/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-28 18:14:10.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_bus_device/spi_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.123596 adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-28 18:14:18.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-28 18:14:18.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 18:14:18.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-28 18:14:18.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 18:14:18.000000 adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.127596 adafruit-circuitpython-busdevice-5.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.127596 adafruit-circuitpython-busdevice-5.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:14:18.127596 adafruit-circuitpython-busdevice-5.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-28 18:14:10.000000 adafruit-circuitpython-busdevice-5.2.4/examples/busdevice_read_register_i2c_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-28 18:14:10.000000 adafruit-circuitpython-busdevice-5.2.4/examples/busdevice_read_register_spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-28 18:14:10.000000 adafruit-circuitpython-busdevice-5.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-28 18:14:00.000000 adafruit-circuitpython-busdevice-5.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 18:14:18.127596 adafruit-circuitpython-busdevice-5.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.094153 adafruit-circuitpython-busdevice-5.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.082153 adafruit-circuitpython-busdevice-5.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.086153 adafruit-circuitpython-busdevice-5.2.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.086153 adafruit-circuitpython-busdevice-5.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.086153 adafruit-circuitpython-busdevice-5.2.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-18 15:32:22.090153 adafruit-circuitpython-busdevice-5.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.090153 adafruit-circuitpython-busdevice-5.2.5/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:13.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_bus_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-18 15:32:13.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_bus_device/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-18 15:32:13.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_bus_device/spi_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.090153 adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-18 15:32:22.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-18 15:32:22.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:32:22.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 15:32:22.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 15:32:22.000000 adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.090153 adafruit-circuitpython-busdevice-5.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.090153 adafruit-circuitpython-busdevice-5.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:22.090153 adafruit-circuitpython-busdevice-5.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 15:32:13.000000 adafruit-circuitpython-busdevice-5.2.5/examples/busdevice_read_register_i2c_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-18 15:32:13.000000 adafruit-circuitpython-busdevice-5.2.5/examples/busdevice_read_register_spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-18 15:32:13.000000 adafruit-circuitpython-busdevice-5.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-18 15:32:01.000000 adafruit-circuitpython-busdevice-5.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:32:22.094153 adafruit-circuitpython-busdevice-5.2.5/setup.cfg
```

### Comparing `adafruit-circuitpython-busdevice-5.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-busdevice-5.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/.gitignore` & `adafruit-circuitpython-busdevice-5.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/.pre-commit-config.yaml` & `adafruit-circuitpython-busdevice-5.2.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-busdevice-5.2.4/.pylintrc` & `adafruit-circuitpython-busdevice-5.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-busdevice-5.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/LICENSE` & `adafruit-circuitpython-busdevice-5.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-busdevice-5.2.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/LICENSES/MIT.txt` & `adafruit-circuitpython-busdevice-5.2.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-busdevice-5.2.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/PKG-INFO` & `adafruit-circuitpython-busdevice-5.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-busdevice
-Version: 5.2.4
+Version: 5.2.5
 Summary: CircuitPython bus device classes to manage bus sharing.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 Keywords: adafruit,spi,i2c,bus,device,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-busdevice-5.2.4/README.rst` & `adafruit-circuitpython-busdevice-5.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/adafruit_bus_device/i2c_device.py` & `adafruit-circuitpython-busdevice-5.2.5/adafruit_bus_device/i2c_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # Used only for type annotations.
     from busio import I2C
 except ImportError:
     pass
 
 
-__version__ = "5.2.4"
+__version__ = "5.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BusDevice.git"
 
 
 class I2CDevice:
     """
     Represents a single I2C device and manages locking the bus and the device
     address.
@@ -51,15 +51,14 @@
                 device.readinto(bytes_read)
             # A second transaction
             with device:
                 device.write(bytes_read)
     """
 
     def __init__(self, i2c: I2C, device_address: int, probe: bool = True) -> None:
-
         self.i2c = i2c
         self.device_address = device_address
 
         if probe:
             self.__probe_for_device()
 
     def readinto(
```

### Comparing `adafruit-circuitpython-busdevice-5.2.4/adafruit_bus_device/spi_device.py` & `adafruit-circuitpython-busdevice-5.2.5/adafruit_bus_device/spi_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # Used only for type annotations.
     from busio import SPI
     from digitalio import DigitalInOut
 except ImportError:
     pass
 
 
-__version__ = "5.2.4"
+__version__ = "5.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BusDevice.git"
 
 
 class SPIDevice:
     """
     Represents a single SPI device and manages locking the bus and the device
     address.
```

### Comparing `adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/PKG-INFO` & `adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-busdevice
-Version: 5.2.4
+Version: 5.2.5
 Summary: CircuitPython bus device classes to manage bus sharing.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 Keywords: adafruit,spi,i2c,bus,device,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-busdevice-5.2.4/adafruit_circuitpython_busdevice.egg-info/SOURCES.txt` & `adafruit-circuitpython-busdevice-5.2.5/adafruit_circuitpython_busdevice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/docs/_static/favicon.ico` & `adafruit-circuitpython-busdevice-5.2.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/docs/conf.py` & `adafruit-circuitpython-busdevice-5.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/docs/index.rst` & `adafruit-circuitpython-busdevice-5.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/examples/busdevice_read_register_i2c_simpletest.py` & `adafruit-circuitpython-busdevice-5.2.5/examples/busdevice_read_register_i2c_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/examples/busdevice_read_register_spi_simpletest.py` & `adafruit-circuitpython-busdevice-5.2.5/examples/busdevice_read_register_spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-busdevice-5.2.4/pyproject.toml` & `adafruit-circuitpython-busdevice-5.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-busdevice"
 description = "CircuitPython bus device classes to manage bus sharing."
-version = "5.2.4"
+version = "5.2.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BusDevice"}
 keywords = [
     "adafruit",
```

