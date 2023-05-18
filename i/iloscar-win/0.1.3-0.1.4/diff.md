# Comparing `tmp/iloscar_win-0.1.3.tar.gz` & `tmp/iloscar_win-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar_win-0.1.3.tar", last modified: Thu May 18 17:17:18 2023, max compression
+gzip compressed data, was "iloscar_win-0.1.4.tar", last modified: Thu May 18 17:20:35 2023, max compression
```

## Comparing `iloscar_win-0.1.3.tar` & `iloscar_win-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:17:18.208684 iloscar_win-0.1.3/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:17:18.207686 iloscar_win-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:17:18.127421 iloscar_win-0.1.3/iloscar_win/
--rw-rw-rw-   0        0        0      350 2023-05-18 17:16:18.000000 iloscar_win-0.1.3/iloscar_win/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-05-18 17:00:12.000000 iloscar_win-0.1.3/iloscar_win/app.py
--rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar_win-0.1.3/iloscar_win/iLOSCAR_backend.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:17:18.203697 iloscar_win-0.1.3/iloscar_win/pages/
--rw-rw-rw-   0        0        0     5797 2023-05-18 17:01:06.000000 iloscar_win-0.1.3/iloscar_win/pages/Function.py
--rw-rw-rw-   0        0        0    26245 2023-05-18 17:00:56.000000 iloscar_win-0.1.3/iloscar_win/pages/forward.py
--rw-rw-rw-   0        0        0      887 2023-05-18 17:01:55.000000 iloscar_win-0.1.3/iloscar_win/pages/home.py
--rw-rw-rw-   0        0        0    46215 2023-05-18 17:01:22.000000 iloscar_win-0.1.3/iloscar_win/pages/inverse.py
--rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.3/iloscar_win/style.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:17:18.190131 iloscar_win-0.1.3/iloscar_win.egg-info/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:17:17.000000 iloscar_win-0.1.3/iloscar_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-05-18 17:17:17.000000 iloscar_win-0.1.3/iloscar_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:17:17.000000 iloscar_win-0.1.3/iloscar_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-05-18 17:17:17.000000 iloscar_win-0.1.3/iloscar_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-05-18 17:17:17.000000 iloscar_win-0.1.3/iloscar_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 17:17:18.209686 iloscar_win-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1509 2023-05-18 17:17:15.000000 iloscar_win-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.100375 iloscar_win-0.1.4/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:20:35.097381 iloscar_win-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.035607 iloscar_win-0.1.4/iloscar_win/
+-rw-rw-rw-   0        0        0      350 2023-05-18 17:19:34.000000 iloscar_win-0.1.4/iloscar_win/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-05-18 17:00:12.000000 iloscar_win-0.1.4/iloscar_win/app.py
+-rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar_win-0.1.4/iloscar_win/iLOSCAR_backend.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.091884 iloscar_win-0.1.4/iloscar_win/pages/
+-rw-rw-rw-   0        0        0     5797 2023-05-18 17:01:06.000000 iloscar_win-0.1.4/iloscar_win/pages/Function.py
+-rw-rw-rw-   0        0        0    26245 2023-05-18 17:00:56.000000 iloscar_win-0.1.4/iloscar_win/pages/forward.py
+-rw-rw-rw-   0        0        0      887 2023-05-18 17:01:55.000000 iloscar_win-0.1.4/iloscar_win/pages/home.py
+-rw-rw-rw-   0        0        0    46215 2023-05-18 17:01:22.000000 iloscar_win-0.1.4/iloscar_win/pages/inverse.py
+-rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.4/iloscar_win/style.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:20:35.080547 iloscar_win-0.1.4/iloscar_win.egg-info/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-05-18 17:20:34.000000 iloscar_win-0.1.4/iloscar_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:20:35.100375 iloscar_win-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1509 2023-05-18 17:19:47.000000 iloscar_win-0.1.4/setup.py
```

### Comparing `iloscar_win-0.1.3/PKG-INFO` & `iloscar_win-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar_win
-Version: 0.1.3
+Version: 0.1.4
 Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar_win-0.1.3/README.md` & `iloscar_win-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/app.py` & `iloscar_win-0.1.4/iloscar_win/app.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/iLOSCAR_backend.py` & `iloscar_win-0.1.4/iloscar_win/iLOSCAR_backend.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/pages/Function.py` & `iloscar_win-0.1.4/iloscar_win/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/pages/forward.py` & `iloscar_win-0.1.4/iloscar_win/pages/forward.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/pages/home.py` & `iloscar_win-0.1.4/iloscar_win/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/pages/inverse.py` & `iloscar_win-0.1.4/iloscar_win/pages/inverse.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win/style.py` & `iloscar_win-0.1.4/iloscar_win/style.py`

 * *Files identical despite different names*

### Comparing `iloscar_win-0.1.3/iloscar_win.egg-info/PKG-INFO` & `iloscar_win-0.1.4/iloscar_win.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar-win
-Version: 0.1.3
+Version: 0.1.4
 Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar_win-0.1.3/setup.py` & `iloscar_win-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'iLOSCAR_win'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar_win",
     version=VERSION,
```

