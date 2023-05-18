# Comparing `tmp/playmolecule-1.7.7.tar.gz` & `tmp/playmolecule-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.7.7.tar", last modified: Wed May 17 12:39:21 2023, max compression
+gzip compressed data, was "playmolecule-1.7.8.tar", last modified: Thu May 18 08:58:51 2023, max compression
```

## Comparing `playmolecule-1.7.7.tar` & `playmolecule-1.7.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:21.503035 playmolecule-1.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-17 12:38:55.000000 playmolecule-1.7.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 12:38:55.000000 playmolecule-1.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 12:39:21.503035 playmolecule-1.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-17 12:38:55.000000 playmolecule-1.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:21.503035 playmolecule-1.7.7/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 12:39:21.503035 playmolecule-1.7.7/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    34607 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-17 12:38:55.000000 playmolecule-1.7.7/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:21.503035 playmolecule-1.7.7/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 12:39:21.000000 playmolecule-1.7.7/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-17 12:39:21.000000 playmolecule-1.7.7/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:39:21.000000 playmolecule-1.7.7/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:39:21.000000 playmolecule-1.7.7/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 12:39:21.000000 playmolecule-1.7.7/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 12:39:21.000000 playmolecule-1.7.7/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-17 12:38:55.000000 playmolecule-1.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:39:21.503035 playmolecule-1.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 12:38:55.000000 playmolecule-1.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:39:21.503035 playmolecule-1.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-17 12:38:55.000000 playmolecule-1.7.7/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-17 12:38:55.000000 playmolecule-1.7.7/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-17 12:38:55.000000 playmolecule-1.7.7/tests/test_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-17 12:38:55.000000 playmolecule-1.7.7/tests/test_func_to_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:58:51.078870 playmolecule-1.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-18 08:58:33.000000 playmolecule-1.7.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 08:58:33.000000 playmolecule-1.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-18 08:58:51.078870 playmolecule-1.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-18 08:58:33.000000 playmolecule-1.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:58:51.078870 playmolecule-1.7.8/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 08:58:51.078870 playmolecule-1.7.8/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34606 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-18 08:58:33.000000 playmolecule-1.7.8/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:58:51.078870 playmolecule-1.7.8/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-18 08:58:51.000000 playmolecule-1.7.8/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 08:58:51.000000 playmolecule-1.7.8/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:58:51.000000 playmolecule-1.7.8/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:58:50.000000 playmolecule-1.7.8/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 08:58:51.000000 playmolecule-1.7.8/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 08:58:51.000000 playmolecule-1.7.8/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-18 08:58:33.000000 playmolecule-1.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:58:51.078870 playmolecule-1.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-18 08:58:33.000000 playmolecule-1.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:58:51.078870 playmolecule-1.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-18 08:58:33.000000 playmolecule-1.7.8/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-18 08:58:33.000000 playmolecule-1.7.8/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-18 08:58:33.000000 playmolecule-1.7.8/tests/test_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-18 08:58:33.000000 playmolecule-1.7.8/tests/test_func_to_argparse.py
```

### Comparing `playmolecule-1.7.7/LICENSE.md` & `playmolecule-1.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/PKG-INFO` & `playmolecule-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.7
+Version: 1.7.8
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.7/playmolecule/__init__.py` & `playmolecule-1.7.8/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/_test_funcs.py` & `playmolecule-1.7.8/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/config.py` & `playmolecule-1.7.8/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/datacenter.py` & `playmolecule-1.7.8/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/devutils.py` & `playmolecule-1.7.8/playmolecule/devutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
     _pm_try_except(func, SESSION, JOB, standalone, args.debug, args)
 
     if not standalone:
         # set the complete status of the job
         setAsCompleted(args.outdir)
 
 
-def get_manifest(file, parser, pm_mode=False):
+def get_manifest(file, parser, pm_mode=True):
     from collections import OrderedDict
     import json
 
     manifest = OrderedDict()
     manifestf = os.path.join(os.path.dirname(file), "manifest.json")
     if os.path.exists(manifestf):
         with open(manifestf, "r") as f:
```

### Comparing `playmolecule-1.7.7/playmolecule/func2argparse.py` & `playmolecule-1.7.8/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/job.py` & `playmolecule-1.7.8/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/jsonlogger.py` & `playmolecule-1.7.8/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/local.py` & `playmolecule-1.7.8/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/playqueue.py` & `playmolecule-1.7.8/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/session.py` & `playmolecule-1.7.8/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule/utils.py` & `playmolecule-1.7.8/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.7.8/playmolecule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.7
+Version: 1.7.8
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.7/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.7.8/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/pyproject.toml` & `playmolecule-1.7.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/tests/test.py` & `playmolecule-1.7.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/tests/test_app_wrapper.py` & `playmolecule-1.7.8/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/tests/test_datacenter.py` & `playmolecule-1.7.8/tests/test_datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.7/tests/test_func_to_argparse.py` & `playmolecule-1.7.8/tests/test_func_to_argparse.py`

 * *Files identical despite different names*

