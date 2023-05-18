# Comparing `tmp/pycmx-1.1.5.tar.gz` & `tmp/pycmx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmx-1.1.5.tar", last modified: Sat Nov 19 07:06:23 2022, max compression
+gzip compressed data, was "pycmx-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pycmx-1.1.5.tar` & `pycmx-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 07:06:23.203244 pycmx-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-11-19 07:06:07.000000 pycmx-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-11-19 07:06:23.203244 pycmx-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-11-19 07:06:07.000000 pycmx-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 07:06:23.203244 pycmx-1.1.5/pycmx/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3116 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/channel_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/edit.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/edit_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/parse_cmx_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     6668 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/parse_cmx_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/transition.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-11-19 07:06:07.000000 pycmx-1.1.5/pycmx/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 07:06:23.203244 pycmx-1.1.5/pycmx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-11-19 07:06:23.000000 pycmx-1.1.5/pycmx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-19 07:06:23.000000 pycmx-1.1.5/pycmx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 07:06:23.000000 pycmx-1.1.5/pycmx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-19 07:06:23.000000 pycmx-1.1.5/pycmx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-19 07:06:23.203244 pycmx-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-19 07:06:07.000000 pycmx-1.1.5/setup.py
+-rw-r--r--   0        0        0     2803 2023-05-18 00:06:45.586033 pycmx-1.2.0/README.md
+-rw-r--r--   0        0        0      444 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/__init__.py
+-rw-r--r--   0        0        0     3116 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/channel_map.py
+-rw-r--r--   0        0        0     3624 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/edit.py
+-rw-r--r--   0        0        0     2993 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/edit_list.py
+-rw-r--r--   0        0        0     3156 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/event.py
+-rw-r--r--   0        0        0      463 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/parse_cmx_events.py
+-rw-r--r--   0        0        0     6668 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/parse_cmx_statements.py
+-rw-r--r--   0        0        0     2258 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/transition.py
+-rw-r--r--   0        0        0      801 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/util.py
+-rw-r--r--   0        0        0     1465 2023-05-18 00:06:45.586033 pycmx-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 pycmx-1.2.0/PKG-INFO
```

### Comparing `pycmx-1.1.5/PKG-INFO` & `pycmx-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: pycmx
-Version: 1.1.5
-Summary: CMX 3600 Edit Decision List Parser
-Home-page: https://github.com/iluvcapra/pycmx
-Author: Jamie Hardt
-Author-email: jamiehardt@me.com
-Project-URL: Source, https://github.com/iluvcapra/pycmx
-Project-URL: Documentation, https://pycmx.readthedocs.io/
-Project-URL: Issues, https://github.com/iluvcapra/pycmx/issues
+Version: 1.2.0
+Summary: pycmx is a module for parsing CMX 3600-style EDLs. For more information and
+Keywords: parser,film,broadcast
+Author-email: Jamie Hardt <jamiehardt@me.com>
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Text Processing
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: sphinx >= 5.3.0 ; extra == "doc"
+Requires-Dist: sphinx_rtd_theme >= 1.1.1 ; extra == "doc"
+Project-URL: Documentation, https://pycmx.readthedocs.io/
+Project-URL: Home, https://github.com/iluvcapra/pycmx
+Project-URL: Issues, https://github.com/iluvcapra/pycmx/issues
+Project-URL: Source, https://github.com/iluvcapra/pycmx.git
+Provides-Extra: doc
 
 [![Documentation Status](https://readthedocs.org/projects/pycmx/badge/?version=latest)](https://pycmx.readthedocs.io/en/latest/?badge=latest) ![](https://img.shields.io/github/license/iluvcapra/pycmx.svg) ![](https://img.shields.io/pypi/pyversions/pycmx.svg) [![](https://img.shields.io/pypi/v/pycmx.svg)](https://pypi.org/project/pycmx/) ![](https://img.shields.io/pypi/wheel/pycmx.svg)
 ![GitHub last commit](https://img.shields.io/github/last-commit/iluvcapra/pycmx)
 [![Lint and Test](https://github.com/iluvcapra/pycmx/actions/workflows/python-package.yml/badge.svg)](https://github.com/iluvcapra/pycmx/actions/workflows/python-package.yml)
 
 
 # pycmx
@@ -104,7 +107,8 @@
 ... 
 Audio channel 7 is present
 >>> events[2].edits[0].channels.video
 False
 ```
 
 
+
```

### Comparing `pycmx-1.1.5/README.md` & `pycmx-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/channel_map.py` & `pycmx-1.2.0/pycmx/channel_map.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/edit.py` & `pycmx-1.2.0/pycmx/edit.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/edit_list.py` & `pycmx-1.2.0/pycmx/edit_list.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/event.py` & `pycmx-1.2.0/pycmx/event.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/parse_cmx_statements.py` & `pycmx-1.2.0/pycmx/parse_cmx_statements.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/transition.py` & `pycmx-1.2.0/pycmx/transition.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.1.5/pycmx/util.py` & `pycmx-1.2.0/pycmx/util.py`

 * *Files identical despite different names*

