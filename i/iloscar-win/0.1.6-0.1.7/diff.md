# Comparing `tmp/iloscar_win-0.1.6.tar.gz` & `tmp/iloscar_win-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar_win-0.1.6.tar", last modified: Thu May 18 17:27:36 2023, max compression
+gzip compressed data, was "iloscar_win-0.1.7.tar", last modified: Thu May 18 17:32:41 2023, max compression
```

## Comparing `iloscar_win-0.1.6.tar` & `iloscar_win-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:27:36.391480 iloscar_win-0.1.6/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:27:36.389477 iloscar_win-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:27:36.327999 iloscar_win-0.1.6/iloscar_win/
--rw-rw-rw-   0        0        0      354 2023-05-18 17:27:06.000000 iloscar_win-0.1.6/iloscar_win/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-05-18 17:22:58.000000 iloscar_win-0.1.6/iloscar_win/app.py
--rw-rw-rw-   0        0        0   106434 2023-05-18 17:23:19.000000 iloscar_win-0.1.6/iloscar_win/iLOSCAR_backend.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:27:36.380520 iloscar_win-0.1.6/iloscar_win/pages/
--rw-rw-rw-   0        0        0     5801 2023-05-18 17:23:48.000000 iloscar_win-0.1.6/iloscar_win/pages/Function.py
--rw-rw-rw-   0        0        0    26253 2023-05-18 17:23:44.000000 iloscar_win-0.1.6/iloscar_win/pages/forward.py
--rw-rw-rw-   0        0        0      891 2023-05-18 17:23:53.000000 iloscar_win-0.1.6/iloscar_win/pages/home.py
--rw-rw-rw-   0        0        0    46223 2023-05-18 17:24:04.000000 iloscar_win-0.1.6/iloscar_win/pages/inverse.py
--rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.6/iloscar_win/style.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:27:36.365677 iloscar_win-0.1.6/iloscar_win.egg-info/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:27:36.000000 iloscar_win-0.1.6/iloscar_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-05-18 17:27:36.000000 iloscar_win-0.1.6/iloscar_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:27:36.000000 iloscar_win-0.1.6/iloscar_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-05-18 17:27:36.000000 iloscar_win-0.1.6/iloscar_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 17:27:36.000000 iloscar_win-0.1.6/iloscar_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 17:27:36.391480 iloscar_win-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1509 2023-05-18 17:27:12.000000 iloscar_win-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:32:41.239483 iloscar_win-0.1.7/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:32:41.239483 iloscar_win-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:32:41.160397 iloscar_win-0.1.7/iloscar_win/
+-rw-rw-rw-   0        0        0      354 2023-05-18 17:27:06.000000 iloscar_win-0.1.7/iloscar_win/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-18 17:22:58.000000 iloscar_win-0.1.7/iloscar_win/app.py
+-rw-rw-rw-   0        0        0   106434 2023-05-18 17:23:19.000000 iloscar_win-0.1.7/iloscar_win/iLOSCAR_backend.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:32:41.232458 iloscar_win-0.1.7/iloscar_win/pages/
+-rw-rw-rw-   0        0        0     5801 2023-05-18 17:23:48.000000 iloscar_win-0.1.7/iloscar_win/pages/Function.py
+-rw-rw-rw-   0        0        0    26253 2023-05-18 17:23:44.000000 iloscar_win-0.1.7/iloscar_win/pages/forward.py
+-rw-rw-rw-   0        0        0      891 2023-05-18 17:23:53.000000 iloscar_win-0.1.7/iloscar_win/pages/home.py
+-rw-rw-rw-   0        0        0    46223 2023-05-18 17:24:04.000000 iloscar_win-0.1.7/iloscar_win/pages/inverse.py
+-rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.7/iloscar_win/style.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:32:41.222342 iloscar_win-0.1.7/iloscar_win.egg-info/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:32:40.000000 iloscar_win-0.1.7/iloscar_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-05-18 17:32:41.000000 iloscar_win-0.1.7/iloscar_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:32:40.000000 iloscar_win-0.1.7/iloscar_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-05-18 17:32:40.000000 iloscar_win-0.1.7/iloscar_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 17:32:40.000000 iloscar_win-0.1.7/iloscar_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:32:41.240656 iloscar_win-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1513 2023-05-18 17:32:26.000000 iloscar_win-0.1.7/setup.py
```

### Comparing `iloscar_win-0.1.6/PKG-INFO` & `iloscar_win-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar_win
-Version: 0.1.6
+Version: 0.1.7
 Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar_win-0.1.6/README.md` & `iloscar_win-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/app.py` & `iloscar_win-0.1.7/iloscar_win/app.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/iLOSCAR_backend.py` & `iloscar_win-0.1.7/iloscar_win/iLOSCAR_backend.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/pages/Function.py` & `iloscar_win-0.1.7/iloscar_win/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/pages/forward.py` & `iloscar_win-0.1.7/iloscar_win/pages/forward.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/pages/home.py` & `iloscar_win-0.1.7/iloscar_win/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/pages/inverse.py` & `iloscar_win-0.1.7/iloscar_win/pages/inverse.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win/style.py` & `iloscar_win-0.1.7/iloscar_win/style.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.6/iloscar_win.egg-info/PKG-INFO` & `iloscar_win-0.1.7/iloscar_win.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar-win
-Version: 0.1.6
+Version: 0.1.7
 Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar_win-0.1.6/setup.py` & `iloscar_win-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'iLOSCAR_win'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar_win",
     version=VERSION,
@@ -32,12 +32,12 @@
         # "Operating System :: Unix",
         # "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 
     include_package_data = True,
     package_data = {
-    'iloscar': ['dat_y0/*.dat']
+    'iloscar_win': ['dat_y0/*.dat']
     },
     python_requires='>3.7, <3.11'
 
 )
```

