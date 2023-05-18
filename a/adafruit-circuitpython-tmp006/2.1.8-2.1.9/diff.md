# Comparing `tmp/adafruit-circuitpython-tmp006-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-tmp006-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tmp006-2.1.8.tar", last modified: Fri Feb  4 20:35:21 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tmp006-2.1.9.tar", last modified: Fri Apr  1 20:05:28 2022, max compression
```

## Comparing `adafruit-circuitpython-tmp006-2.1.8.tar` & `adafruit-circuitpython-tmp006-2.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.244571 adafruit-circuitpython-tmp006-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.236571 adafruit-circuitpython-tmp006-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-02-04 20:35:21.244571 adafruit-circuitpython-tmp006-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-02-04 20:35:21.000000 adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-02-04 20:35:21.000000 adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:35:21.000000 adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 20:35:21.000000 adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:35:21.000000 adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5199 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/adafruit_tmp006.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:21.240571 adafruit-circuitpython-tmp006-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/examples/tmp006_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:35:21.244571 adafruit-circuitpython-tmp006-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-02-04 20:35:04.000000 adafruit-circuitpython-tmp006-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.012054 adafruit-circuitpython-tmp006-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.016054 adafruit-circuitpython-tmp006-2.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.016054 adafruit-circuitpython-tmp006-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.016054 adafruit-circuitpython-tmp006-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-04-01 20:05:27.000000 adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-04-01 20:05:27.000000 adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 20:05:27.000000 adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-04-01 20:05:27.000000 adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-01 20:05:27.000000 adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5197 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/adafruit_tmp006.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/examples/tmp006_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-01 20:05:28.020054 adafruit-circuitpython-tmp006-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-04-01 20:05:14.000000 adafruit-circuitpython-tmp006-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-tmp006-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tmp006-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-tmp006-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-tmp006-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tmp006-2.1.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
 -   repo: https://github.com/python/black
-    rev: 20.8b1
+    rev: 22.3.0
     hooks:
     - id: black
 -   repo: https://github.com/fsfe/reuse-tool
     rev: v0.12.1
     hooks:
     - id: reuse
 -   repo: https://github.com/pre-commit/pre-commit-hooks
```

### Comparing `adafruit-circuitpython-tmp006-2.1.8/.pylintrc` & `adafruit-circuitpython-tmp006-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tmp006-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/LICENSE` & `adafruit-circuitpython-tmp006-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tmp006-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tmp006-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tmp006-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/PKG-INFO` & `adafruit-circuitpython-tmp006-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tmp006
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for TMP006 contactless IR thermometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TMP006
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit contactless ir thermometer temperature tmp006 hardware micropython circuitpython
 Platform: UNKNOWN
@@ -76,20 +76,17 @@
 Ensure your device works with the simple test in the examples folder.
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/tmp006/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TMP006/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-tmp006-2.1.8/README.rst` & `adafruit-circuitpython-tmp006-2.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,15 @@
 Ensure your device works with the simple test in the examples folder.
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/tmp006/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TMP006/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/PKG-INFO` & `adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tmp006
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for TMP006 contactless IR thermometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TMP006
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit contactless ir thermometer temperature tmp006 hardware micropython circuitpython
 Platform: UNKNOWN
@@ -76,20 +76,17 @@
 Ensure your device works with the simple test in the examples folder.
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/tmp006/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TMP006/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-tmp006-2.1.8/adafruit_circuitpython_tmp006.egg-info/SOURCES.txt` & `adafruit-circuitpython-tmp006-2.1.9/adafruit_circuitpython_tmp006.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/adafruit_tmp006.py` & `adafruit-circuitpython-tmp006-2.1.9/adafruit_tmp006.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         b2 = 4.63e-9
         c2 = 13.4
 
         S = S0 * (1 + a1 * (tamb - TREF) + a2 * (tamb - TREF) ** 2)
         VOS = b0 + b1 * (tamb - TREF) + b2 * (tamb - TREF) ** 2
         fVOBJ = (vobj - VOS) + c2 * (vobj - VOS) ** 2
 
-        TOBJ = (tamb ** 4 + (fVOBJ / S)) ** 0.25
+        TOBJ = (tamb**4 + (fVOBJ / S)) ** 0.25
 
         return TOBJ - 273.15  # back to celsius
 
     def _data_ready(self):
         return (self.read_register(_TMP006_CONFIG) & _TMP006_CFG_DRDY) != 0
 
     def _read_sensor_voltage(self):
```

### Comparing `adafruit-circuitpython-tmp006-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tmp006-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/docs/conf.py` & `adafruit-circuitpython-tmp006-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/docs/index.rst` & `adafruit-circuitpython-tmp006-2.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/examples/tmp006_simpletest.py` & `adafruit-circuitpython-tmp006-2.1.9/examples/tmp006_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp006-2.1.8/setup.py` & `adafruit-circuitpython-tmp006-2.1.9/setup.py`

 * *Files identical despite different names*

