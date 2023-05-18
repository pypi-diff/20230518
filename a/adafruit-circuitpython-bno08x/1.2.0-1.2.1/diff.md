# Comparing `tmp/adafruit-circuitpython-bno08x-1.2.0.tar.gz` & `tmp/adafruit-circuitpython-bno08x-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.0.tar", last modified: Thu Apr 20 19:39:42 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.1.tar", last modified: Thu May 18 15:32:01 2023, max compression
```

## Comparing `adafruit-circuitpython-bno08x-1.2.0.tar` & `adafruit-circuitpython-bno08x-1.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.732784 adafruit-circuitpython-bno08x-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.724784 adafruit-circuitpython-bno08x-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-20 19:39:42.732784 adafruit-circuitpython-bno08x-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/
--rw-r--r--   0 runner    (1001) docker     (123)    38913 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 19:39:42.000000 adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:39:42.728784 adafruit-circuitpython-bno08x-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_find_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_more_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_quaternion_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-20 19:39:35.000000 adafruit-circuitpython-bno08x-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-20 19:39:25.000000 adafruit-circuitpython-bno08x-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:39:42.732784 adafruit-circuitpython-bno08x-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/
+-rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_find_heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_more_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_quaternion_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/setup.cfg
```

### Comparing `adafruit-circuitpython-bno08x-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bno08x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/.gitignore` & `adafruit-circuitpython-bno08x-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/.pre-commit-config.yaml` & `adafruit-circuitpython-bno08x-1.2.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-bno08x-1.2.0/.pylintrc` & `adafruit-circuitpython-bno08x-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bno08x-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/LICENSE` & `adafruit-circuitpython-bno08x-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bno08x-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/LICENSES/MIT.txt` & `adafruit-circuitpython-bno08x-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bno08x-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.0
+Version: 1.2.1
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.0/README.rst` & `adafruit-circuitpython-bno08x-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/__init__.py` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https:# github.com/adafruit/circuitpython/releases
 
 * `Adafruit's Bus Device library <https:# github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
 """
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __repo__ = "https:# github.com/adafruit/Adafruit_CircuitPython_BNO08x.git"
 
 from struct import unpack_from, pack_into
 from collections import namedtuple
 import time
 from micropython import const
 
@@ -308,15 +308,14 @@
     sw_part_number = unpack_from("<I", buffer, offset=4)[0]
     sw_build_number = unpack_from("<I", buffer, offset=8)[0]
 
     return (sw_part_number, sw_major, sw_minor, sw_patch, sw_build_number)
 
 
 def _parse_command_response(report_bytes):
-
     # CMD response report:
     # 0 Report ID = 0xF1
     # 1 Sequence number
     # 2 Command
     # 3 Command sequence number
     # 4 Response sequence number
     # 5 R0-10 A set of response values. The interpretation of these values is specific
@@ -379,15 +378,14 @@
 
     def __init__(self, packet_bytes):
         self.header = self.header_from_buffer(packet_bytes)
         data_end_index = self.header.data_length + _BNO_HEADER_LEN
         self.data = packet_bytes[_BNO_HEADER_LEN:data_end_index]
 
     def __str__(self):
-
         length = self.header.packet_byte_count
         outstr = "\n\t\t********** Packet *************\n"
         outstr += "DBG::\t\t HEADER:\n"
 
         outstr += "DBG::\t\t Data Len: %d\n" % (self.header.data_length)
         outstr += "DBG::\t\t Channel: %s (%d)\n" % (
             channels[self.channel_number],
@@ -742,15 +740,14 @@
                 0,  # reserved
                 0,  # reserved
             ]
         )
         return self._magnetometer_accuracy
 
     def _send_me_command(self, subcommand_params):
-
         start_time = time.monotonic()
         local_buffer = self._command_buffer
         _insert_command_request_report(
             _ME_CALIBRATE,
             self._command_buffer,  # should use self._data_buffer :\ but send_packet don't
             self._get_report_seq_id(_COMMAND_REQUEST),
             subcommand_params,
```

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/debug.py` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/i2c.py` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/spi.py` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_bno08x/uart.py` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.0
+Version: 1.2.1
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.0/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt` & `adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/docs/_static/favicon.ico` & `adafruit-circuitpython-bno08x-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/docs/conf.py` & `adafruit-circuitpython-bno08x-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/docs/index.rst` & `adafruit-circuitpython-bno08x-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_calibration.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_find_heading.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_find_heading.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_more_reports.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_more_reports.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_quaternion_service.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_quaternion_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 bno.enable_feature(BNO_REPORT_ACCELEROMETER)
 bno.enable_feature(BNO_REPORT_GYROSCOPE)
 bno.enable_feature(BNO_REPORT_MAGNETOMETER)
 bno.enable_feature(BNO_REPORT_ROTATION_VECTOR)
 
 while True:
-
     time.sleep(0.5)
     print("Acceleration:")
     accel_x, accel_y, accel_z = bno.acceleration  # pylint:disable=no-member
     print("X: %0.6f  Y: %0.6f Z: %0.6f  m/s^2" % (accel_x, accel_y, accel_z))
     print("")
 
     print("Gyro:")
```

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_spi.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/examples/bno08x_simpletest_uart.py` & `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.0/pyproject.toml` & `adafruit-circuitpython-bno08x-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bno08x"
 description = "Helper library for the Hillcrest Laboratories BNO08x IMUs"
-version = "1.2.0"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BNO08x"}
 keywords = [
     "adafruit",
```

