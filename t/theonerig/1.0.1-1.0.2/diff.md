# Comparing `tmp/theonerig-1.0.1.tar.gz` & `tmp/theonerig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theonerig-1.0.1.tar", last modified: Wed May 17 14:47:57 2023, max compression
+gzip compressed data, was "theonerig-1.0.2.tar", last modified: Thu May 18 13:01:45 2023, max compression
```

## Comparing `theonerig-1.0.1.tar` & `theonerig-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-17 14:47:57.021815 theonerig-1.0.1/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    11357 2023-05-17 08:46:59.000000 theonerig-1.0.1/LICENSE
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     5106 2023-05-17 14:47:57.021815 theonerig-1.0.1/PKG-INFO
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     4445 2023-05-17 14:38:35.000000 theonerig-1.0.1/README.md
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       38 2023-05-17 14:47:57.021815 theonerig-1.0.1/setup.cfg
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     1897 2023-05-17 14:47:00.000000 theonerig-1.0.1/setup.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-17 14:47:57.017815 theonerig-1.0.1/theonerig/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       22 2023-05-17 14:38:19.000000 theonerig-1.0.1/theonerig/__init__.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      814 2023-05-17 14:38:19.000000 theonerig-1.0.1/theonerig/_modidx.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    10718 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/_nbdev.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    27014 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/core.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     5414 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/database.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     6699 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/eyetrack.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    15148 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/leddome.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    20955 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/modelling.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)   110396 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/plotting.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    35828 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/processing.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-17 14:47:57.021815 theonerig-1.0.1/theonerig/synchro/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)        0 2023-05-17 14:38:19.000000 theonerig-1.0.1/theonerig/synchro/__init__.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    11249 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/synchro/extracting.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    61175 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/synchro/io.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    26036 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/synchro/nested_stims.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    23284 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/synchro/processing.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     1903 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/testdata.py
--rw-rw-r--   0 tristan   (1000) tristan   (1000)    35031 2023-05-17 08:46:59.000000 theonerig-1.0.1/theonerig/utils.py
-drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-17 14:47:57.017815 theonerig-1.0.1/theonerig.egg-info/
--rw-rw-r--   0 tristan   (1000) tristan   (1000)     5106 2023-05-17 14:47:56.000000 theonerig-1.0.1/theonerig.egg-info/PKG-INFO
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      630 2023-05-17 14:47:56.000000 theonerig-1.0.1/theonerig.egg-info/SOURCES.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)        1 2023-05-17 14:47:56.000000 theonerig-1.0.1/theonerig.egg-info/dependency_links.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)        1 2023-05-17 08:50:04.000000 theonerig-1.0.1/theonerig.egg-info/not-zip-safe
--rw-rw-r--   0 tristan   (1000) tristan   (1000)      147 2023-05-17 14:47:56.000000 theonerig-1.0.1/theonerig.egg-info/requires.txt
--rw-rw-r--   0 tristan   (1000) tristan   (1000)       10 2023-05-17 14:47:56.000000 theonerig-1.0.1/theonerig.egg-info/top_level.txt
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-18 13:01:45.954964 theonerig-1.0.2/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    11357 2023-05-17 08:46:59.000000 theonerig-1.0.2/LICENSE
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     5106 2023-05-18 13:01:45.954964 theonerig-1.0.2/PKG-INFO
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     4445 2023-05-18 13:00:06.000000 theonerig-1.0.2/README.md
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       38 2023-05-18 13:01:45.954964 theonerig-1.0.2/setup.cfg
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     1897 2023-05-17 14:47:00.000000 theonerig-1.0.2/setup.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-18 13:01:45.954964 theonerig-1.0.2/theonerig/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       22 2023-05-18 13:00:26.000000 theonerig-1.0.2/theonerig/__init__.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      814 2023-05-18 13:00:26.000000 theonerig-1.0.2/theonerig/_modidx.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    10718 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/_nbdev.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    27014 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/core.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     5414 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/database.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     6699 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/eyetrack.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    15148 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/leddome.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    20955 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/modelling.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)   110396 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/plotting.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    35828 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/processing.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-18 13:01:45.954964 theonerig-1.0.2/theonerig/synchro/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)        0 2023-05-18 13:00:26.000000 theonerig-1.0.2/theonerig/synchro/__init__.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    11249 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/synchro/extracting.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    61175 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/synchro/io.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    26036 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/synchro/nested_stims.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    23284 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/synchro/processing.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     1903 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/testdata.py
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)    35031 2023-05-17 08:46:59.000000 theonerig-1.0.2/theonerig/utils.py
+drwxrwxr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-18 13:01:45.954964 theonerig-1.0.2/theonerig.egg-info/
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)     5106 2023-05-18 13:01:45.000000 theonerig-1.0.2/theonerig.egg-info/PKG-INFO
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      630 2023-05-18 13:01:45.000000 theonerig-1.0.2/theonerig.egg-info/SOURCES.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)        1 2023-05-18 13:01:45.000000 theonerig-1.0.2/theonerig.egg-info/dependency_links.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)        1 2023-05-17 08:50:04.000000 theonerig-1.0.2/theonerig.egg-info/not-zip-safe
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)      146 2023-05-18 13:01:45.000000 theonerig-1.0.2/theonerig.egg-info/requires.txt
+-rw-rw-r--   0 tristan   (1000) tristan   (1000)       10 2023-05-18 13:01:45.000000 theonerig-1.0.2/theonerig.egg-info/top_level.txt
```

### Comparing `theonerig-1.0.1/LICENSE` & `theonerig-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/PKG-INFO` & `theonerig-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theonerig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Timeseries synchronisation toolkit for computational neuroscience
 Home-page: https://github.com/Tom-TBT/theonerig
 Author: Tom Boissonnet
 Author-email: tom.boissonnet@hotmail.fr
 License: Apache Software License 2.0
 Keywords: neuroscience synchronisation timeserie pipeline
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `theonerig-1.0.1/README.md` & `theonerig-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/setup.py` & `theonerig-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/_modidx.py` & `theonerig-1.0.2/theonerig/_modidx.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/_nbdev.py` & `theonerig-1.0.2/theonerig/_nbdev.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/core.py` & `theonerig-1.0.2/theonerig/core.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/database.py` & `theonerig-1.0.2/theonerig/database.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/eyetrack.py` & `theonerig-1.0.2/theonerig/eyetrack.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/leddome.py` & `theonerig-1.0.2/theonerig/leddome.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/modelling.py` & `theonerig-1.0.2/theonerig/modelling.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/plotting.py` & `theonerig-1.0.2/theonerig/plotting.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/processing.py` & `theonerig-1.0.2/theonerig/processing.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/synchro/extracting.py` & `theonerig-1.0.2/theonerig/synchro/extracting.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/synchro/io.py` & `theonerig-1.0.2/theonerig/synchro/io.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/synchro/nested_stims.py` & `theonerig-1.0.2/theonerig/synchro/nested_stims.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/synchro/processing.py` & `theonerig-1.0.2/theonerig/synchro/processing.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/testdata.py` & `theonerig-1.0.2/theonerig/testdata.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig/utils.py` & `theonerig-1.0.2/theonerig/utils.py`

 * *Files identical despite different names*

### Comparing `theonerig-1.0.1/theonerig.egg-info/PKG-INFO` & `theonerig-1.0.2/theonerig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theonerig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Timeseries synchronisation toolkit for computational neuroscience
 Home-page: https://github.com/Tom-TBT/theonerig
 Author: Tom Boissonnet
 Author-email: tom.boissonnet@hotmail.fr
 License: Apache Software License 2.0
 Keywords: neuroscience synchronisation timeserie pipeline
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `theonerig-1.0.1/theonerig.egg-info/SOURCES.txt` & `theonerig-1.0.2/theonerig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

