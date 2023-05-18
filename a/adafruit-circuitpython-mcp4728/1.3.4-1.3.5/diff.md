# Comparing `tmp/adafruit-circuitpython-mcp4728-1.3.4.tar.gz` & `tmp/adafruit-circuitpython-mcp4728-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp4728-1.3.4.tar", last modified: Mon Nov 21 17:36:01 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp4728-1.3.5.tar", last modified: Mon Nov 28 18:09:54 2022, max compression
```

## Comparing `adafruit-circuitpython-mcp4728-1.3.4.tar` & `adafruit-circuitpython-mcp4728-1.3.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.659960 adafruit-circuitpython-mcp4728-1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.659960 adafruit-circuitpython-mcp4728-1.3.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.659960 adafruit-circuitpython-mcp4728-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.659960 adafruit-circuitpython-mcp4728-1.3.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-11-21 17:36:01.000000 adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2022-11-21 17:36:01.000000 adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 17:36:01.000000 adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-21 17:36:01.000000 adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-21 17:36:01.000000 adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12140 2022-11-21 17:35:53.000000 adafruit-circuitpython-mcp4728-1.3.4/adafruit_mcp4728.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5873 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-11-21 17:35:53.000000 adafruit-circuitpython-mcp4728-1.3.4/examples/mcp4728_generalcalltest.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-21 17:35:53.000000 adafruit-circuitpython-mcp4728-1.3.4/examples/mcp4728_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-11-21 17:35:53.000000 adafruit-circuitpython-mcp4728-1.3.4/examples/mcp4728_vref_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-11-21 17:35:53.000000 adafruit-circuitpython-mcp4728-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-21 17:35:44.000000 adafruit-circuitpython-mcp4728-1.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 17:36:01.663960 adafruit-circuitpython-mcp4728-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.985890 adafruit-circuitpython-mcp4728-1.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.981890 adafruit-circuitpython-mcp4728-1.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.981890 adafruit-circuitpython-mcp4728-1.3.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.981890 adafruit-circuitpython-mcp4728-1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.981890 adafruit-circuitpython-mcp4728-1.3.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3738 2022-11-28 18:09:54.985890 adafruit-circuitpython-mcp4728-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2981 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.981890 adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3738 2022-11-28 18:09:54.000000 adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2022-11-28 18:09:54.000000 adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:09:54.000000 adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-28 18:09:54.000000 adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:09:54.000000 adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12140 2022-11-28 18:09:47.000000 adafruit-circuitpython-mcp4728-1.3.5/adafruit_mcp4728.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.985890 adafruit-circuitpython-mcp4728-1.3.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.985890 adafruit-circuitpython-mcp4728-1.3.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (122)     5873 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:54.985890 adafruit-circuitpython-mcp4728-1.3.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2022-11-28 18:09:47.000000 adafruit-circuitpython-mcp4728-1.3.5/examples/mcp4728_generalcalltest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2022-11-28 18:09:47.000000 adafruit-circuitpython-mcp4728-1.3.5/examples/mcp4728_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2022-11-28 18:09:47.000000 adafruit-circuitpython-mcp4728-1.3.5/examples/mcp4728_vref_example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2022-11-28 18:09:47.000000 adafruit-circuitpython-mcp4728-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2022-11-28 18:09:40.000000 adafruit-circuitpython-mcp4728-1.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:09:54.985890 adafruit-circuitpython-mcp4728-1.3.5/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp4728-1.3.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/.gitignore` & `adafruit-circuitpython-mcp4728-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp4728-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/.pylintrc` & `adafruit-circuitpython-mcp4728-1.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp4728-1.3.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/LICENSE` & `adafruit-circuitpython-mcp4728-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp4728-1.3.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp4728-1.3.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp4728-1.3.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/PKG-INFO` & `adafruit-circuitpython-mcp4728-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp4728
-Version: 1.3.4
+Version: 1.3.5
 Summary: Helper library for the MCP4728 I2C 12-bit Quad DAC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP4728
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4728,dac,12-bit,quad,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/README.rst` & `adafruit-circuitpython-mcp4728-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp4728
-Version: 1.3.4
+Version: 1.3.5
 Summary: Helper library for the MCP4728 I2C 12-bit Quad DAC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP4728
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4728,dac,12-bit,quad,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp4728-1.3.5/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/adafruit_mcp4728.py` & `adafruit-circuitpython-mcp4728-1.3.5/adafruit_mcp4728.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards: https://circuitpython.org/downloads
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP4728.git"
 
 from struct import pack_into
 from time import sleep
 from adafruit_bus_device import i2c_device
 
 try:
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp4728-1.3.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/docs/conf.py` & `adafruit-circuitpython-mcp4728-1.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/docs/examples.rst` & `adafruit-circuitpython-mcp4728-1.3.5/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/docs/index.rst` & `adafruit-circuitpython-mcp4728-1.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/examples/mcp4728_generalcalltest.py` & `adafruit-circuitpython-mcp4728-1.3.5/examples/mcp4728_generalcalltest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2021 codenio (Aananth K)
 # SPDX-License-Identifier: MIT
 
 import board
 import adafruit_mcp4728
 
 i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 mcp4728 = adafruit_mcp4728.MCP4728(i2c)
 
 mcp4728.channel_a.value = 65535  # Voltage = VDD
 mcp4728.channel_b.value = int(65535 / 2)  # VDD/2
 mcp4728.channel_c.value = int(65535 / 4)  # VDD/4
 mcp4728.channel_d.value = 0  # 0V
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/examples/mcp4728_simpletest.py` & `adafruit-circuitpython-mcp4728-1.3.5/examples/mcp4728_simpletest.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import board
 import adafruit_mcp4728
 
 MCP4728_DEFAULT_ADDRESS = 0x60
 MCP4728A4_DEFAULT_ADDRESS = 0x64
 
 i2c = board.I2C()  # uses board.SCL and board.SDA
+# i2c = board.STEMMA_I2C()  # For using the built-in STEMMA QT connector on a microcontroller
 #  use for MCP4728 variant
 mcp4728 = adafruit_mcp4728.MCP4728(i2c, adafruit_mcp4728.MCP4728_DEFAULT_ADDRESS)
 #  use for MCP4728A4 variant
 #  mcp4728 = adafruit_mcp4728.MCP4728(i2c, adafruit_mcp4728.MCP4728A4_DEFAULT_ADDRESS)
 
 mcp4728.channel_a.value = 65535  # Voltage = VDD
 mcp4728.channel_b.value = int(65535 / 2)  # VDD/2
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.4/pyproject.toml` & `adafruit-circuitpython-mcp4728-1.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp4728"
 description = "Helper library for the MCP4728 I2C 12-bit Quad DAC"
-version = "1.3.4"
+version = "1.3.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP4728"}
 keywords = [
     "adafruit",
```

