# Comparing `tmp/adafruit-circuitpython-pybadger-3.7.8.tar.gz` & `tmp/adafruit-circuitpython-pybadger-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pybadger-3.7.8.tar", last modified: Tue Sep 13 23:47:18 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pybadger-3.7.9.tar", last modified: Tue Nov 15 17:43:50 2022, max compression
```

## Comparing `adafruit-circuitpython-pybadger-3.7.8.tar` & `adafruit-circuitpython-pybadger-3.7.9.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.111950 adafruit-circuitpython-pybadger-3.7.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.099950 adafruit-circuitpython-pybadger-3.7.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.099950 adafruit-circuitpython-pybadger-3.7.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.103950 adafruit-circuitpython-pybadger-3.7.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.103950 adafruit-circuitpython-pybadger-3.7.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17967 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-09-13 23:47:18.107950 adafruit-circuitpython-pybadger-3.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.103950 adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-09-13 23:47:18.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-09-13 23:47:18.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 23:47:18.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-13 23:47:18.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-13 23:47:18.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.103950 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/clue.py
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/cpb_gizmo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/magtag.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pewpewm4.py
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pybadge.py
--rw-r--r--   0 runner    (1001) docker     (121)    31860 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pybadger_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pygamer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pyportal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.107950 adafruit-circuitpython-pybadger-3.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.107950 adafruit-circuitpython-pybadger-3.7.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5915 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.107950 adafruit-circuitpython-pybadger-3.7.8/docs/mocks/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/mocks/keypad.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:47:18.107950 adafruit-circuitpython-pybadger-3.7.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)    61494 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   115256 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_CLUE.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_CLUE.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    38966 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_MagTag.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_MagTag.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    11382 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_PewPewM4.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_PewPewM4.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    42102 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_PyPortal.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_PyPortal.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    38470 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/QR_Blinka_CircuitPythonOrg.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/examples/QR_Blinka_CircuitPythonOrg.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_button_debouncing.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_clue_custom_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_clue_custom_image_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_custom_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_pewpewm4_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_pygamer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_pyportal_touchscreen.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-09-13 23:47:09.000000 adafruit-circuitpython-pybadger-3.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-13 23:46:59.000000 adafruit-circuitpython-pybadger-3.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-13 23:47:18.111950 adafruit-circuitpython-pybadger-3.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.605360 adafruit-circuitpython-pybadger-3.7.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.593360 adafruit-circuitpython-pybadger-3.7.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.597360 adafruit-circuitpython-pybadger-3.7.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.597360 adafruit-circuitpython-pybadger-3.7.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.597360 adafruit-circuitpython-pybadger-3.7.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17967 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-11-15 17:43:50.605360 adafruit-circuitpython-pybadger-3.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.597360 adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-11-15 17:43:50.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-11-15 17:43:50.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 17:43:50.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-15 17:43:50.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-15 17:43:50.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.601360 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/clue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/cpb_gizmo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/magtag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pewpewm4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pybadge.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31860 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pybadger_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pygamer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pyportal.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.601360 adafruit-circuitpython-pybadger-3.7.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.601360 adafruit-circuitpython-pybadger-3.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5915 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.601360 adafruit-circuitpython-pybadger-3.7.9/docs/mocks/
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/mocks/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:43:50.605360 adafruit-circuitpython-pybadger-3.7.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    61494 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   115256 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_CLUE.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_CLUE.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    38966 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_MagTag.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_MagTag.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    11382 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_PewPewM4.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_PewPewM4.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    42102 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_PyPortal.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_PyPortal.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    38470 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/QR_Blinka_CircuitPythonOrg.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/examples/QR_Blinka_CircuitPythonOrg.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_button_debouncing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_clue_custom_badge.py
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_clue_custom_image_badge.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_custom_badge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_pewpewm4_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_pygamer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_pyportal_touchscreen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-11-15 17:43:40.000000 adafruit-circuitpython-pybadger-3.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-15 17:43:28.000000 adafruit-circuitpython-pybadger-3.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 17:43:50.605360 adafruit-circuitpython-pybadger-3.7.9/setup.cfg
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pybadger-3.7.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/.gitignore` & `adafruit-circuitpython-pybadger-3.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pybadger-3.7.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/.pylintrc` & `adafruit-circuitpython-pybadger-3.7.9/.pylintrc`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
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

### Comparing `adafruit-circuitpython-pybadger-3.7.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pybadger-3.7.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/LICENSE` & `adafruit-circuitpython-pybadger-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pybadger-3.7.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-pybadger-3.7.9/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pybadger-3.7.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pybadger-3.7.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/PKG-INFO` & `adafruit-circuitpython-pybadger-3.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pybadger
-Version: 3.7.8
+Version: 3.7.9
 Summary: Badge-focused CircuitPython helper library for PyBadge, PyBadge LC, PyGamer and CLUE
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pybadge,pygamer,clue,display,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/README.rst` & `adafruit-circuitpython-pybadger-3.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/PKG-INFO` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pybadger
-Version: 3.7.8
+Version: 3.7.9
 Summary: Badge-focused CircuitPython helper library for PyBadge, PyBadge LC, PyGamer and CLUE
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pybadge,pygamer,clue,display,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_circuitpython_pybadger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

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
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_pybadger.egg-info/PKG-INFO
 adafruit_circuitpython_pybadger.egg-info/SOURCES.txt
 adafruit_circuitpython_pybadger.egg-info/dependency_links.txt
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/__init__.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/clue.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/clue.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import board
 import audiopwmio
 import keypad
 import adafruit_lsm6ds.lsm6ds33
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "a b")
 
 try:
     from typing import Type
 except ImportError:
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/cpb_gizmo.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/cpb_gizmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 try:
     from typing import Type
 except ImportError:
     pass
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "a b")
 
 
 class CPB_Gizmo(PyBadgerBase):
     """Class that represents a single Circuit Playground Bluefruit with TFT Gizmo."""
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/magtag.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/magtag.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from adafruit_pybadger.pybadger_base import PyBadgerBase
 
 try:
     from typing import Type
 except ImportError:
     pass
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "a b c d")
 
 
 class MagTag(PyBadgerBase):
     """Class that represents a single Mag Tag."""
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pewpewm4.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pewpewm4.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 try:
     from typing import Type
 except ImportError:
     pass
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", ("o", "x", "z", "right", "down", "up", "left"))
 
 
 class PewPewM4(PyBadgerBase):
     """Class that represents a single Pew Pew M4."""
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pybadge.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pybadge.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 try:
     from typing import Type
 except ImportError:
     pass
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "b a start select right down up left")
 
 
 class PyBadge(PyBadgerBase):
     """Class that represents a single PyBadge, PyBadge LC, or EdgeBadge."""
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pybadger_base.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pybadger_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     from adafruit_bitmap_font.bdf import BDF  # pylint: disable=ungrouped-imports
     from adafruit_bitmap_font.pcf import PCF  # pylint: disable=ungrouped-imports
     from fontio import BuiltinFont
     from keypad import Keys, ShiftRegisterKeys
     from neopixel import NeoPixel
 
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 
 def load_font(fontname: str, text: str) -> Union[BDF, PCF]:
     """Load a font and glyphs in the text string
 
     :param str fontname: The full path to the font file.
@@ -395,18 +395,18 @@
     def _check_for_movement(self, movement_threshold: int = 10) -> bool:
         """Checks to see if board is moving. Used to auto-dim display when not moving."""
         current_accelerometer = self.acceleration
         if self._last_accelerometer is None:
             self._last_accelerometer = current_accelerometer
             return False
         acceleration_delta = sum(
-            [
+            (
                 abs(self._last_accelerometer[n] - current_accelerometer[n])
                 for n in range(3)
-            ]
+            )
         )
         self._last_accelerometer = current_accelerometer
         return acceleration_delta > movement_threshold
 
     def auto_dim_display(self, delay: float = 5.0, movement_threshold: int = 10):
         """Auto-dim the display when board is not moving.
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pygamer.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pygamer.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from adafruit_pybadger.pybadger_base import PyBadgerBase, KeyStates
 
 try:
     from typing import Type, Tuple
 except ImportError:
     pass
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 Buttons = namedtuple("Buttons", "b a start select right down up left")
 
 
 class PyGamer(PyBadgerBase):
     """Class that represents a single PyGamer."""
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/adafruit_pybadger/pyportal.py` & `adafruit-circuitpython-pybadger-3.7.9/adafruit_pybadger/pyportal.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 import board
 import analogio
 import audioio
 import neopixel
 from adafruit_pybadger.pybadger_base import PyBadgerBase
 
-__version__ = "3.7.8"
+__version__ = "3.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PyBadger.git"
 
 
 class PyPortal(PyBadgerBase):
     """Class that represents a single PyPortal."""
 
     _audio_out = audioio.AudioOut
```

### Comparing `adafruit-circuitpython-pybadger-3.7.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pybadger-3.7.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/docs/api.rst` & `adafruit-circuitpython-pybadger-3.7.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/docs/conf.py` & `adafruit-circuitpython-pybadger-3.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/docs/index.rst` & `adafruit-circuitpython-pybadger-3.7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/docs/mocks/keypad.py` & `adafruit-circuitpython-pybadger-3.7.9/docs/mocks/keypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/Blinka.bmp` & `adafruit-circuitpython-pybadger-3.7.9/examples/Blinka.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_CLUE.bmp` & `adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_CLUE.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_MagTag.bmp` & `adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_MagTag.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_PewPewM4.bmp` & `adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_PewPewM4.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/Blinka_PyPortal.bmp` & `adafruit-circuitpython-pybadger-3.7.9/examples/Blinka_PyPortal.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/QR_Blinka_CircuitPythonOrg.bmp` & `adafruit-circuitpython-pybadger-3.7.9/examples/QR_Blinka_CircuitPythonOrg.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_button_debouncing.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_button_debouncing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_clue_custom_badge.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_clue_custom_badge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_clue_custom_image_badge.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_clue_custom_image_badge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_custom_badge.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_custom_badge.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_magtag_simpletest.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_pewpewm4_simpletest.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_pewpewm4_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_pygamer_asyncio.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_pygamer_asyncio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_pyportal_touchscreen.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_pyportal_touchscreen.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/examples/pybadger_simpletest.py` & `adafruit-circuitpython-pybadger-3.7.9/examples/pybadger_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pybadger-3.7.8/pyproject.toml` & `adafruit-circuitpython-pybadger-3.7.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pybadger"
 description = "Badge-focused CircuitPython helper library for PyBadge, PyBadge LC, PyGamer and CLUE"
-version = "3.7.8"
+version = "3.7.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_REPLACE"}
 keywords = [
     "adafruit",
```

