# Comparing `tmp/adafruit-circuitpython-lsm6ds-4.5.8.tar.gz` & `tmp/adafruit-circuitpython-lsm6ds-4.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lsm6ds-4.5.8.tar", last modified: Tue Apr 25 22:50:29 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-lsm6ds-4.5.9.tar", last modified: Thu May 18 15:38:22 2023, max compression
```

## Comparing `adafruit-circuitpython-lsm6ds-4.5.8.tar` & `adafruit-circuitpython-lsm6ds-4.5.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.094131 adafruit-circuitpython-lsm6ds-4.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.094131 adafruit-circuitpython-lsm6ds-4.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 22:50:29.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/ism330dhcx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds33.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3trc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dso32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dsox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.098131 adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_full_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_ism330dhcx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3trc_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dso32_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_mlc_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_pedometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-25 22:50:21.000000 adafruit-circuitpython-lsm6ds-4.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 22:50:12.000000 adafruit-circuitpython-lsm6ds-4.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:50:29.102131 adafruit-circuitpython-lsm6ds-4.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.924544 adafruit-circuitpython-lsm6ds-4.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.924544 adafruit-circuitpython-lsm6ds-4.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.924544 adafruit-circuitpython-lsm6ds-4.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.924544 adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-18 15:38:22.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-18 15:38:22.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:38:22.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:38:22.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:38:22.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/ism330dhcx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6ds3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6ds33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6ds3trc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6dso32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6dsox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_full_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_ism330dhcx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6ds33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6ds3_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6ds3trc_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6dso32_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6dsox_mlc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6dsox_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_pedometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-18 15:38:15.000000 adafruit-circuitpython-lsm6ds-4.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:38:04.000000 adafruit-circuitpython-lsm6ds-4.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:38:22.928544 adafruit-circuitpython-lsm6ds-4.5.9/setup.cfg
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lsm6ds-4.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/.gitignore` & `adafruit-circuitpython-lsm6ds-4.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-lsm6ds-4.5.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/.pylintrc` & `adafruit-circuitpython-lsm6ds-4.5.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lsm6ds-4.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/LICENSE` & `adafruit-circuitpython-lsm6ds-4.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lsm6ds-4.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/PKG-INFO` & `adafruit-circuitpython-lsm6ds-4.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm6ds
-Version: 4.5.8
+Version: 4.5.9
 Summary: CircuitPython helper library for the LSM6DS family of motion sensors from ST
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS
 Keywords: adafruit,blinka,circuitpython,micropython,lsm6ds,lsm6dsox,lsmds33,lsm6dso32,st,imu,gyro,accelerometer,ism330dhcx,imu,gyro,gyroscope,inemo
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/README.rst` & `adafruit-circuitpython-lsm6ds-4.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm6ds
-Version: 4.5.8
+Version: 4.5.9
 Summary: CircuitPython helper library for the LSM6DS family of motion sensors from ST
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS
 Keywords: adafruit,blinka,circuitpython,micropython,lsm6ds,lsm6dsox,lsmds33,lsm6dso32,st,imu,gyro,accelerometer,ism330dhcx,imu,gyro,gyroscope,inemo
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_circuitpython_lsm6ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/__init__.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 * Adafruit's Bus Device library:
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
-__version__ = "4.5.8"
+__version__ = "4.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS.git"
 
 import struct
 from time import sleep
 from math import radians
 from micropython import const
 from adafruit_bus_device import i2c_device
@@ -315,15 +315,16 @@
         self._accel_range = value
         self._cached_accel_range = value
         sleep(0.2)  # needed to let new range settle
 
     @property
     def gyro_range(self) -> int:
         """Adjusts the range of values that the sensor can measure, from 125 Degrees/s to 2000
-        degrees/s. Note that larger ranges will be less accurate. Must be a ``GyroRange``."""
+        degrees/s. Note that larger ranges will be less accurate. Must be a ``GyroRange``.
+        """
         return self._cached_gyro_range
 
     @gyro_range.setter
     def gyro_range(self, value: int) -> None:
         self._set_gyro_range(value)
         sleep(0.2)
 
@@ -344,15 +345,14 @@
     @property
     def accelerometer_data_rate(self) -> int:
         """Select the rate at which the accelerometer takes measurements. Must be a ``Rate``"""
         return self._accel_data_rate
 
     @accelerometer_data_rate.setter
     def accelerometer_data_rate(self, value: int) -> None:
-
         if not Rate.is_valid(value):
             raise AttributeError("accelerometer_data_rate must be a `Rate`")
 
         self._accel_data_rate = value
         # sleep(.2) # needed to let new range settle
 
     @property
```

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/ism330dhcx.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/ism330dhcx.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6ds3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds33.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6ds33.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6ds3trc.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6ds3trc.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dso32.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6dso32.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/adafruit_lsm6ds/lsm6dsox.py` & `adafruit-circuitpython-lsm6ds-4.5.9/adafruit_lsm6ds/lsm6dsox.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-lsm6ds-4.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/docs/api.rst` & `adafruit-circuitpython-lsm6ds-4.5.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/docs/conf.py` & `adafruit-circuitpython-lsm6ds-4.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/docs/examples.rst` & `adafruit-circuitpython-lsm6ds-4.5.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/docs/index.rst` & `adafruit-circuitpython-lsm6ds-4.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_full_test.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_full_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_ism330dhcx_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_ism330dhcx_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds33_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6ds33_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6ds3_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6ds3trc_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6ds3trc_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dso32_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6dso32_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_mlc_test.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6dsox_mlc_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_lsm6dsox_simpletest.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_lsm6dsox_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_pedometer.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_pedometer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/examples/lsm6ds_rate_test.py` & `adafruit-circuitpython-lsm6ds-4.5.9/examples/lsm6ds_rate_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm6ds-4.5.8/pyproject.toml` & `adafruit-circuitpython-lsm6ds-4.5.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lsm6ds"
 description = "CircuitPython helper library for the LSM6DS family of motion sensors from ST"
-version = "4.5.8"
+version = "4.5.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LSM6DS"}
 keywords = [
     "adafruit",
```

