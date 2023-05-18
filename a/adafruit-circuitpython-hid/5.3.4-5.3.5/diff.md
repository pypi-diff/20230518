# Comparing `tmp/adafruit-circuitpython-hid-5.3.4.tar.gz` & `tmp/adafruit-circuitpython-hid-5.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-hid-5.3.4.tar", last modified: Mon Mar 20 21:32:43 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-hid-5.3.5.tar", last modified: Thu May 18 15:37:26 2023, max compression
```

## Comparing `adafruit-circuitpython-hid-5.3.4.tar` & `adafruit-circuitpython-hid-5.3.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.564402 adafruit-circuitpython-hid-5.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.568402 adafruit-circuitpython-hid-5.3.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.568402 adafruit-circuitpython-hid-5.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.568402 adafruit-circuitpython-hid-5.3.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.568402 adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-03-20 21:32:43.000000 adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-20 21:32:43.000000 adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 21:32:43.000000 adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-20 21:32:43.000000 adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-20 21:32:43.000000 adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/adafruit_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/consumer_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/consumer_control_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/keyboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7044 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/keyboard_layout_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5197 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/keyboard_layout_us.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/keycode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/adafruit_hid/mouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/examples/hid_consumer_control_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/examples/hid_gamepad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/examples/hid_joywing_gamepad.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/examples/hid_keyboard_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/examples/hid_simple_gamepad.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/examples/hid_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-20 21:32:34.000000 adafruit-circuitpython-hid-5.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-20 21:32:23.000000 adafruit-circuitpython-hid-5.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 21:32:43.572402 adafruit-circuitpython-hid-5.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.196438 adafruit-circuitpython-hid-5.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.180438 adafruit-circuitpython-hid-5.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.184438 adafruit-circuitpython-hid-5.3.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.188438 adafruit-circuitpython-hid-5.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.192438 adafruit-circuitpython-hid-5.3.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-18 15:37:26.196438 adafruit-circuitpython-hid-5.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.192438 adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-18 15:37:26.000000 adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-18 15:37:26.000000 adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:37:26.000000 adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:37:26.000000 adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 15:37:26.000000 adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.192438 adafruit-circuitpython-hid-5.3.5/adafruit_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/consumer_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/consumer_control_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/keyboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7044 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/keyboard_layout_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5197 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/keyboard_layout_us.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/keycode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/adafruit_hid/mouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.192438 adafruit-circuitpython-hid-5.3.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.192438 adafruit-circuitpython-hid-5.3.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:26.196438 adafruit-circuitpython-hid-5.3.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/examples/hid_consumer_control_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/examples/hid_gamepad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/examples/hid_joywing_gamepad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/examples/hid_keyboard_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/examples/hid_simple_gamepad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/examples/hid_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 15:37:16.000000 adafruit-circuitpython-hid-5.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:37:01.000000 adafruit-circuitpython-hid-5.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:37:26.196438 adafruit-circuitpython-hid-5.3.5/setup.cfg
```

### Comparing `adafruit-circuitpython-hid-5.3.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-hid-5.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/.gitignore` & `adafruit-circuitpython-hid-5.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/.pre-commit-config.yaml` & `adafruit-circuitpython-hid-5.3.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-hid-5.3.4/.pylintrc` & `adafruit-circuitpython-hid-5.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-hid-5.3.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/LICENSE` & `adafruit-circuitpython-hid-5.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-hid-5.3.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/LICENSES/MIT.txt` & `adafruit-circuitpython-hid-5.3.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-hid-5.3.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/PKG-INFO` & `adafruit-circuitpython-hid-5.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hid
-Version: 5.3.4
+Version: 5.3.5
 Summary: CircuitPython helper library for simulating HID devices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HID
 Keywords: adafruit,hid,human,interface,device,keyboard,mouse,keycode,keypadhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hid-5.3.4/README.rst` & `adafruit-circuitpython-hid-5.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/PKG-INFO` & `adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hid
-Version: 5.3.4
+Version: 5.3.5
 Summary: CircuitPython helper library for simulating HID devices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HID
 Keywords: adafruit,hid,human,interface,device,keyboard,mouse,keycode,keypadhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_circuitpython_hid.egg-info/SOURCES.txt` & `adafruit-circuitpython-hid-5.3.5/adafruit_circuitpython_hid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/__init__.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 try:
     from typing import Sequence
     import usb_hid
 except ImportError:
     pass
 
-__version__ = "5.3.4"
+__version__ = "5.3.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HID.git"
 
 
 def find_device(
     devices: Sequence[usb_hid.Device], *, usage_page: int, usage: int
 ) -> usb_hid.Device:
     """Search through the provided sequence of devices to find the one with the matching
```

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/consumer_control.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/consumer_control.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/consumer_control_code.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/consumer_control_code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/keyboard.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/keyboard.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/keyboard_layout_base.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/keyboard_layout_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 try:
     from typing import Tuple
     from .keyboard import Keyboard
 except ImportError:
     pass
 
 
-__version__ = "5.3.4"
+__version__ = "5.3.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HID.git"
 
 
 class KeyboardLayoutBase:
     """Base class for keyboard layouts. Uses the tables defined in the subclass
     to map UTF-8 characters to appropriate keypresses.
```

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/keyboard_layout_us.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/keyboard_layout_us.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/keycode.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/keycode.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/adafruit_hid/mouse.py` & `adafruit-circuitpython-hid-5.3.5/adafruit_hid/mouse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/docs/_static/favicon.ico` & `adafruit-circuitpython-hid-5.3.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/docs/conf.py` & `adafruit-circuitpython-hid-5.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/docs/examples.rst` & `adafruit-circuitpython-hid-5.3.5/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/docs/index.rst` & `adafruit-circuitpython-hid-5.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/examples/hid_consumer_control_brightness.py` & `adafruit-circuitpython-hid-5.3.5/examples/hid_consumer_control_brightness.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/examples/hid_gamepad.py` & `adafruit-circuitpython-hid-5.3.5/examples/hid_gamepad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/examples/hid_joywing_gamepad.py` & `adafruit-circuitpython-hid-5.3.5/examples/hid_joywing_gamepad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/examples/hid_keyboard_shortcuts.py` & `adafruit-circuitpython-hid-5.3.5/examples/hid_keyboard_shortcuts.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/examples/hid_simple_gamepad.py` & `adafruit-circuitpython-hid-5.3.5/examples/hid_simple_gamepad.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     button.direction = digitalio.Direction.INPUT
     button.pull = digitalio.Pull.UP
 
 # Connect an analog two-axis joystick to A4 and A5.
 ax = analogio.AnalogIn(board.A4)
 ay = analogio.AnalogIn(board.A5)
 
+
 # Equivalent of Arduino's map() function.
 def range_map(x, in_min, in_max, out_min, out_max):
     return (x - in_min) * (out_max - out_min) // (in_max - in_min) + out_min
 
 
 while True:
     # Buttons are grounded when pressed (.value = False).
```

### Comparing `adafruit-circuitpython-hid-5.3.4/examples/hid_simpletest.py` & `adafruit-circuitpython-hid-5.3.5/examples/hid_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hid-5.3.4/pyproject.toml` & `adafruit-circuitpython-hid-5.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-hid"
 description = "CircuitPython helper library for simulating HID devices."
-version = "5.3.4"
+version = "5.3.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HID"}
 keywords = [
     "adafruit",
```

