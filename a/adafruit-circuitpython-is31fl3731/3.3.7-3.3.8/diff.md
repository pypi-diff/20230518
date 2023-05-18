# Comparing `tmp/adafruit-circuitpython-is31fl3731-3.3.7.tar.gz` & `tmp/adafruit-circuitpython-is31fl3731-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-is31fl3731-3.3.7.tar", last modified: Mon Feb 27 20:05:34 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-is31fl3731-3.3.8.tar", last modified: Thu May 18 15:37:58 2023, max compression
```

## Comparing `adafruit-circuitpython-is31fl3731-3.3.7.tar` & `adafruit-circuitpython-is31fl3731-3.3.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.083061 adafruit-circuitpython-is31fl3731-3.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.083061 adafruit-circuitpython-is31fl3731-3.3.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.083061 adafruit-circuitpython-is31fl3731-3.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.083061 adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.083061 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-02-27 20:05:34.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-02-27 20:05:34.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:05:34.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-27 20:05:34.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-27 20:05:34.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/charlie_bonnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/charlie_wing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/keybow2040.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/led_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/matrix_11x7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/rgbmatrix5x5.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/scroll_phat_hd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_blink_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_frame_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_keybow_2040_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_ledshim_fade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_ledshim_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_pillow_animated_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_pillow_marquee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_pillow_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_rgbmatrix5x5_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_text_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_wave_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-27 20:05:26.000000 adafruit-circuitpython-is31fl3731-3.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-27 20:05:15.000000 adafruit-circuitpython-is31fl3731-3.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:05:34.087061 adafruit-circuitpython-is31fl3731-3.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.857215 adafruit-circuitpython-is31fl3731-3.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.845215 adafruit-circuitpython-is31fl3731-3.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.849215 adafruit-circuitpython-is31fl3731-3.3.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.849215 adafruit-circuitpython-is31fl3731-3.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.849215 adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-18 15:37:58.853215 adafruit-circuitpython-is31fl3731-3.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.849215 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-18 15:37:58.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-18 15:37:58.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:37:58.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:37:58.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 15:37:58.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.853215 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/charlie_bonnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/charlie_wing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/keybow2040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/led_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/matrix_11x7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/rgbmatrix5x5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/scroll_phat_hd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.853215 adafruit-circuitpython-is31fl3731-3.3.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.853215 adafruit-circuitpython-is31fl3731-3.3.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:58.853215 adafruit-circuitpython-is31fl3731-3.3.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_blink_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_frame_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_keybow_2040_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_ledshim_fade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_ledshim_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_pillow_animated_gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_pillow_marquee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_pillow_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_rgbmatrix5x5_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_text_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_wave_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-18 15:37:50.000000 adafruit-circuitpython-is31fl3731-3.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-18 15:37:39.000000 adafruit-circuitpython-is31fl3731-3.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:37:58.857215 adafruit-circuitpython-is31fl3731-3.3.8/setup.cfg
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-is31fl3731-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/.gitignore` & `adafruit-circuitpython-is31fl3731-3.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/.pre-commit-config.yaml` & `adafruit-circuitpython-is31fl3731-3.3.8/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/.pylintrc` & `adafruit-circuitpython-is31fl3731-3.3.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-is31fl3731-3.3.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/LICENSE` & `adafruit-circuitpython-is31fl3731-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/MIT.txt` & `adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-is31fl3731-3.3.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/PKG-INFO` & `adafruit-circuitpython-is31fl3731-3.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-is31fl3731
-Version: 3.3.7
+Version: 3.3.8
 Summary: CircuitPython library for IS31FL3731 charlieplex LED matrices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731
 Keywords: adafruit,is31fl3731,led,matrix,charlieplex,featherwingbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/README.rst` & `adafruit-circuitpython-is31fl3731-3.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-is31fl3731
-Version: 3.3.7
+Version: 3.3.8
 Summary: CircuitPython library for IS31FL3731 charlieplex LED matrices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731
 Keywords: adafruit,is31fl3731,led,matrix,charlieplex,featherwingbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/__init__.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # imports
 import math
 import time
 from micropython import const
 
 from adafruit_bus_device.i2c_device import I2CDevice
 
-__version__ = "3.3.7"
+__version__ = "3.3.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731.git"
 
 _MODE_REGISTER = const(0x00)
 _FRAME_REGISTER = const(0x01)
 _AUTOPLAY1_REGISTER = const(0x02)
 _AUTOPLAY2_REGISTER = const(0x03)
 _BLINK_REGISTER = const(0x05)
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/charlie_bonnet.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/charlie_bonnet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/charlie_wing.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/charlie_wing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/keybow2040.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/keybow2040.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
         # pylint: disable=inconsistent-return-statements
         # pylint: disable=too-many-return-statements
         # pylint: disable=too-many-branches
 
     @staticmethod
     def pixel_addr(x, y):
-
         lookup = [
             (120, 88, 104),  # 0, 0
             (136, 40, 72),  # 1, 0
             (112, 80, 96),  # 2, 0
             (128, 32, 64),  # 3, 0
             (121, 89, 105),  # 0, 1
             (137, 41, 73),  # 1, 1
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/led_shim.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/led_shim.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/matrix.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/matrix.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/matrix_11x7.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/matrix_11x7.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/rgbmatrix5x5.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/rgbmatrix5x5.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/adafruit_is31fl3731/scroll_phat_hd.py` & `adafruit-circuitpython-is31fl3731-3.3.8/adafruit_is31fl3731/scroll_phat_hd.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/docs/_static/favicon.ico` & `adafruit-circuitpython-is31fl3731-3.3.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/docs/api.rst` & `adafruit-circuitpython-is31fl3731-3.3.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/docs/conf.py` & `adafruit-circuitpython-is31fl3731-3.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/docs/examples.rst` & `adafruit-circuitpython-is31fl3731-3.3.8/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/docs/index.rst` & `adafruit-circuitpython-is31fl3731-3.3.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_blink_example.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_blink_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_frame_example.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_frame_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_keybow_2040_rainbow.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_keybow_2040_rainbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_ledshim_rainbow.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_ledshim_rainbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_pillow_animated_gif.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_pillow_animated_gif.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_pillow_marquee.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_pillow_marquee.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_pillow_numbers.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_pillow_numbers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_rgbmatrix5x5_rainbow.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_rgbmatrix5x5_rainbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_simpletest.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_text_example.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_text_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/examples/is31fl3731_wave_example.py` & `adafruit-circuitpython-is31fl3731-3.3.8/examples/is31fl3731_wave_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.7/pyproject.toml` & `adafruit-circuitpython-is31fl3731-3.3.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-is31fl3731"
 description = "CircuitPython library for IS31FL3731 charlieplex LED matrices."
-version = "3.3.7"
+version = "3.3.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731"}
 keywords = [
     "adafruit",
```

