# Comparing `tmp/adafruit-circuitpython-stmpe610-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-stmpe610-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-stmpe610-1.3.8.tar", last modified: Tue Sep 13 23:43:55 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-stmpe610-1.3.9.tar", last modified: Thu Oct 27 02:40:34 2022, max compression
```

## Comparing `adafruit-circuitpython-stmpe610-1.3.8.tar` & `adafruit-circuitpython-stmpe610-1.3.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.649458 adafruit-circuitpython-stmpe610-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2764 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-09-13 23:43:55.000000 adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-13 23:43:55.000000 adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 23:43:55.000000 adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-13 23:43:55.000000 adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-13 23:43:55.000000 adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    21208 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/adafruit_stmpe610.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2558 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_button_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_paint_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6757 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_touch_calibrator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1226 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_touch_point_paint_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      542 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_touch_point_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-09-13 23:43:48.000000 adafruit-circuitpython-stmpe610-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-13 23:43:40.000000 adafruit-circuitpython-stmpe610-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-13 23:43:55.653458 adafruit-circuitpython-stmpe610-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.688660 adafruit-circuitpython-stmpe610-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2764 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-10-27 02:40:34.000000 adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-10-27 02:40:34.000000 adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 02:40:34.000000 adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-27 02:40:34.000000 adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-27 02:40:34.000000 adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    21178 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/adafruit_stmpe610.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2558 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_button_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_paint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6757 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_touch_calibrator.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1226 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_touch_point_paint_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      542 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_touch_point_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-10-27 02:40:27.000000 adafruit-circuitpython-stmpe610-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-27 02:40:20.000000 adafruit-circuitpython-stmpe610-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 02:40:34.692660 adafruit-circuitpython-stmpe610-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-stmpe610-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-stmpe610-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-stmpe610-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/.gitignore` & `adafruit-circuitpython-stmpe610-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-stmpe610-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/.pylintrc` & `adafruit-circuitpython-stmpe610-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-stmpe610-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/LICENSE` & `adafruit-circuitpython-stmpe610-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-stmpe610-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-stmpe610-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-stmpe610-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/PKG-INFO` & `adafruit-circuitpython-stmpe610-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-stmpe610
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for STMPE610 Resistive Touch Screen Controller.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_STMPE610
 Keywords: adafruit,stmpe610,resistive,touch,screen,controllerhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/README.rst` & `adafruit-circuitpython-stmpe610-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/PKG-INFO` & `adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-stmpe610
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for STMPE610 Resistive Touch Screen Controller.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_STMPE610
 Keywords: adafruit,stmpe610,resistive,touch,screen,controllerhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/adafruit_circuitpython_stmpe610.egg-info/SOURCES.txt` & `adafruit-circuitpython-stmpe610-1.3.9/adafruit_circuitpython_stmpe610.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/adafruit_stmpe610.py` & `adafruit-circuitpython-stmpe610-1.3.9/adafruit_stmpe610.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from typing import Dict, List, Optional, Tuple
     from typing_extensions import Literal
     from microcontroller import Pin
     from busio import I2C, SPI
 except ImportError:
     pass
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_STMPE610.git"
 
 
 def map_range(
     x: float, in_min: float, in_max: float, out_min: float, out_max: float
 ) -> float:
     """
@@ -467,15 +467,14 @@
                 spi, cs, baudrate=baudrate, polarity=0, phase=1
             )
             version = self.get_version
             if _STMPE_VERSION != version:
                 raise RuntimeError(
                     f"Failed to find STMPE610 controller! Chip Version {hex(version).upper()}. "
                     "If you are using the breakout, verify you are in SPI mode."
-                    % version
                 )
         super().__init__()
 
     @property
     def touch_point(  # pylint: disable=too-many-branches
         self,
     ) -> Optional[Tuple[int, int, int]]:
```

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-stmpe610-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/docs/conf.py` & `adafruit-circuitpython-stmpe610-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/docs/index.rst` & `adafruit-circuitpython-stmpe610-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_button_demo.py` & `adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_button_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_paint_demo.py` & `adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_paint_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_touch_calibrator.py` & `adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_touch_calibrator.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_touch_point_paint_demo.py` & `adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_touch_point_paint_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/examples/stmpe610_touch_point_simpletest.py` & `adafruit-circuitpython-stmpe610-1.3.9/examples/stmpe610_touch_point_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-stmpe610-1.3.8/pyproject.toml` & `adafruit-circuitpython-stmpe610-1.3.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-stmpe610"
 description = "CircuitPython library for STMPE610 Resistive Touch Screen Controller."
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_STMPE610"}
 keywords = [
     "adafruit",
```

