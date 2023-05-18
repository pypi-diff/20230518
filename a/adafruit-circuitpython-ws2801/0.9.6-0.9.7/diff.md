# Comparing `tmp/adafruit-circuitpython-ws2801-0.9.6.tar.gz` & `tmp/adafruit-circuitpython-ws2801-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-ws2801-0.9.6.tar", last modified: Mon Jan 20 20:22:50 2020, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-ws2801-0.9.7.tar", last modified: Wed Feb  5 13:31:22 2020, max compression
```

## Comparing `adafruit-circuitpython-ws2801-0.9.6.tar` & `adafruit-circuitpython-ws2801-0.9.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (115)       85 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (115)       59 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (115)     5824 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (115)     1231 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)     4390 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2913 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     4390 2020-01-20 20:22:50.000000 adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      556 2020-01-20 20:22:50.000000 adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-20 20:22:50.000000 adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       49 2020-01-20 20:22:50.000000 adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       16 2020-01-20 20:22:50.000000 adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)     6998 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/adafruit_ws2801.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (115)      265 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (115)     5185 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (115)      186 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (115)     1393 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/examples/
--rw-r--r--   0 runner    (1001) docker     (115)      837 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/examples/ws2801_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)       49 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-20 20:22:50.894939 adafruit-circuitpython-ws2801-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1834 2020-01-20 20:22:43.000000 adafruit-circuitpython-ws2801-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.715848 adafruit-circuitpython-ws2801-0.9.7/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.711848 adafruit-circuitpython-ws2801-0.9.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.711848 adafruit-circuitpython-ws2801-0.9.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (115)       85 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (115)       59 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     5824 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1231 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)     4390 2020-02-05 13:31:22.715848 adafruit-circuitpython-ws2801-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2913 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.711848 adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     4390 2020-02-05 13:31:18.000000 adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      556 2020-02-05 13:31:22.000000 adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-02-05 13:31:18.000000 adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       49 2020-02-05 13:31:18.000000 adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       16 2020-02-05 13:31:18.000000 adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)     6998 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/adafruit_ws2801.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.711848 adafruit-circuitpython-ws2801-0.9.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.711848 adafruit-circuitpython-ws2801-0.9.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (115)      265 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     5184 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (115)      186 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     1393 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:31:22.715848 adafruit-circuitpython-ws2801-0.9.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (115)      837 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/examples/ws2801_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)       49 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-02-05 13:31:22.715848 adafruit-circuitpython-ws2801-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1834 2020-02-05 13:30:45.000000 adafruit-circuitpython-ws2801-0.9.7/setup.py
```

### Comparing `adafruit-circuitpython-ws2801-0.9.6/.github/workflows/build.yml` & `adafruit-circuitpython-ws2801-0.9.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/.github/workflows/release.yml` & `adafruit-circuitpython-ws2801-0.9.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/.pylintrc` & `adafruit-circuitpython-ws2801-0.9.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ws2801-0.9.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/LICENSE` & `adafruit-circuitpython-ws2801-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/PKG-INFO` & `adafruit-circuitpython-ws2801-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ws2801
-Version: 0.9.6
+Version: 0.9.7
 Summary: CircuitPython library for WS2801 LEDs.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_WS2801
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-ws2801-0.9.6/README.rst` & `adafruit-circuitpython-ws2801-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/PKG-INFO` & `adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ws2801
-Version: 0.9.6
+Version: 0.9.7
 Summary: CircuitPython library for WS2801 LEDs.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_WS2801
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-ws2801-0.9.6/adafruit_circuitpython_ws2801.egg-info/SOURCES.txt` & `adafruit-circuitpython-ws2801-0.9.7/adafruit_circuitpython_ws2801.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/adafruit_ws2801.py` & `adafruit-circuitpython-ws2801-0.9.7/adafruit_ws2801.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/docs/_static/favicon.ico` & `adafruit-circuitpython-ws2801-0.9.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/docs/conf.py` & `adafruit-circuitpython-ws2801-0.9.7/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'sphinx.ext.napoleon',
     'sphinx.ext.todo',
 ]
 
 ### Using busio
 # autodoc_mock_imports = ["digitalio", "busio"]
 
-intersphinx_mapping = {'python': ('https://docs.python.org/3.4', None),'BusDevice': ('https://circuitpython.readthedocs.io/projects/bus_device/en/latest/', None),'CircuitPython': ('https://circuitpython.readthedocs.io/en/latest/', None)}
+intersphinx_mapping = {'python': ('https://docs.python.org/3.4', None),'BusDevice': ('https://circuitpython.readthedocs.io/projects/busdevice/en/latest/', None),'CircuitPython': ('https://circuitpython.readthedocs.io/en/latest/', None)}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 source_suffix = '.rst'
 
 # The master toctree document.
```

### Comparing `adafruit-circuitpython-ws2801-0.9.6/docs/index.rst` & `adafruit-circuitpython-ws2801-0.9.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/examples/ws2801_simpletest.py` & `adafruit-circuitpython-ws2801-0.9.7/examples/ws2801_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ws2801-0.9.6/setup.py` & `adafruit-circuitpython-ws2801-0.9.7/setup.py`

 * *Files identical despite different names*

