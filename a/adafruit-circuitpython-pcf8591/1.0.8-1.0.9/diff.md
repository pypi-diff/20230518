# Comparing `tmp/adafruit-circuitpython-pcf8591-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-pcf8591-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pcf8591-1.0.8.tar", last modified: Tue Jun  7 17:11:57 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pcf8591-1.0.9.tar", last modified: Thu Jun  9 18:30:16 2022, max compression
```

## Comparing `adafruit-circuitpython-pcf8591-1.0.8.tar` & `adafruit-circuitpython-pcf8591-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.137464 adafruit-circuitpython-pcf8591-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.133464 adafruit-circuitpython-pcf8591-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.133464 adafruit-circuitpython-pcf8591-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.133464 adafruit-circuitpython-pcf8591-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.133464 adafruit-circuitpython-pcf8591-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-07 17:11:57.137464 adafruit-circuitpython-pcf8591-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.133464 adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-07 17:11:57.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-06-07 17:11:57.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:11:57.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-07 17:11:57.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-07 17:11:57.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.133464 adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/analog_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/analog_out.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/pcf8591.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.137464 adafruit-circuitpython-pcf8591-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.137464 adafruit-circuitpython-pcf8591-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:11:57.137464 adafruit-circuitpython-pcf8591-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_adc_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_analog_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_dac_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:11:57.137464 adafruit-circuitpython-pcf8591-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-06-07 17:11:41.000000 adafruit-circuitpython-pcf8591-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.749323 adafruit-circuitpython-pcf8591-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.741323 adafruit-circuitpython-pcf8591-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.745323 adafruit-circuitpython-pcf8591-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.745323 adafruit-circuitpython-pcf8591-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.745323 adafruit-circuitpython-pcf8591-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-09 18:30:16.749323 adafruit-circuitpython-pcf8591-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.745323 adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4355 2022-06-09 18:30:16.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-06-09 18:30:16.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:30:16.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-09 18:30:16.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 18:30:16.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.745323 adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/analog_out.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/pcf8591.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.749323 adafruit-circuitpython-pcf8591-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.749323 adafruit-circuitpython-pcf8591-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:30:16.749323 adafruit-circuitpython-pcf8591-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_adc_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_dac_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:30:16.749323 adafruit-circuitpython-pcf8591-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-06-09 18:30:04.000000 adafruit-circuitpython-pcf8591-1.0.9/setup.py
```

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pcf8591-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-pcf8591-1.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-pcf8591-1.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/.gitignore` & `adafruit-circuitpython-pcf8591-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pcf8591-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/.pylintrc` & `adafruit-circuitpython-pcf8591-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pcf8591-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/LICENSE` & `adafruit-circuitpython-pcf8591-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pcf8591-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pcf8591-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pcf8591-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/PKG-INFO` & `adafruit-circuitpython-pcf8591-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8591
-Version: 1.0.8
+Version: 1.0.9
 Summary: ADC+DAC Combo
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PCF8591
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython pcf8591 Analog Digital Converter Breakout PCF
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/README.rst` & `adafruit-circuitpython-pcf8591-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/PKG-INFO` & `adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8591
-Version: 1.0.8
+Version: 1.0.9
 Summary: ADC+DAC Combo
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PCF8591
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython pcf8591 Analog Digital Converter Breakout PCF
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/adafruit_circuitpython_pcf8591.egg-info/SOURCES.txt` & `adafruit-circuitpython-pcf8591-1.0.9/adafruit_circuitpython_pcf8591.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/analog_in.py` & `adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/analog_out.py` & `adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/analog_out.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/adafruit_pcf8591/pcf8591.py` & `adafruit-circuitpython-pcf8591-1.0.9/adafruit_pcf8591/pcf8591.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pcf8591-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/docs/conf.py` & `adafruit-circuitpython-pcf8591-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/docs/index.rst` & `adafruit-circuitpython-pcf8591-1.0.9/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 .. toctree::
     :caption: Related Products.
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_PCF8591/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_PCF8591/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_adc_example.py` & `adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_adc_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_analog_in.py` & `adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_dac_example.py` & `adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_dac_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/examples/pcf8591_simpletest.py` & `adafruit-circuitpython-pcf8591-1.0.9/examples/pcf8591_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8591-1.0.8/setup.py` & `adafruit-circuitpython-pcf8591-1.0.9/setup.py`

 * *Files identical despite different names*

