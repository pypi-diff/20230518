# Comparing `tmp/adafruit-circuitpython-mcp230xx-2.5.8.tar.gz` & `tmp/adafruit-circuitpython-mcp230xx-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp230xx-2.5.8.tar", last modified: Fri Aug 26 02:25:35 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp230xx-2.5.9.tar", last modified: Tue Feb  7 23:13:25 2023, max compression
```

## Comparing `adafruit-circuitpython-mcp230xx-2.5.8.tar` & `adafruit-circuitpython-mcp230xx-2.5.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.144623 adafruit-circuitpython-mcp230xx-2.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.144623 adafruit-circuitpython-mcp230xx-2.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16252 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3074 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-08-26 02:25:35.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-08-26 02:25:35.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:25:35.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:25:35.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-26 02:25:35.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/digital_inout.py
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23008.py
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23016.py
--rw-r--r--   0 runner    (1001) docker     (121)    11506 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23017.py
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp230xx.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23s08.py
--rw-r--r--   0 runner    (1001) docker     (121)    11023 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23s17.py
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23sxx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23xxx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_event_detect_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_leds_and_buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_leds_and_buttons_irq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp23Sxx_event_detect_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp23Sxx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-08-26 02:25:27.000000 adafruit-circuitpython-mcp230xx-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:25:20.000000 adafruit-circuitpython-mcp230xx-2.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:25:35.148623 adafruit-circuitpython-mcp230xx-2.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.071470 adafruit-circuitpython-mcp230xx-2.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.063470 adafruit-circuitpython-mcp230xx-2.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.067470 adafruit-circuitpython-mcp230xx-2.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.067470 adafruit-circuitpython-mcp230xx-2.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.067470 adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-02-07 23:13:25.071470 adafruit-circuitpython-mcp230xx-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.067470 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-02-07 23:13:25.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-07 23:13:25.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 23:13:25.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-07 23:13:25.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-07 23:13:25.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.067470 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/digital_inout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23016.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp230xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23s08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23s17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23sxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23xxx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.071470 adafruit-circuitpython-mcp230xx-2.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.071470 adafruit-circuitpython-mcp230xx-2.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:13:25.071470 adafruit-circuitpython-mcp230xx-2.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_event_detect_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_leds_and_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_leds_and_buttons_irq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp23Sxx_event_detect_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp23Sxx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-07 23:13:17.000000 adafruit-circuitpython-mcp230xx-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-07 23:13:06.000000 adafruit-circuitpython-mcp230xx-2.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 23:13:25.071470 adafruit-circuitpython-mcp230xx-2.5.9/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp230xx-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/.gitignore` & `adafruit-circuitpython-mcp230xx-2.5.9/.gitignore`

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

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp230xx-2.5.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

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
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/.pylintrc` & `adafruit-circuitpython-mcp230xx-2.5.9/.pylintrc`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2017 Tony DiCola for Adafruit Industries
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

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp230xx-2.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/LICENSE` & `adafruit-circuitpython-mcp230xx-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp230xx-2.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/PKG-INFO` & `adafruit-circuitpython-mcp230xx-2.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp230xx
-Version: 2.5.8
+Version: 2.5.9
 Summary: CircuitPython library for controlling a MCP23008 or MCP23017 I2C GPIO expander.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx
 Keywords: adafruit,mcp23017,mcp23008,i2c,gpio,expander,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/README.rst` & `adafruit-circuitpython-mcp230xx-2.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp230xx
-Version: 2.5.8
+Version: 2.5.9
 Summary: CircuitPython library for controlling a MCP23008 or MCP23017 I2C GPIO expander.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx
 Keywords: adafruit,mcp23017,mcp23008,i2c,gpio,expander,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_circuitpython_mcp230xx.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_circuitpython_mcp230xx.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
 adafruit_circuitpython_mcp230xx.egg-info/PKG-INFO
 adafruit_circuitpython_mcp230xx.egg-info/SOURCES.txt
 adafruit_circuitpython_mcp230xx.egg-info/dependency_links.txt
 adafruit_circuitpython_mcp230xx.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/digital_inout.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/digital_inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 try:
     from typing import Optional
     from adafruit_mcp230xx.mcp23xxx import MCP23XXX
     from digitalio import Pull, Direction
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 # Internal helpers to simplify setting and getting a bit inside an integer.
 def _get_bit(val, bit: int) -> int:
     return val & (1 << bit) > 0
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23008.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23s08.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 # SPDX-FileCopyrightText: 2017 Tony DiCola for Adafruit Industries
 # SPDX-FileCopyrightText: 2019 Carter Nelson
+# SPDX-FileCopyrightText: 2021 Red_M
 #
 # SPDX-License-Identifier: MIT
 
 """
-`mcp23008`
+`MCP23S08`
 ====================================================
 
-CircuitPython module for the MCP23008 I2C I/O extenders.
+CircuitPython module for the MCP23S08 I2C I/O extenders.
 
-* Author(s): Tony DiCola
+* Author(s): Tony DiCola, Romy Bompart (2020), Red_M (2021)
 """
 
 from micropython import const
-from .mcp230xx import MCP230XX
+from .mcp23sxx import MCP23SXX
 from .digital_inout import DigitalInOut
 
 try:
     import typing  # pylint: disable=unused-import
-    from busio import I2C
+    from busio import SPI
+    import digitalio
 except ImportError:
     pass
 
-__version__ = "2.5.8"
-__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
+__version__ = "2.5.9"
+__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP23Sxx.git"
 
-_MCP23008_ADDRESS = const(0x20)
-_MCP23008_IODIR = const(0x00)
-_MCP23008_IPOL = const(0x01)
-_MCP23008_GPINTEN = const(0x02)
-_MCP23008_DEFVAL = const(0x03)
-_MCP23008_INTCON = const(0x04)
-_MCP23008_IOCON = const(0x05)
-_MCP23008_GPPU = const(0x06)
-_MCP23008_INTF = const(0x07)
-_MCP23008_INTCAP = const(0x08)
-_MCP23008_GPIO = const(0x09)
-
-
-class MCP23008(MCP230XX):
-    """Supports MCP23008 instance on specified I2C bus and optionally
+_MCP23S08_ADDRESS = const(0x20)
+_MCP23S08_IODIR = const(0x00)
+_MCP23S08_IPOL = const(0x01)
+_MCP23S08_GPINTEN = const(0x02)
+_MCP23S08_DEFVAL = const(0x03)
+_MCP23S08_INTCON = const(0x04)
+_MCP23S08_IOCON = const(0x05)
+_MCP23S08_GPPU = const(0x06)
+_MCP23S08_INTF = const(0x07)
+_MCP23S08_INTCAP = const(0x08)
+_MCP23S08_GPIO = const(0x09)
+
+# pylint: disable=too-many-arguments
+class MCP23S08(MCP23SXX):
+    """Supports MCP23S08 instance on specified I2C bus and optionally
     at the specified I2C address.
     """
 
     def __init__(
-        self, i2c: I2C, address: int = _MCP23008_ADDRESS, reset: bool = True
+        self,
+        spi: SPI,
+        chip_select: digitalio.DigitalInOut,
+        address: int = _MCP23S08_ADDRESS,
+        reset: bool = True,
+        baudrate: int = 100000,
     ) -> None:
-        super().__init__(i2c, address)
-
+        super().__init__(spi, address, chip_select, baudrate=baudrate)
+        # For user information
+        self.address = address
         if reset:
             # Reset to all inputs with no pull-ups and no inverted polarity.
             self.iodir = 0xFF
             self.gppu = 0x00
-            self._write_u8(_MCP23008_IPOL, 0x00)
+            self._write_u8(_MCP23S08_IPOL, 0x00)
 
     @property
     def gpio(self) -> int:
         """The raw GPIO output register.  Each bit represents the
         output value of the associated pin (0 = low, 1 = high), assuming that
         pin has been configured as an output previously.
         """
-        return self._read_u8(_MCP23008_GPIO)
+        return self._read_u8(_MCP23S08_GPIO)
 
     @gpio.setter
     def gpio(self, val: int) -> None:
-        self._write_u8(_MCP23008_GPIO, val)
+        self._write_u8(_MCP23S08_GPIO, val)
 
     @property
     def iodir(self) -> int:
         """The raw IODIR direction register.  Each bit represents
         direction of a pin, either 1 for an input or 0 for an output mode.
         """
-        return self._read_u8(_MCP23008_IODIR)
+        return self._read_u8(_MCP23S08_IODIR)
 
     @iodir.setter
     def iodir(self, val: int) -> None:
-        self._write_u8(_MCP23008_IODIR, val)
+        self._write_u8(_MCP23S08_IODIR, val)
 
     @property
     def gppu(self) -> int:
         """The raw GPPU pull-up register.  Each bit represents
         if a pull-up is enabled on the specified pin (1 = pull-up enabled,
         0 = pull-up disabled).  Note pull-down resistors are NOT supported!
         """
-        return self._read_u8(_MCP23008_GPPU)
+        return self._read_u8(_MCP23S08_GPPU)
 
     @gppu.setter
     def gppu(self, val: int) -> None:
-        self._write_u8(_MCP23008_GPPU, val)
+        self._write_u8(_MCP23S08_GPPU, val)
 
     def get_pin(self, pin: int) -> DigitalInOut:
         """Convenience function to create an instance of the DigitalInOut class
-        pointing at the specified pin of this MCP23008 device.
+        pointing at the specified pin of this MCP23S08 device.
         """
         if not 0 <= pin <= 7:
             raise ValueError("Pin number must be 0-7.")
         return DigitalInOut(pin, self)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23016.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23016.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 _MCP23016_ADDRESS = const(0x20)
 _MCP23016_GPIO0 = const(0x00)
 _MCP23016_GPIO1 = const(0x01)
 _MCP23016_IPOL0 = const(0x04)
 _MCP23016_IPOL1 = const(0x05)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23017.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23017.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,39 @@
 """
 `mcp23017`
 ====================================================
 
 CircuitPython module for the MCP23017 I2C I/O extenders.
 
 * Author(s): Tony DiCola
+
+Implementation Notes
+--------------------
+
+**Hardware:**
+
+* `MCP23017 - i2c 16 input/output port expander
+  <https://www.adafruit.com/product/732>`_
+
+* `Adafruit MCP23017 I2C GPIO Expander Breakout - STEMMA QT / Qwiic
+  <https://www.adafruit.com/product/5346>`_
+
 """
 
 from micropython import const
 from .mcp230xx import MCP230XX
 from .digital_inout import DigitalInOut
 
 try:
     from typing import List
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 _MCP23017_ADDRESS = const(0x20)
 _MCP23017_IODIRA = const(0x00)
 _MCP23017_IODIRB = const(0x01)
 _MCP23017_IPOLA = const(0x02)
 _MCP23017_IPOLB = const(0x03)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp230xx.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp230xx.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 CircuitPython module for the MCP23017 and MCP23008 I2C I/O extenders.
 
 * Author(s): Tony DiCola, Red_M (2021)
 """
 
 from .mcp23xxx import MCP23XXX
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 # Global buffer for reading and writing registers with the devices.  This is
 # shared between both the MCP23008 and MCP23017 class to reduce memory allocations.
 # However this is explicitly not thread safe or re-entrant by design!
 _BUFFER = bytearray(3)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23s08.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23008.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,107 @@
 # SPDX-FileCopyrightText: 2017 Tony DiCola for Adafruit Industries
 # SPDX-FileCopyrightText: 2019 Carter Nelson
-# SPDX-FileCopyrightText: 2021 Red_M
 #
 # SPDX-License-Identifier: MIT
 
 """
-`MCP23S08`
+`mcp23008`
 ====================================================
 
-CircuitPython module for the MCP23S08 I2C I/O extenders.
+CircuitPython module for the MCP23008 I2C I/O extenders.
+
+* Author(s): Tony DiCola
+
+Implementation Notes
+--------------------
+
+**Hardware:**
+
+* `MCP23008 - i2c 8 input/output port expander
+  <https://www.adafruit.com/product/593>`_
 
-* Author(s): Tony DiCola, Romy Bompart (2020), Red_M (2021)
 """
 
 from micropython import const
-from .mcp23sxx import MCP23SXX
+from .mcp230xx import MCP230XX
 from .digital_inout import DigitalInOut
 
 try:
     import typing  # pylint: disable=unused-import
-    from busio import SPI
-    import digitalio
+    from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.5.8"
-__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP23Sxx.git"
+__version__ = "2.5.9"
+__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
-_MCP23S08_ADDRESS = const(0x20)
-_MCP23S08_IODIR = const(0x00)
-_MCP23S08_IPOL = const(0x01)
-_MCP23S08_GPINTEN = const(0x02)
-_MCP23S08_DEFVAL = const(0x03)
-_MCP23S08_INTCON = const(0x04)
-_MCP23S08_IOCON = const(0x05)
-_MCP23S08_GPPU = const(0x06)
-_MCP23S08_INTF = const(0x07)
-_MCP23S08_INTCAP = const(0x08)
-_MCP23S08_GPIO = const(0x09)
-
-# pylint: disable=too-many-arguments
-class MCP23S08(MCP23SXX):
-    """Supports MCP23S08 instance on specified I2C bus and optionally
+_MCP23008_ADDRESS = const(0x20)
+_MCP23008_IODIR = const(0x00)
+_MCP23008_IPOL = const(0x01)
+_MCP23008_GPINTEN = const(0x02)
+_MCP23008_DEFVAL = const(0x03)
+_MCP23008_INTCON = const(0x04)
+_MCP23008_IOCON = const(0x05)
+_MCP23008_GPPU = const(0x06)
+_MCP23008_INTF = const(0x07)
+_MCP23008_INTCAP = const(0x08)
+_MCP23008_GPIO = const(0x09)
+
+
+class MCP23008(MCP230XX):
+    """Supports MCP23008 instance on specified I2C bus and optionally
     at the specified I2C address.
     """
 
     def __init__(
-        self,
-        spi: SPI,
-        chip_select: digitalio.DigitalInOut,
-        address: int = _MCP23S08_ADDRESS,
-        reset: bool = True,
-        baudrate: int = 100000,
+        self, i2c: I2C, address: int = _MCP23008_ADDRESS, reset: bool = True
     ) -> None:
-        super().__init__(spi, address, chip_select, baudrate=baudrate)
-        # For user information
-        self.address = address
+        super().__init__(i2c, address)
+
         if reset:
             # Reset to all inputs with no pull-ups and no inverted polarity.
             self.iodir = 0xFF
             self.gppu = 0x00
-            self._write_u8(_MCP23S08_IPOL, 0x00)
+            self._write_u8(_MCP23008_IPOL, 0x00)
 
     @property
     def gpio(self) -> int:
         """The raw GPIO output register.  Each bit represents the
         output value of the associated pin (0 = low, 1 = high), assuming that
         pin has been configured as an output previously.
         """
-        return self._read_u8(_MCP23S08_GPIO)
+        return self._read_u8(_MCP23008_GPIO)
 
     @gpio.setter
     def gpio(self, val: int) -> None:
-        self._write_u8(_MCP23S08_GPIO, val)
+        self._write_u8(_MCP23008_GPIO, val)
 
     @property
     def iodir(self) -> int:
         """The raw IODIR direction register.  Each bit represents
         direction of a pin, either 1 for an input or 0 for an output mode.
         """
-        return self._read_u8(_MCP23S08_IODIR)
+        return self._read_u8(_MCP23008_IODIR)
 
     @iodir.setter
     def iodir(self, val: int) -> None:
-        self._write_u8(_MCP23S08_IODIR, val)
+        self._write_u8(_MCP23008_IODIR, val)
 
     @property
     def gppu(self) -> int:
         """The raw GPPU pull-up register.  Each bit represents
         if a pull-up is enabled on the specified pin (1 = pull-up enabled,
         0 = pull-up disabled).  Note pull-down resistors are NOT supported!
         """
-        return self._read_u8(_MCP23S08_GPPU)
+        return self._read_u8(_MCP23008_GPPU)
 
     @gppu.setter
     def gppu(self, val: int) -> None:
-        self._write_u8(_MCP23S08_GPPU, val)
+        self._write_u8(_MCP23008_GPPU, val)
 
     def get_pin(self, pin: int) -> DigitalInOut:
         """Convenience function to create an instance of the DigitalInOut class
-        pointing at the specified pin of this MCP23S08 device.
+        pointing at the specified pin of this MCP23008 device.
         """
         if not 0 <= pin <= 7:
             raise ValueError("Pin number must be 0-7.")
         return DigitalInOut(pin, self)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23s17.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23s17.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 try:
     from typing import List
     from busio import SPI
     import digitalio
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 _MCP23S17_ADDRESS = const(0x20)
 _MCP23S17_IODIRA = const(0x00)
 _MCP23S17_IODIRB = const(0x01)
 _MCP23S17_IPOLA = const(0x02)
 _MCP23S17_IPOLB = const(0x03)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23sxx.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23sxx.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     import typing  # pylint: disable=unused-import
     from busio import SPI
     import digitalio
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 # shared between both the MCP23S17 class to reduce memory allocations.
 # However this is explicitly not thread safe or re-entrant by design!
 # Header to start a reading or writting operation
 _OUT_BUFFER = bytearray(4)
 _IN_BUFFER = bytearray(4)
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/adafruit_mcp230xx/mcp23xxx.py` & `adafruit-circuitpython-mcp230xx-2.5.9/adafruit_mcp230xx/mcp23xxx.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 try:
     from typing import Union, Optional
     from busio import I2C, SPI
     import digitalio
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx.git"
 
 # pylint: disable=too-few-public-methods
 class MCP23XXX:
     """Base class for MCP23xxx devices."""
 
     def __init__(
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp230xx-2.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/docs/api.rst` & `adafruit-circuitpython-mcp230xx-2.5.9/docs/api.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 
 .. If you created a package, create one automodule per module in the package.
 
 .. If your library file(s) are nested in a directory (e.g. /adafruit_foo/foo.py)
 .. use this format as the module name: "adafruit_foo.foo"
 
+.. automodule:: adafruit_mcp230xx.mcp23xxx
+   :members:
+
 .. automodule:: adafruit_mcp230xx.mcp230xx
    :members:
 
 .. automodule:: adafruit_mcp230xx.mcp23008
    :members:
 
+.. automodule:: adafruit_mcp230xx.mcp23016
+   :members:
+
 .. automodule:: adafruit_mcp230xx.mcp23017
    :members:
 
 .. automodule:: adafruit_mcp230xx.mcp23sxx
    :members:
 
 .. automodule:: adafruit_mcp230xx.mcp23s08
```

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/docs/conf.py` & `adafruit-circuitpython-mcp230xx-2.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/docs/index.rst` & `adafruit-circuitpython-mcp230xx-2.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_event_detect_interrupt.py` & `adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_event_detect_interrupt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_leds_and_buttons.py` & `adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_leds_and_buttons.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_leds_and_buttons_irq.py` & `adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_leds_and_buttons_irq.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp230xx_simpletest.py` & `adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp230xx_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp23Sxx_event_detect_interrupt.py` & `adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp23Sxx_event_detect_interrupt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/examples/mcp23Sxx_simpletest.py` & `adafruit-circuitpython-mcp230xx-2.5.9/examples/mcp23Sxx_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp230xx-2.5.8/pyproject.toml` & `adafruit-circuitpython-mcp230xx-2.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp230xx"
 description = "CircuitPython library for controlling a MCP23008 or MCP23017 I2C GPIO expander."
-version = "2.5.8"
+version = "2.5.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP230xx"}
 keywords = [
     "adafruit",
```

