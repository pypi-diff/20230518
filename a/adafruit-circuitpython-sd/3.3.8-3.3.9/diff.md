# Comparing `tmp/adafruit-circuitpython-sd-3.3.8.tar.gz` & `tmp/adafruit-circuitpython-sd-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-sd-3.3.8.tar", last modified: Mon Mar 28 19:11:25 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-sd-3.3.9.tar", last modified: Mon Apr 25 17:52:59 2022, max compression
```

## Comparing `adafruit-circuitpython-sd-3.3.8.tar` & `adafruit-circuitpython-sd-3.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.753104 adafruit-circuitpython-sd-3.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.745104 adafruit-circuitpython-sd-3.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.749104 adafruit-circuitpython-sd-3.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.749104 adafruit-circuitpython-sd-3.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.749104 adafruit-circuitpython-sd-3.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-03-28 19:11:25.753104 adafruit-circuitpython-sd-3.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.749104 adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-03-28 19:11:25.000000 adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-03-28 19:11:25.000000 adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 19:11:25.000000 adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-03-28 19:11:25.000000 adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-28 19:11:25.000000 adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17468 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/adafruit_sdcard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.753104 adafruit-circuitpython-sd-3.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.753104 adafruit-circuitpython-sd-3.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:11:25.753104 adafruit-circuitpython-sd-3.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/examples/sd_read_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-28 19:11:25.753104 adafruit-circuitpython-sd-3.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-03-28 19:11:11.000000 adafruit-circuitpython-sd-3.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.289982 adafruit-circuitpython-sd-3.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.289982 adafruit-circuitpython-sd-3.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.289982 adafruit-circuitpython-sd-3.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.289982 adafruit-circuitpython-sd-3.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3679 2022-04-25 17:52:59.000000 adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-04-25 17:52:59.000000 adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 17:52:59.000000 adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-04-25 17:52:59.000000 adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-25 17:52:59.000000 adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18621 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/adafruit_sdcard.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/examples/sd_read_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 17:52:59.293982 adafruit-circuitpython-sd-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-04-25 17:52:48.000000 adafruit-circuitpython-sd-3.3.9/setup.py
```

### Comparing `adafruit-circuitpython-sd-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-sd-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-sd-3.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-sd-3.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-sd-3.3.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-sd-3.3.8/.pylintrc` & `adafruit-circuitpython-sd-3.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-sd-3.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/LICENSE` & `adafruit-circuitpython-sd-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-sd-3.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-sd-3.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-sd-3.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/PKG-INFO` & `adafruit-circuitpython-sd-3.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sd
-Version: 3.3.8
+Version: 3.3.9
 Summary: CircuitPython library for SD cards.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SD
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit sdcard sd card mount storage featherwing adaloggerbreakout hardware micropython circuitpython
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-sd/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/sd/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SD/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SD/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-sd-3.3.8/README.rst` & `adafruit-circuitpython-sd-3.3.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-sd/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/sd/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SD/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SD/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/PKG-INFO` & `adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sd
-Version: 3.3.8
+Version: 3.3.9
 Summary: CircuitPython library for SD cards.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SD
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit sdcard sd card mount storage featherwing adaloggerbreakout hardware micropython circuitpython
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-sd/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/sd/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_SD/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_SD/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-sd-3.3.8/adafruit_circuitpython_sd.egg-info/SOURCES.txt` & `adafruit-circuitpython-sd-3.3.9/adafruit_circuitpython_sd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/adafruit_sdcard.py` & `adafruit-circuitpython-sd-3.3.9/adafruit_sdcard.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 import time
 from micropython import const
 from adafruit_bus_device import spi_device
 
+try:
+    from typing import Union, Optional
+    from busio import SPI
+    from digitalio import DigitalInOut
+    from circuitpython_typing import ReadableBuffer, WriteableBuffer
+except ImportError:
+    pass
+
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SD.git"
 
 _CMD_TIMEOUT = const(200)
 
 _R1_IDLE_STATE = const(1 << 0)
 # R1_ERASE_RESET = const(1 << 1)
@@ -82,15 +90,15 @@
         sd = adafruit_sdcard.SDCard(spi, board.SD_CS)
         vfs = storage.VfsFat(sdcard)
         storage.mount(vfs, '/sd')
         os.listdir('/')
 
     """
 
-    def __init__(self, spi, cs, baudrate=1320000):
+    def __init__(self, spi: SPI, cs: DigitalInOut, baudrate: int = 1320000) -> None:
         # Create an SPIDevice running at a lower initialization baudrate first.
         self._spi = spi_device.SPIDevice(spi, cs, baudrate=250000, extra_clocks=8)
 
         self._cmdbuf = bytearray(6)
         self._single_byte = bytearray(1)
 
         # Card is byte addressing, set to 1 if addresses are per block
@@ -98,15 +106,15 @@
 
         # initialise the card
         self._init_card(cs)
 
         # Create a new SPIDevice with the (probably) higher operating baudrate.
         self._spi = spi_device.SPIDevice(spi, cs, baudrate=baudrate, extra_clocks=8)
 
-    def _init_card(self, chip_select):
+    def _init_card(self, chip_select: DigitalInOut) -> None:
         """Initialize the card in SPI mode."""
         # clock card at least 80 cycles with cs high
         with self._spi as card:
             # Force CS high.
             chip_select.value = True
             self._single_byte[0] = 0xFF
             for _ in range(80 // 8 + 1):
@@ -148,24 +156,24 @@
                 mult = 2 ** (((csd[9] & 0x3) << 1 | (csd[10] & 0x80) >> 7) + 2)
                 self._sectors = block_length // 512 * mult * (c_size + 1)
 
             # CMD16: set block length to 512 bytes
             if self._cmd(card, 16, 512, 0x15) != 0:
                 raise OSError("can't set 512 block size")
 
-    def _init_card_v1(self, card):
+    def _init_card_v1(self, card: SPI) -> None:
         """Initialize v1 SDCards which use byte addressing."""
         for _ in range(_CMD_TIMEOUT):
             self._cmd(card, 55, 0, 0)
             if self._cmd(card, 41, 0, 0) == 0:
                 # print("[SDCard] v1 card")
                 return
         raise OSError("timeout waiting for v1 card")
 
-    def _init_card_v2(self, card):
+    def _init_card_v2(self, card: SPI) -> None:
         """Initialize v2 SDCards which use 512-byte block addressing."""
         ocr = bytearray(4)
         for _ in range(_CMD_TIMEOUT):
             time.sleep(0.050)
             self._cmd(card, 58, 0, 0xFD, response_buf=ocr, data_block=False)
             self._cmd(card, 55, 0, 0x65)
             # On non-longint builds, we cannot use 0x40000000 directly as the arg
@@ -176,15 +184,15 @@
                 # Check for block addressing
                 if (ocr[0] & 0x40) != 0:
                     self._cdv = 1
                 # print("[SDCard] v2 card")
                 return
         raise OSError("timeout waiting for v2 card")
 
-    def _wait_for_ready(self, card, timeout=0.3):
+    def _wait_for_ready(self, card: SPI, timeout: float = 0.3) -> None:
         """
         Wait for the card to clock out 0xff to indicate its ready.
 
         :param busio.SPI card: The locked SPI bus.
         :param float timeout: Maximum time to wait in seconds.
         """
         start_time = time.monotonic()
@@ -192,25 +200,33 @@
         while time.monotonic() - start_time < timeout and self._single_byte[0] != 0xFF:
             card.readinto(self._single_byte, write_value=0xFF)
 
     # pylint: disable-msg=too-many-arguments
     # pylint: disable=no-member
     # no-member disable should be reconsidered when it can be tested
     def _cmd(
-        self, card, cmd, arg=0, crc=0, response_buf=None, data_block=True, wait=True
-    ):
+        self,
+        card: SPI,
+        cmd: int,
+        arg: Union[int, ReadableBuffer] = 0,
+        crc: int = 0,
+        response_buf: Optional[WriteableBuffer] = None,
+        data_block: bool = True,
+        wait: bool = True,
+    ) -> int:
         """
         Issue a command to the card and read an optional data response.
 
         :param busio.SPI card: The locked SPI bus.
         :param int cmd: The command number.
         :param int|buf(4) arg: The command argument
         :param int crc: The crc to allow the card to verify the command and argument.
-        :param bytearray response_buf: Buffer to read a data block response into.
+        :param WriteableBuffer response_buf: Buffer to read a data block response into.
         :param bool data_block: True if the response data is in a data block.
+        :param bool wait: True if the command should wait until the card is ready
         """
         # create and send the command
         buf = self._cmdbuf
         buf[0] = 0x40 | cmd
         if isinstance(arg, int):
             buf[1] = (arg >> 24) & 0xFF
             buf[2] = (arg >> 16) & 0xFF
@@ -248,22 +264,30 @@
                         card.readinto(buf, start=1, end=3, write_value=0xFF)
                 return buf[0]
         return -1
 
     # pylint: enable-msg=too-many-arguments
 
     # pylint: disable-msg=too-many-arguments
-    def _block_cmd(self, card, cmd, block, crc, response_buf=None):
+    def _block_cmd(
+        self,
+        card: SPI,
+        cmd: int,
+        block: int,
+        crc: int,
+        response_buf: Optional[WriteableBuffer] = None,
+    ) -> int:
         """
         Issue a command to the card with a block argument.
 
         :param busio.SPI card: The locked SPI bus.
         :param int cmd: The command number.
         :param int block: The relevant block.
         :param int crc: The crc to allow the card to verify the command and argument.
+        :param WriteableBuffer response_buf: Buffer to read a data block response into.
         """
         if self._cdv == 1:
             return self._cmd(card, cmd, block, crc, response_buf=response_buf)
 
         # create and send the command
         buf = self._cmdbuf
         buf[0] = 0x40 | cmd
@@ -297,38 +321,41 @@
         if response_buf != None and result == 0:
             self._readinto(card, response_buf)
 
         return result
 
     # pylint: enable-msg=too-many-arguments
 
-    def _cmd_nodata(self, card, cmd, response=0xFF):
+    def _cmd_nodata(self, card: SPI, cmd: int, response: int = 0xFF) -> int:
         """
         Issue a command to the card with no argument.
 
         :param busio.SPI card: The locked SPI bus.
         :param int cmd: The command number.
+        :param int response: The expected response, default is ``0xFF``
         """
         buf = self._cmdbuf
         buf[0] = cmd
         buf[1] = 0xFF
 
         card.write(buf, end=2)
         for _ in range(_CMD_TIMEOUT):
             card.readinto(buf, end=1, write_value=0xFF)
             if buf[0] == response:
                 return 0  # OK
         return 1  # timeout
 
-    def _readinto(self, card, buf, start=0, end=None):
+    def _readinto(
+        self, card: SPI, buf: WriteableBuffer, start: int = 0, end: Optional[int] = None
+    ) -> None:
         """
         Read a data block into buf.
 
         :param busio.SPI card: The locked SPI bus.
-        :param bytearray buf: The buffer to write into
+        :param WriteableBuffer buf: The buffer to write into
         :param int start: The first index to write data at
         :param int end: The index after the last byte to write to.
         """
         if end is None:
             end = len(buf)
 
         # read until start byte (0xfe)
@@ -338,21 +365,28 @@
 
         card.readinto(buf, start=start, end=end, write_value=0xFF)
 
         # read checksum and throw it away
         card.readinto(self._cmdbuf, end=2, write_value=0xFF)
 
     # pylint: disable-msg=too-many-arguments
-    def _write(self, card, token, buf, start=0, end=None):
+    def _write(
+        self,
+        card: SPI,
+        token: int,
+        buf: ReadableBuffer,
+        start: int = 0,
+        end: Optional[int] = None,
+    ) -> int:
         """
         Write a data block to the card.
 
         :param busio.SPI card: The locked SPI bus.
         :param int token: The start token
-        :param bytearray buf: The buffer to write from
+        :param ReadableBuffer buf: The buffer to write from
         :param int start: The first index to read data from
         :param int end: The index after the last byte to read from.
         """
         cmd = self._cmdbuf
         if end is None:
             end = len(buf)
 
@@ -382,29 +416,29 @@
         while cmd[0] == 0:
             card.readinto(cmd, end=1, write_value=0xFF)
 
         return 0  # worked
 
     # pylint: enable-msg=too-many-arguments
 
-    def count(self):
+    def count(self) -> int:
         """
         Returns the total number of sectors.
 
         :return: The number of 512-byte blocks
         :rtype: int
         """
         return self._sectors
 
-    def readblocks(self, start_block, buf):
+    def readblocks(self, start_block: int, buf: WriteableBuffer) -> int:
         """
         Read one or more blocks from the card
 
         :param int start_block: The block to start reading from
-        :param bytearray buf: The buffer to write into. Length must be multiple of 512.
+        :param WriteableBuffer buf: The buffer to write into. Length must be multiple of 512.
         """
         nblocks, err = divmod(len(buf), 512)
         assert nblocks and not err, "Buffer length is invalid"
         with self._spi as card:
             if nblocks == 1:
                 # CMD17: set read address for single block
                 # We use _block_cmd to read our data so that the chip select line
@@ -425,20 +459,20 @@
                 while ret != 0:
                     card.readinto(self._single_byte, write_value=0xFF)
                     if self._single_byte[0] & 0x80:
                         return ret
                     ret = self._single_byte[0]
         return 0
 
-    def writeblocks(self, start_block, buf):
+    def writeblocks(self, start_block: int, buf: ReadableBuffer) -> int:
         """
         Write one or more blocks to the card
 
         :param int start_block: The block to start writing to
-        :param bytearray buf: The buffer to write into. Length must be multiple of 512.
+        :param ReadableBuffer buf: The buffer to write into. Length must be multiple of 512.
         """
         nblocks, err = divmod(len(buf), 512)
         assert nblocks and not err, "Buffer length is invalid"
         with self._spi as card:
             if nblocks == 1:
                 # CMD24: set write address for single block
                 if self._block_cmd(card, 24, start_block, 0) != 0:
@@ -458,15 +492,15 @@
                     )
                     offset += 512
                     nblocks -= 1
                 self._cmd_nodata(card, _TOKEN_STOP_TRAN, 0x0)
         return 0
 
 
-def _calculate_crc_table():
+def _calculate_crc_table() -> bytearray:
     """Precompute the table used in calculate_crc."""
     # Code converted from https://github.com/hazelnusse/crc7/blob/master/crc7.cc by devoh747
     # With permission from Dale Lukas Peterson <hazelnusse@gmail.com>
     # 8/6/2019
 
     crc_table = bytearray(256)
     crc_poly = const(0x89)  # the value of our CRC-7 polynomial
@@ -483,15 +517,15 @@
                 crc_table[i] = crc_table[i] ^ crc_poly
     return crc_table
 
 
 CRC_TABLE = _calculate_crc_table()
 
 
-def calculate_crc(message):
+def calculate_crc(message: ReadableBuffer) -> int:
     """
     Calculate the CRC of message[0:5], using a precomputed table in CRC_TABLE.
 
     :param bytearray message: Where each index is a byte
     """
 
     crc = 0
```

### Comparing `adafruit-circuitpython-sd-3.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-sd-3.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/docs/conf.py` & `adafruit-circuitpython-sd-3.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/docs/index.rst` & `adafruit-circuitpython-sd-3.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/examples/sd_read_simpletest.py` & `adafruit-circuitpython-sd-3.3.9/examples/sd_read_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sd-3.3.8/setup.py` & `adafruit-circuitpython-sd-3.3.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     long_description=long_description,
     long_description_content_type="text/x-rst",
     # The project's main homepage.
     url="https://github.com/adafruit/Adafruit_CircuitPython_SD",
     # Author details
     author="Adafruit Industries",
     author_email="circuitpython@adafruit.com",
-    install_requires=["Adafruit-Blinka", "adafruit-circuitpython-busdevice"],
+    install_requires=[
+        "Adafruit-Blinka>=7.0.0",
+        "adafruit-circuitpython-busdevice",
+        "adafruit-circuitpython-typing",
+    ],
     # Choose your license
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
```

