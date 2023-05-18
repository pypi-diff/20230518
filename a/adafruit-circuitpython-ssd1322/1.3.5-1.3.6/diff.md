# Comparing `tmp/adafruit-circuitpython-ssd1322-1.3.5.tar.gz` & `tmp/adafruit-circuitpython-ssd1322-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1322-1.3.5.tar", last modified: Mon Aug 22 18:48:03 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1322-1.3.6.tar", last modified: Wed Aug 24 23:26:46 2022, max compression
```

## Comparing `adafruit-circuitpython-ssd1322-1.3.5.tar` & `adafruit-circuitpython-ssd1322-1.3.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.690007 adafruit-circuitpython-ssd1322-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16351 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-08-22 18:48:03.000000 adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-22 18:48:03.000000 adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:48:03.000000 adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 18:48:03.000000 adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 18:48:03.000000 adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4799 2022-08-22 18:47:56.000000 adafruit-circuitpython-ssd1322-1.3.5/adafruit_ssd1322.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-22 18:47:56.000000 adafruit-circuitpython-ssd1322-1.3.5/examples/ssd1322_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-08-22 18:47:56.000000 adafruit-circuitpython-ssd1322-1.3.5/examples/ssd1322_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-22 18:47:56.000000 adafruit-circuitpython-ssd1322-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:47:48.000000 adafruit-circuitpython-ssd1322-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:48:03.694007 adafruit-circuitpython-ssd1322-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.815794 adafruit-circuitpython-ssd1322-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.815794 adafruit-circuitpython-ssd1322-1.3.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.815794 adafruit-circuitpython-ssd1322-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16351 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.815794 adafruit-circuitpython-ssd1322-1.3.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-08-24 23:26:46.000000 adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-24 23:26:46.000000 adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 23:26:46.000000 adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-24 23:26:46.000000 adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-24 23:26:46.000000 adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4851 2022-08-24 23:26:37.000000 adafruit-circuitpython-ssd1322-1.3.6/adafruit_ssd1322.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-24 23:26:37.000000 adafruit-circuitpython-ssd1322-1.3.6/examples/ssd1322_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-08-24 23:26:37.000000 adafruit-circuitpython-ssd1322-1.3.6/examples/ssd1322_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-24 23:26:37.000000 adafruit-circuitpython-ssd1322-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-24 23:26:28.000000 adafruit-circuitpython-ssd1322-1.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 23:26:46.819794 adafruit-circuitpython-ssd1322-1.3.6/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1322-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/.github/workflows/build.yml` & `adafruit-circuitpython-ssd1322-1.3.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/.github/workflows/release.yml` & `adafruit-circuitpython-ssd1322-1.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/.gitignore` & `adafruit-circuitpython-ssd1322-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1322-1.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/.pylintrc` & `adafruit-circuitpython-ssd1322-1.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1322-1.3.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/LICENSE` & `adafruit-circuitpython-ssd1322-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1322-1.3.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1322-1.3.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1322-1.3.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/PKG-INFO` & `adafruit-circuitpython-ssd1322-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1322
-Version: 1.3.5
+Version: 1.3.6
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1322
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1322
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1322,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/README.rst` & `adafruit-circuitpython-ssd1322-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1322
-Version: 1.3.5
+Version: 1.3.6
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1322
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1322
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1322,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1322-1.3.6/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/adafruit_ssd1322.py` & `adafruit-circuitpython-ssd1322-1.3.6/adafruit_ssd1322.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython 5+ firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1322.git"
 
 _INIT_SEQUENCE = (
     b"\xfd\x01\x12"  # Set_Command_Lock(0x12);// Unlock Basic Commands (0x12/0x16)
     b"\xae\x00"  # Set_Display_On_Off(0x00);// Display Off (0x00/0x01)
     b"\xb3\x01\x91"  # Set_Display_Clock(0x91);// Set Clock as 80 Frames/Sec
     b"\xca\x01\x3f"  # Set_Multiplex_Ratio(0x3F);// 1/64 Duty (0x0F~0x3F)
@@ -69,15 +69,15 @@
 
     :param int width: The width of the display
     :param int height: The height of the display
     :param int rotation: The rotation of the display in degrees. Default is 0. Must be one of
         (0, 90, 180, 270)
     """
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
         # Patch the init sequence for 32 pixel high displays.
         init_sequence = bytearray(_INIT_SEQUENCE)
         height = kwargs["height"]
         if "rotation" in kwargs and kwargs["rotation"] % 180 != 0:
             height = kwargs["width"]
         init_sequence[10] = height - 1  # patch mux ratio
         super().__init__(
@@ -92,32 +92,32 @@
             single_byte_bounds=True,
             reverse_pixels_in_byte=True,
             bytes_per_cell=2,
         )
         self._is_awake = True  # Display starts in active state (_INIT_SEQUENCE)
 
     @property
-    def is_awake(self):
+    def is_awake(self) -> bool:
         """
         The power state of the display. (read-only)
         `True` if the display is active, `False` if in sleep mode.
         :type: bool
         """
         return self._is_awake
 
-    def sleep(self):
+    def sleep(self) -> None:
         """
         Put display into sleep mode.
         Display uses < 10uA in sleep mode. Display remembers display data and operation mode
         active prior to sleeping. MP can access (update) the built-in display RAM.
         """
         if self._is_awake:
             self.bus.send(0xAE, b"")  # 0xAE = display off, sleep mode
             self._is_awake = False
 
-    def wake(self):
+    def wake(self) -> None:
         """
         Wake display from sleep mode
         """
         if not self._is_awake:
             self.bus.send(0xAF, b"")  # 0xAF = display on
             self._is_awake = True
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1322-1.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/docs/conf.py` & `adafruit-circuitpython-ssd1322-1.3.6/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -39,15 +40,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit SSD1322 Library"
-copyright = "2019 Scott Shawcroft"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Scott Shawcroft"
 author = "Scott Shawcroft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/docs/index.rst` & `adafruit-circuitpython-ssd1322-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/examples/ssd1322_gamma.py` & `adafruit-circuitpython-ssd1322-1.3.6/examples/ssd1322_gamma.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/examples/ssd1322_simpletest.py` & `adafruit-circuitpython-ssd1322-1.3.6/examples/ssd1322_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.5/pyproject.toml` & `adafruit-circuitpython-ssd1322-1.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1322"
 description = "DisplayIO driver for grayscale OLEDs drive by SSD1322"
-version = "1.3.5"
+version = "1.3.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1322"}
 keywords = [
     "adafruit",
```

