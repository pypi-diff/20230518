# Comparing `tmp/adafruit-circuitpython-ht16k33-4.6.3.tar.gz` & `tmp/adafruit-circuitpython-ht16k33-4.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ht16k33-4.6.3.tar", last modified: Tue Feb 21 16:57:19 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ht16k33-4.6.4.tar", last modified: Thu May 18 15:37:47 2023, max compression
```

## Comparing `adafruit-circuitpython-ht16k33-4.6.3.tar` & `adafruit-circuitpython-ht16k33-4.6.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.705078 adafruit-circuitpython-ht16k33-4.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.697078 adafruit-circuitpython-ht16k33-4.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-02-21 16:57:19.705078 adafruit-circuitpython-ht16k33-4.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-02-21 16:57:19.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-21 16:57:19.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 16:57:19.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-21 16:57:19.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-21 16:57:19.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/bargraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/ht16k33.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21576 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.701078 adafruit-circuitpython-ht16k33-4.6.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:57:19.705078 adafruit-circuitpython-ht16k33-4.6.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_animation_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_bicolor24_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_multi_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_pillow_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_text_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_14x4_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_7x4customchars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_multi_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-21 16:57:12.000000 adafruit-circuitpython-ht16k33-4.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-21 16:57:02.000000 adafruit-circuitpython-ht16k33-4.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 16:57:19.705078 adafruit-circuitpython-ht16k33-4.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.109946 adafruit-circuitpython-ht16k33-4.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.101943 adafruit-circuitpython-ht16k33-4.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.101943 adafruit-circuitpython-ht16k33-4.6.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.101943 adafruit-circuitpython-ht16k33-4.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.105944 adafruit-circuitpython-ht16k33-4.6.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-18 15:37:47.109946 adafruit-circuitpython-ht16k33-4.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.105944 adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-18 15:37:47.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-18 15:37:47.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:37:47.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 15:37:47.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:37:47.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.105944 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/bargraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/ht16k33.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21576 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.105944 adafruit-circuitpython-ht16k33-4.6.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.105944 adafruit-circuitpython-ht16k33-4.6.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:37:47.109946 adafruit-circuitpython-ht16k33-4.6.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_animation_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_bicolor24_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_multi_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_pillow_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_text_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_14x4_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_7x4customchars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_multi_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-18 15:37:38.000000 adafruit-circuitpython-ht16k33-4.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-18 15:37:27.000000 adafruit-circuitpython-ht16k33-4.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:37:47.109946 adafruit-circuitpython-ht16k33-4.6.4/setup.cfg
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ht16k33-4.6.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/.gitignore` & `adafruit-circuitpython-ht16k33-4.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/.pre-commit-config.yaml` & `adafruit-circuitpython-ht16k33-4.6.4/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/.pylintrc` & `adafruit-circuitpython-ht16k33-4.6.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ht16k33-4.6.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/LICENSE` & `adafruit-circuitpython-ht16k33-4.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ht16k33-4.6.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/LICENSES/MIT.txt` & `adafruit-circuitpython-ht16k33-4.6.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ht16k33-4.6.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/PKG-INFO` & `adafruit-circuitpython-ht16k33-4.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ht16k33
-Version: 4.6.3
+Version: 4.6.4
 Summary: CircuitPython library for HT16K33 LED matrices and segment displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HT16K33
 Keywords: adafruit,ht16k33,led,matrix,segment,displays,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/README.rst` & `adafruit-circuitpython-ht16k33-4.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/PKG-INFO` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ht16k33
-Version: 4.6.3
+Version: 4.6.4
 Summary: CircuitPython library for HT16K33 LED matrices and segment displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HT16K33
 Keywords: adafruit,ht16k33,led,matrix,segment,displays,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_circuitpython_ht16k33.egg-info/SOURCES.txt` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_circuitpython_ht16k33.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/animations.py` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/animations.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
     :param display: HTK33 Display object
 
 
     """
 
     def __init__(self, display: Seg14x4) -> None:
-
         self._display = display
 
     def animate(
         self,
         digits: List[int],
         bitmasks: List[int],
         delay: float = 0.2,
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/bargraph.py` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/bargraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * Authors: Carter Nelson for Adafruit Industries
 
 """
 
 from adafruit_ht16k33.ht16k33 import HT16K33
 
 
-__version__ = "4.6.3"
+__version__ = "4.6.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git"
 
 
 class Bicolor24(HT16K33):
     """Bi-color 24-bar bargraph display."""
 
     LED_OFF = 0
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/ht16k33.py` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/ht16k33.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 try:
     from typing import Union, List, Tuple, Optional
     from busio import I2C
 except ImportError:
     pass
 
 
-__version__ = "4.6.3"
+__version__ = "4.6.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git"
 
 _HT16K33_BLINK_CMD = const(0x80)
 _HT16K33_BLINK_DISPLAYON = const(0x01)
 _HT16K33_CMD_BRIGHTNESS = const(0xE0)
 _HT16K33_OSCILATOR_ON = const(0x21)
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/matrix.py` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from typing import Optional, Tuple, Union, List
     from circuitpython_typing.pil import Image
     from busio import I2C
 except ImportError:
     pass
 
 
-__version__ = "4.6.3"
+__version__ = "4.6.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git"
 
 
 class Matrix8x8(HT16K33):
     """A single matrix."""
 
     _columns = 8
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/adafruit_ht16k33/segments.py` & `adafruit-circuitpython-ht16k33-4.6.4/adafruit_ht16k33/segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 try:
     from typing import Union, List, Tuple, Optional, Dict
     from busio import I2C
 except ImportError:
     pass
 
 
-__version__ = "4.6.3"
+__version__ = "4.6.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git"
 
 # fmt: off
 CHARS = (
     0b00000000, 0b00000000, #
     0b01000000, 0b00000110, # !
     0b00000010, 0b00100000, # "
```

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/docs/_static/favicon.ico` & `adafruit-circuitpython-ht16k33-4.6.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/docs/conf.py` & `adafruit-circuitpython-ht16k33-4.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/docs/examples.rst` & `adafruit-circuitpython-ht16k33-4.6.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/docs/index.rst` & `adafruit-circuitpython-ht16k33-4.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_animation_demo.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_animation_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_bicolor24_simpletest.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_bicolor24_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_multi_display.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_multi_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_pillow_image.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_pillow_image.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_simpletest.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_matrix_text_example.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_matrix_text_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_14x4_demo.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_14x4_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_7x4customchars.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_7x4customchars.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_multi_display.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_multi_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/examples/ht16k33_segments_simpletest.py` & `adafruit-circuitpython-ht16k33-4.6.4/examples/ht16k33_segments_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ht16k33-4.6.3/pyproject.toml` & `adafruit-circuitpython-ht16k33-4.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ht16k33"
 description = "CircuitPython library for HT16K33 LED matrices and segment displays."
-version = "4.6.3"
+version = "4.6.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HT16K33"}
 keywords = [
     "adafruit",
```

