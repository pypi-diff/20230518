# Comparing `tmp/iloscar-win-0.1.1.tar.gz` & `tmp/iloscar_win-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar-win-0.1.1.tar", last modified: Thu May 18 17:02:15 2023, max compression
+gzip compressed data, was "iloscar_win-0.1.2.tar", last modified: Thu May 18 17:07:07 2023, max compression
```

## Comparing `iloscar-win-0.1.1.tar` & `iloscar_win-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.407099 iloscar-win-0.1.1/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:02:15.404554 iloscar-win-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar-win-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.346659 iloscar-win-0.1.1/iloscar/
--rw-rw-rw-   0        0        0      349 2023-05-18 16:58:34.000000 iloscar-win-0.1.1/iloscar/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-05-18 17:00:12.000000 iloscar-win-0.1.1/iloscar/app.py
--rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar-win-0.1.1/iloscar/iLOSCAR_backend.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.354953 iloscar-win-0.1.1/iloscar/pages/
--rw-rw-rw-   0        0        0     5797 2023-05-18 17:01:06.000000 iloscar-win-0.1.1/iloscar/pages/Function.py
--rw-rw-rw-   0        0        0    26245 2023-05-18 17:00:56.000000 iloscar-win-0.1.1/iloscar/pages/forward.py
--rw-rw-rw-   0        0        0      887 2023-05-18 17:01:55.000000 iloscar-win-0.1.1/iloscar/pages/home.py
--rw-rw-rw-   0        0        0    46215 2023-05-18 17:01:22.000000 iloscar-win-0.1.1/iloscar/pages/inverse.py
--rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar-win-0.1.1/iloscar/style.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:02:15.399333 iloscar-win-0.1.1/iloscar_win.egg-info/
--rw-rw-rw-   0        0        0    18548 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-18 17:02:15.000000 iloscar-win-0.1.1/iloscar_win.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 17:02:15.407099 iloscar-win-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-05-18 17:01:51.000000 iloscar-win-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:07:07.974215 iloscar_win-0.1.2/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:07:07.970205 iloscar_win-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17783 2023-05-18 16:23:09.000000 iloscar_win-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:07:07.881899 iloscar_win-0.1.2/iloscar/
+-rw-rw-rw-   0        0        0      349 2023-05-18 16:58:34.000000 iloscar_win-0.1.2/iloscar/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-05-18 17:00:12.000000 iloscar_win-0.1.2/iloscar/app.py
+-rw-rw-rw-   0        0        0   106422 2023-05-18 16:23:10.000000 iloscar_win-0.1.2/iloscar/iLOSCAR_backend.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:07:07.903686 iloscar_win-0.1.2/iloscar/pages/
+-rw-rw-rw-   0        0        0     5797 2023-05-18 17:01:06.000000 iloscar_win-0.1.2/iloscar/pages/Function.py
+-rw-rw-rw-   0        0        0    26245 2023-05-18 17:00:56.000000 iloscar_win-0.1.2/iloscar/pages/forward.py
+-rw-rw-rw-   0        0        0      887 2023-05-18 17:01:55.000000 iloscar_win-0.1.2/iloscar/pages/home.py
+-rw-rw-rw-   0        0        0    46215 2023-05-18 17:01:22.000000 iloscar_win-0.1.2/iloscar/pages/inverse.py
+-rw-rw-rw-   0        0        0     1357 2023-05-18 16:23:10.000000 iloscar_win-0.1.2/iloscar/style.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:07:07.964139 iloscar_win-0.1.2/iloscar_win.egg-info/
+-rw-rw-rw-   0        0        0    18548 2023-05-18 17:07:07.000000 iloscar_win-0.1.2/iloscar_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-18 17:07:07.000000 iloscar_win-0.1.2/iloscar_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:07:07.000000 iloscar_win-0.1.2/iloscar_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-05-18 17:07:07.000000 iloscar_win-0.1.2/iloscar_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-18 17:07:07.000000 iloscar_win-0.1.2/iloscar_win.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:07:07.975218 iloscar_win-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-05-18 17:06:25.000000 iloscar_win-0.1.2/setup.py
```

### Comparing `iloscar-win-0.1.1/PKG-INFO` & `iloscar_win-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: iloscar-win
-Version: 0.1.1
-Summary: iLOSCAR-win
+Name: iloscar_win
+Version: 0.1.2
+Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `iloscar-win-0.1.1/README.md` & `iloscar_win-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/app.py` & `iloscar_win-0.1.2/iloscar/app.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/iLOSCAR_backend.py` & `iloscar_win-0.1.2/iloscar/iLOSCAR_backend.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/pages/Function.py` & `iloscar_win-0.1.2/iloscar/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/pages/forward.py` & `iloscar_win-0.1.2/iloscar/pages/forward.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/pages/home.py` & `iloscar_win-0.1.2/iloscar/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/pages/inverse.py` & `iloscar_win-0.1.2/iloscar/pages/inverse.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar/style.py` & `iloscar_win-0.1.2/iloscar/style.py`

 * *Files identical despite different names*

### Comparing `iloscar-win-0.1.1/iloscar_win.egg-info/PKG-INFO` & `iloscar_win-0.1.2/iloscar_win.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iloscar-win
-Version: 0.1.1
-Summary: iLOSCAR-win
+Version: 0.1.2
+Summary: iLOSCAR_win
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `iloscar-win-0.1.1/setup.py` & `iloscar_win-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
-DESCRIPTION = 'iLOSCAR-win'
+VERSION = '0.1.2'
+DESCRIPTION = 'iLOSCAR_win'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
-    name="iloscar-win",
+    name="iloscar_win",
     version=VERSION,
     url = 'https://github.com/Shihan150/iloscar',
     license = 'MIT',
     author="Shihan Li",
     author_email="<shihan@tamu.edu>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

