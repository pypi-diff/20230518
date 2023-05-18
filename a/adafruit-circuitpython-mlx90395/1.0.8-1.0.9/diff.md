# Comparing `tmp/adafruit-circuitpython-mlx90395-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-mlx90395-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mlx90395-1.0.8.tar", last modified: Fri Aug 26 02:26:11 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mlx90395-1.0.9.tar", last modified: Sun Oct 30 17:28:03 2022, max compression
```

## Comparing `adafruit-circuitpython-mlx90395-1.0.8.tar` & `adafruit-circuitpython-mlx90395-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.945835 adafruit-circuitpython-mlx90395-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-08-26 02:26:11.000000 adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-08-26 02:26:11.000000 adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:26:11.000000 adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:26:11.000000 adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-26 02:26:11.000000 adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8051 2022-08-26 02:26:04.000000 adafruit-circuitpython-mlx90395-1.0.8/adafruit_mlx90395.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5996 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-08-26 02:26:04.000000 adafruit-circuitpython-mlx90395-1.0.8/examples/mlx90395_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-26 02:26:04.000000 adafruit-circuitpython-mlx90395-1.0.8/examples/mlx90395_tuning.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-08-26 02:26:04.000000 adafruit-circuitpython-mlx90395-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:25:57.000000 adafruit-circuitpython-mlx90395-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:26:11.949835 adafruit-circuitpython-mlx90395-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.672413 adafruit-circuitpython-mlx90395-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.664413 adafruit-circuitpython-mlx90395-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-10-30 17:28:03.000000 adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-30 17:28:03.000000 adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 17:28:03.000000 adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-10-30 17:28:03.000000 adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-30 17:28:03.000000 adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8432 2022-10-30 17:27:54.000000 adafruit-circuitpython-mlx90395-1.0.9/adafruit_mlx90395.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5996 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 17:28:03.668413 adafruit-circuitpython-mlx90395-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-10-30 17:27:54.000000 adafruit-circuitpython-mlx90395-1.0.9/examples/mlx90395_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-10-30 17:27:54.000000 adafruit-circuitpython-mlx90395-1.0.9/examples/mlx90395_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-10-30 17:27:54.000000 adafruit-circuitpython-mlx90395-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-30 17:27:45.000000 adafruit-circuitpython-mlx90395-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 17:28:03.672413 adafruit-circuitpython-mlx90395-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mlx90395-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-mlx90395-1.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-mlx90395-1.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/.gitignore` & `adafruit-circuitpython-mlx90395-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-mlx90395-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/.pylintrc` & `adafruit-circuitpython-mlx90395-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mlx90395-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/LICENSE` & `adafruit-circuitpython-mlx90395-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mlx90395-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-mlx90395-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mlx90395-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/PKG-INFO` & `adafruit-circuitpython-mlx90395-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mlx90395
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython helper library for using the Adafruit MLX90395 tri-Axis magnetometer breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MLX90395
 Keywords: adafruit,blinka,circuitpython,micropython,mlx90395,magnet,position,magnetometer,3-axis,hard,iron
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/README.rst` & `adafruit-circuitpython-mlx90395-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/PKG-INFO` & `adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mlx90395
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython helper library for using the Adafruit MLX90395 tri-Axis magnetometer breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MLX90395
 Keywords: adafruit,blinka,circuitpython,micropython,mlx90395,magnet,position,magnetometer,3-axis,hard,iron
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/adafruit_circuitpython_mlx90395.egg-info/SOURCES.txt` & `adafruit-circuitpython-mlx90395-1.0.9/adafruit_circuitpython_mlx90395.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/adafruit_mlx90395.py` & `adafruit-circuitpython-mlx90395-1.0.9/adafruit_mlx90395.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,21 @@
 
 # from adafruit_register.i2c_struct import ROUnaryStruct, Struct
 from adafruit_register.i2c_bits import RWBits
 from adafruit_register.i2c_struct import UnaryStruct
 
 # from adafruit_register.i2c_bit import RWBit
 
-__version__ = "1.0.8"
+try:
+    from typing import Iterable, Optional, Tuple, Union
+    from busio import I2C
+except ImportError:
+    pass
+
+__version__ = "1.0.9"
 __repo__ = "https:#github.com/adafruit/Adafruit_CircuitPython_MLX90395.git"
 
 _DEFAULT_ADDR = const(0x0C)  ## Can also be 0x18, depending on IC */
 
 _STATUS_RESET = const(0x02)
 _STATUS_SMMODE = const(0x20)
 _STATUS_DRDY = const(0x01)
@@ -83,27 +89,29 @@
 ]
 
 
 class CV:
     """struct helper"""
 
     @classmethod
-    def add_values(cls, value_tuples):
+    def add_values(
+        cls, value_tuples: Iterable[Tuple[str, int, Union[str, int], Optional[float]]]
+    ) -> None:
         "creates CV entires"
         cls.string = {}
         cls.lsb = {}
 
         for value_tuple in value_tuples:
             name, value, string, lsb = value_tuple
             setattr(cls, name, value)
             cls.string[value] = string
             cls.lsb[value] = lsb
 
     @classmethod
-    def is_valid(cls, value):
+    def is_valid(cls, value: int) -> bool:
         "Returns true if the given value is a member of the CV"
         return value in cls.string
 
 
 class OSR(CV):
     """Options for ``oversample_rate``"""
 
@@ -168,88 +176,88 @@
     _osr = RWBits(2, _REG_2, 0, 2, False)
     _reg0 = UnaryStruct(
         _REG_0,
         ">H",
     )
     _reg2 = UnaryStruct(_REG_2, ">H")
 
-    def __init__(self, i2c_bus, address=_DEFAULT_ADDR):
+    def __init__(self, i2c_bus: I2C, address: int = _DEFAULT_ADDR) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         self._ut_lsb = None
         self._gain_val = 0
         self._buffer = bytearray(12)
 
         self.reset()
         self.initialize()
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset the sensor to it's power-on state"""
 
         self._command(_REG_EX)
         self._command(_REG_EX)
 
         sleep(0.10)
         if self._command(_REG_RT) != _STATUS_RESET:
             raise RuntimeError("Unable to reset!")
 
         sleep(0.10)
 
-    def initialize(self):
+    def initialize(self) -> None:
         """Configure the sensor for use"""
         self._gain_val = self.gain
         if self._gain_val == 8:  # default high field gain
             self._ut_lsb = 7.14
         else:
             self._ut_lsb = 2.5  # medium field gain
 
     @property
-    def resolution(self):
+    def resolution(self) -> int:
         """The current resolution setting for the magnetometer"""
         return self._resolution
 
     @resolution.setter
-    def resolution(self, value):
+    def resolution(self, value: int) -> None:
         if not Resolution.is_valid(value):
             raise AttributeError("resolution must be a Resolution")
         self._resolution = value
 
     @property
-    def gain(self):
+    def gain(self) -> int:
         """The gain applied to the magnetometer's ADC."""
         return self._gain
 
     @gain.setter
-    def gain(self, value):
+    def gain(self, value: int) -> None:
         if not Gain.is_valid(value):
             raise AttributeError("gain must be a valid value")
         self._gain = value
         self._gain_val = value
 
-    def _command(self, command_id):
+    def _command(self, command_id: int) -> int:
 
         buffer = bytearray([0x80, command_id])
         with self.i2c_device as i2c:
             i2c.write_then_readinto(buffer, buffer, in_end=1)
         return buffer[0]
 
     @property
-    def magnetic(self):
+    def magnetic(self) -> Tuple[float, float, float]:
         """The processed magnetometer sensor values.
         A 3-tuple of X, Y, Z axis values in microteslas that are signed floats.
         """
         if self._command(_REG_SM | 0x0F) != _STATUS_SMMODE:
             raise RuntimeError("Unable to initiate a single reading")
         res = self._read_measurement()
         while res is None:
             sleep(0.001)
             res = self._read_measurement()
 
         return res
 
-    def _read_measurement(self):
+    def _read_measurement(self) -> Tuple[float, float, float]:
 
         # clear the buffer
         for i in range(len(self._buffer)):  # pylint: disable=consider-using-enumerate
             self._buffer[i] = 0
         self._buffer[0] = 0x80  # read memory command
 
         with self.i2c_device as i2c:
@@ -260,16 +268,16 @@
 
         x_raw, y_raw, z_raw = unpack_from(">hhh", self._buffer, offset=2)
 
         scalar = GAIN_AMOUNT[self._gain_val] * self._ut_lsb
         return (x_raw * scalar, y_raw * scalar, z_raw * scalar)
 
     @property
-    def oversample_rate(self):
+    def oversample_rate(self) -> int:
         """The number of times that the measurements are re-sampled and averaged to reduce noise"""
         return self._osr
 
     @oversample_rate.setter
-    def oversample_rate(self, value):
+    def oversample_rate(self, value: int) -> None:
         if not OSR.is_valid(value):
             raise AttributeError("oversample_rate must be an OSR")
         self._osr = value
```

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-mlx90395-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/docs/conf.py` & `adafruit-circuitpython-mlx90395-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/docs/index.rst` & `adafruit-circuitpython-mlx90395-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/examples/mlx90395_tuning.py` & `adafruit-circuitpython-mlx90395-1.0.9/examples/mlx90395_tuning.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90395-1.0.8/pyproject.toml` & `adafruit-circuitpython-mlx90395-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mlx90395"
 description = "CircuitPython helper library for using the Adafruit MLX90395 tri-Axis magnetometer breakout"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MLX90395"}
 keywords = [
     "adafruit",
```

