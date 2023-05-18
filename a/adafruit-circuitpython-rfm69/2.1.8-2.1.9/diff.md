# Comparing `tmp/adafruit-circuitpython-rfm69-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-rfm69-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-rfm69-2.1.8.tar", last modified: Tue Jun  7 16:59:29 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-rfm69-2.1.9.tar", last modified: Thu Jun  9 18:08:32 2022, max compression
```

## Comparing `adafruit-circuitpython-rfm69-2.1.8.tar` & `adafruit-circuitpython-rfm69-2.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.382050 adafruit-circuitpython-rfm69-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.374050 adafruit-circuitpython-rfm69-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.378050 adafruit-circuitpython-rfm69-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.378050 adafruit-circuitpython-rfm69-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16257 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.378050 adafruit-circuitpython-rfm69-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-06-07 16:59:29.382050 adafruit-circuitpython-rfm69-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.378050 adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-06-07 16:59:29.000000 adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-06-07 16:59:29.000000 adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:59:29.000000 adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-07 16:59:29.000000 adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-07 16:59:29.000000 adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    39302 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/adafruit_rfm69.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.378050 adafruit-circuitpython-rfm69-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.378050 adafruit-circuitpython-rfm69-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:59:29.382050 adafruit-circuitpython-rfm69-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node1_ack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node1_bonnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node2_ack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_rpi_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_rpi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_transmit.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:59:29.382050 adafruit-circuitpython-rfm69-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-06-07 16:59:15.000000 adafruit-circuitpython-rfm69-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.551009 adafruit-circuitpython-rfm69-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.543009 adafruit-circuitpython-rfm69-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.547009 adafruit-circuitpython-rfm69-2.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.547009 adafruit-circuitpython-rfm69-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16257 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.547009 adafruit-circuitpython-rfm69-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-06-09 18:08:32.551009 adafruit-circuitpython-rfm69-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.547009 adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-06-09 18:08:32.000000 adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-06-09 18:08:32.000000 adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:08:32.000000 adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-09 18:08:32.000000 adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-09 18:08:32.000000 adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    39302 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/adafruit_rfm69.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.547009 adafruit-circuitpython-rfm69-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.547009 adafruit-circuitpython-rfm69-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:08:32.551009 adafruit-circuitpython-rfm69-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node1_ack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node1_bonnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node2_ack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_rpi_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_rpi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_transmit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:08:32.551009 adafruit-circuitpython-rfm69-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-06-09 18:08:09.000000 adafruit-circuitpython-rfm69-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-rfm69-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-rfm69-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-rfm69-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-rfm69-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/.gitignore` & `adafruit-circuitpython-rfm69-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-rfm69-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/.pylintrc` & `adafruit-circuitpython-rfm69-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-rfm69-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/LICENSE` & `adafruit-circuitpython-rfm69-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-rfm69-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-rfm69-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-rfm69-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/PKG-INFO` & `adafruit-circuitpython-rfm69-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rfm69
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for RFM69 packet radio.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RFM69
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit rfm69 packet radio hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-rfm69-2.1.8/README.rst` & `adafruit-circuitpython-rfm69-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/PKG-INFO` & `adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rfm69
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for RFM69 packet radio.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RFM69
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit rfm69 packet radio hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-rfm69-2.1.8/adafruit_circuitpython_rfm69.egg-info/SOURCES.txt` & `adafruit-circuitpython-rfm69-2.1.9/adafruit_circuitpython_rfm69.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/adafruit_rfm69.py` & `adafruit-circuitpython-rfm69-2.1.9/adafruit_rfm69.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-rfm69-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/docs/conf.py` & `adafruit-circuitpython-rfm69-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/docs/index.rst` & `adafruit-circuitpython-rfm69-2.1.9/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     Adafruit Radio FeatherWing - RFM69HCW 900MHz - RadioFruit <https://www.adafruit.com/product/3229>
 
     Adafruit Radio FeatherWing - RFM69HCW 433MHz - RadioFruit <https://www.adafruit.com/product/3230>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_RFM69/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_RFM69/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_header.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_header.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node1.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node1.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node1_ack.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node1_ack.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node1_bonnet.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node1_bonnet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node2.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_node2_ack.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_node2_ack.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_rpi_interrupt.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_rpi_interrupt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_rpi_simpletest.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_rpi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_simpletest.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/examples/rfm69_transmit.py` & `adafruit-circuitpython-rfm69-2.1.9/examples/rfm69_transmit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm69-2.1.8/setup.py` & `adafruit-circuitpython-rfm69-2.1.9/setup.py`

 * *Files identical despite different names*

