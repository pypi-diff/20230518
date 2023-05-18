# Comparing `tmp/adafruit-circuitpython-pyportal-6.2.8.tar.gz` & `tmp/adafruit-circuitpython-pyportal-6.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pyportal-6.2.8.tar", last modified: Fri Aug 26 02:22:59 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pyportal-6.2.9.tar", last modified: Thu May 18 15:16:13 2023, max compression
```

## Comparing `adafruit-circuitpython-pyportal-6.2.8.tar` & `adafruit-circuitpython-pyportal-6.2.9.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.287456 adafruit-circuitpython-pyportal-6.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-08-26 02:22:59.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-08-26 02:22:59.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:22:59.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-08-26 02:22:59.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-26 02:22:59.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/
--rwxr-xr-x   0 runner    (1001) docker     (121)    14548 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2438 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8180 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/network.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6067 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_internet_json_fetching.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_qrcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)    86828 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_startup.wav
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_startup.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-08-26 02:22:50.000000 adafruit-circuitpython-pyportal-6.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-08-26 02:22:37.000000 adafruit-circuitpython-pyportal-6.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:22:59.291456 adafruit-circuitpython-pyportal-6.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.406834 adafruit-circuitpython-pyportal-6.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.398834 adafruit-circuitpython-pyportal-6.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-18 15:16:13.406834 adafruit-circuitpython-pyportal-6.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-18 15:16:13.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-18 15:16:13.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:16:13.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-18 15:16:13.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 15:16:13.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14547 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2437 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8180 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6067 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:16:13.402834 adafruit-circuitpython-pyportal-6.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_internet_json_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_qrcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86828 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_startup.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_startup.wav.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-18 15:16:06.000000 adafruit-circuitpython-pyportal-6.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-18 15:15:57.000000 adafruit-circuitpython-pyportal-6.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:16:13.406834 adafruit-circuitpython-pyportal-6.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pyportal-6.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/.gitignore` & `adafruit-circuitpython-pyportal-6.2.9/.gitignore`

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

### Comparing `adafruit-circuitpython-pyportal-6.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pyportal-6.2.9/.pre-commit-config.yaml`

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
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/.pylintrc` & `adafruit-circuitpython-pyportal-6.2.9/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pyportal-6.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/LICENSE` & `adafruit-circuitpython-pyportal-6.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pyportal-6.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pyportal-6.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pyportal-6.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/PKG-INFO` & `adafruit-circuitpython-pyportal-6.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pyportal
-Version: 6.2.8
+Version: 6.2.9
 Summary: CircuitPython driver for Adafruit PyPortal
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pyportal,display,iot,wifi,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/README.rst` & `adafruit-circuitpython-pyportal-6.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/PKG-INFO` & `adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pyportal
-Version: 6.2.8
+Version: 6.2.9
 Summary: CircuitPython driver for Adafruit PyPortal
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pyportal,display,iot,wifi,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/adafruit_circuitpython_pyportal.egg-info/SOURCES.txt` & `adafruit-circuitpython-pyportal-6.2.9/adafruit_circuitpython_pyportal.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_pyportal.egg-info/PKG-INFO
 adafruit_circuitpython_pyportal.egg-info/SOURCES.txt
 adafruit_circuitpython_pyportal.egg-info/dependency_links.txt
 adafruit_circuitpython_pyportal.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/__init__.py` & `adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import terminalio
 import supervisor
 from adafruit_portalbase import PortalBase
 from adafruit_pyportal.network import Network, CONTENT_JSON, CONTENT_TEXT
 from adafruit_pyportal.graphics import Graphics
 from adafruit_pyportal.peripherals import Peripherals
 
-__version__ = "6.2.8"
+__version__ = "6.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyPortal.git"
 
 
 class PyPortal(PortalBase):
     """Class representing the Adafruit PyPortal.
 
     :param url: The URL of your data source. Defaults to ``None``.
@@ -121,15 +121,14 @@
         image_url_path=None,
         success_callback=None,
         esp=None,
         external_spi=None,
         debug=False,
         secrets_data=None,
     ):
-
         graphics = Graphics(
             default_bg=default_bg,
             debug=debug,
         )
 
         self._default_bg = default_bg
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/graphics.py` & `adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,30 +22,29 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import board
 from adafruit_portalbase.graphics import GraphicsBase
 
-__version__ = "6.2.8"
+__version__ = "6.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyPortal.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the PyPortal Library
 
     :param default_bg: The path to your default background image file or a hex color.
                        Defaults to 0x000000.
     :param debug: Turn on debug print outs. Defaults to False.
 
     """
 
     # pylint: disable=too-few-public-methods
     def __init__(self, *, default_bg=None, debug=False):
-
         super().__init__(board.DISPLAY, default_bg=default_bg, debug=debug)
         # Tracks whether we've hidden the background when we showed the QR code.
         self._qr_only = False
 
     # pylint: disable=arguments-differ
     def qrcode(self, qr_data, *, qr_size=1, x=0, y=0, hide_background=False):
         """Display a QR code
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/network.py` & `adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     NetworkBase,
     CONTENT_JSON,
     CONTENT_TEXT,
 )
 
 # pylint: enable=unused-import
 
-__version__ = "6.2.8"
+__version__ = "6.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyPortal.git"
 
 # you'll need to pass in an io username, width, height, format (bit depth), io key, and then url!
 IMAGE_CONVERTER_SERVICE = (
     "https://io.adafruit.com/api/v2/%s/integrations/image-formatter?"
     "x-aio-key=%s&width=%d&height=%d&output=BMP%d&url=%s"
 )
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/adafruit_pyportal/peripherals.py` & `adafruit-circuitpython-pyportal-6.2.9/adafruit_pyportal/peripherals.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     NATIVE_SD = True
 except ImportError:
     import adafruit_sdcard as sdcardio
 
     NATIVE_SD = False
 
-__version__ = "6.2.8"
+__version__ = "6.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyPortal.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the PyPortal Library"""
 
     # pylint: disable=too-many-instance-attributes, too-many-locals, too-many-branches, too-many-statements
```

### Comparing `adafruit-circuitpython-pyportal-6.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pyportal-6.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/docs/conf.py` & `adafruit-circuitpython-pyportal-6.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/docs/examples.rst` & `adafruit-circuitpython-pyportal-6.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/docs/index.rst` & `adafruit-circuitpython-pyportal-6.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_internet_json_fetching.py` & `adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_internet_json_fetching.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_qrcode_generation.py` & `adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_qrcode_generation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_simpletest.py` & `adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/examples/pyportal_startup.wav` & `adafruit-circuitpython-pyportal-6.2.9/examples/pyportal_startup.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pyportal-6.2.8/pyproject.toml` & `adafruit-circuitpython-pyportal-6.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pyportal"
 description = "CircuitPython driver for Adafruit PyPortal"
-version = "6.2.8"
+version = "6.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_REPLACE"}
 keywords = [
     "adafruit",
```

