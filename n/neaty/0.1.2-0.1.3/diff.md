# Comparing `tmp/neaty-0.1.2.tar.gz` & `tmp/neaty-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neaty-0.1.2.tar", last modified: Tue Mar  7 15:23:55 2023, max compression
+gzip compressed data, was "neaty-0.1.3.tar", last modified: Thu May 18 17:00:47 2023, max compression
```

## Comparing `neaty-0.1.2.tar` & `neaty-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:23:55.065354 neaty-0.1.2/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      604 2023-03-07 15:23:55.065354 neaty-0.1.2/PKG-INFO
--rw-r--r--   0 netvor    (9860) netvor    (9860)    11957 2023-03-07 15:23:54.781349 neaty-0.1.2/setup.py
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:23:55.065354 neaty-0.1.2/src/
-drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:23:55.065354 neaty-0.1.2/src/neaty/
--rw-r--r--   0 netvor    (9860) netvor    (9860)      993 2023-03-07 15:22:03.019259 neaty-0.1.2/src/neaty/__init__.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)      530 2023-03-07 15:23:53.729329 neaty-0.1.2/src/neaty/_meta.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     2588 2023-03-07 15:22:03.019259 neaty-0.1.2/src/neaty/log.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)     7745 2023-03-07 15:22:07.311339 neaty-0.1.2/src/neaty/neaty.py
--rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:22:03.019259 neaty-0.1.2/src/neaty/py.typed
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-05-18 17:00:47.977938 neaty-0.1.3/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      604 2023-05-18 17:00:47.977938 neaty-0.1.3/PKG-INFO
+-rw-r--r--   0 netvor    (9860) netvor    (9860)    11957 2023-05-18 17:00:47.821933 neaty-0.1.3/setup.py
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-05-18 17:00:47.977938 neaty-0.1.3/src/
+drwxr-xr-x   0 netvor    (9860) netvor    (9860)        0 2023-05-18 17:00:47.977938 neaty-0.1.3/src/neaty/
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      993 2023-03-07 15:22:03.019259 neaty-0.1.3/src/neaty/__init__.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)      530 2023-05-18 17:00:47.077908 neaty-0.1.3/src/neaty/_meta.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     2588 2023-03-07 15:22:03.019259 neaty-0.1.3/src/neaty/log.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)     7628 2023-05-18 15:00:46.615036 neaty-0.1.3/src/neaty/neaty.py
+-rw-r--r--   0 netvor    (9860) netvor    (9860)        0 2023-03-07 15:22:03.019259 neaty-0.1.3/src/neaty/py.typed
```

### Comparing `neaty-0.1.2/PKG-INFO` & `neaty-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: neaty
-Version: 0.1.2
+Version: 0.1.3
 Summary: neaty - Neaty logger
 Home-page: https://gitlab.com/vornet/python/python-neaty
 Author: UNKNOWN
 Author-email: Alois Mahdal <netvor+neaty@vornet.cz>
 License: LGPLv2
 Description: Neaty logger
 Platform: UNKNOWN
```

### Comparing `neaty-0.1.2/setup.py` & `neaty-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,12 +344,12 @@
     maintainer_email='Alois Mahdal <netvor+neaty@vornet.cz>',
     name='neaty',
     packages=vdk_packageinfo()['packages'],
     package_dir=vdk_packageinfo()['package_dir'],
     package_data=vdk_packageinfo()['package_data'],
     url='https://gitlab.com/vornet/python/python-neaty',
     requires=vdk_cleanup(VDK_PYLIB_REQUIRES_PYSTUFF),
-    version='0.1.2',
+    version='0.1.3',
     classifiers=vdk_packageinfo()['classifiers'],
 )
 
-# setup.py built with MKit 0.0.60 and vdk-pylib-0.0.29
+# setup.py built with MKit 0.0.60 and vdk-pylib-0.0.31
```

### Comparing `neaty-0.1.2/src/neaty/__init__.py` & `neaty-0.1.3/src/neaty/__init__.py`

 * *Files identical despite different names*

### Comparing `neaty-0.1.2/src/neaty/_meta.py` & `neaty-0.1.3/src/neaty/_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CODENAME: str = """
 
 """.strip()
 
 GIT_LASTHASH: str = """
-90ca604a3d681db1068cb3de71de888933fef43b
+52283d543c687ff829df4f67d811682336e43ce9
 """.strip()
 
 GIT_LASTSUMMARY: str = """
-Bump version to 0.1.2
+Bump version to 0.1.3
 """.strip()
 
 LICENSE: str = """
 LGPLv2
 """.strip()
 
 MAINTAINER: str = """
@@ -31,9 +31,9 @@
 """.strip()
 
 VCS_BROWSER: str = """
 https://gitlab.com/vornet/python/python-neaty
 """.strip()
 
 VERSION: str = """
-0.1.2
+0.1.3
 """.strip()
```

### Comparing `neaty-0.1.2/src/neaty/log.py` & `neaty-0.1.3/src/neaty/log.py`

 * *Files identical despite different names*

### Comparing `neaty-0.1.2/src/neaty/neaty.py` & `neaty-0.1.3/src/neaty/neaty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python3
-
 import sys
 import inspect
 
 
 class _LoggerMode:
 
     def __init__(self, verbose, debug):
@@ -59,26 +57,22 @@
 
         def is_pubapi(f):
             return f[3] in self._pubapi
 
         def is_us(f):
             return f[3] == '_stackfix'
 
-        def is_script(f):
-            return f[3] == '<module>'
-
         frames = inspect.stack()
         focus = frames.pop(0)
         assert is_us(focus)
         focus = frames.pop(0)
         assert is_printers(focus)
         focus = frames.pop(0)
         assert is_pubapi(focus)
         focus = frames.pop()
-        assert is_script(focus)
 
         def fnname(F):
             return F[3] + '():'
 
         if len(frames) == 0:
             prefix = focus[1].split('/')[-1] + ':'
         elif len(frames) < 3:
```

