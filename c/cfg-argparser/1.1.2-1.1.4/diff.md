# Comparing `tmp/cfg-argparser-1.1.2.tar.gz` & `tmp/cfg-argparser-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.1.2.tar", last modified: Mon May  8 12:49:06 2023, max compression
+gzip compressed data, was "cfg-argparser-1.1.4.tar", last modified: Thu May 18 03:01:32 2023, max compression
```

## Comparing `cfg-argparser-1.1.2.tar` & `cfg-argparser-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-08 12:49:06.542828 cfg-argparser-1.1.2/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.2/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-08 12:49:06.542828 cfg-argparser-1.1.2/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-05-02 16:31:49.000000 cfg-argparser-1.1.2/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-05-08 12:48:12.000000 cfg-argparser-1.1.2/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-08 12:49:06.542828 cfg-argparser-1.1.2/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-08 12:49:06.542828 cfg-argparser-1.1.2/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-08 12:49:06.542828 cfg-argparser-1.1.2/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.1.2/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    12166 2023-05-06 16:19:13.000000 cfg-argparser-1.1.2/src/cfg_argparser/config_arg_parser.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-08 12:49:06.542828 cfg-argparser-1.1.2/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-08 12:49:06.000000 cfg-argparser-1.1.2/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-05-08 12:49:06.000000 cfg-argparser-1.1.2/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-08 12:49:06.000000 cfg-argparser-1.1.2/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-08 12:49:06.000000 cfg-argparser-1.1.2/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 03:01:32.504961 cfg-argparser-1.1.4/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.4/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-18 03:01:32.504961 cfg-argparser-1.1.4/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-05-18 03:01:07.000000 cfg-argparser-1.1.4/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-05-18 03:01:17.000000 cfg-argparser-1.1.4/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-18 03:01:32.504961 cfg-argparser-1.1.4/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 03:01:32.501628 cfg-argparser-1.1.4/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 03:01:32.504961 cfg-argparser-1.1.4/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.1.4/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    12217 2023-05-16 06:00:18.000000 cfg-argparser-1.1.4/src/cfg_argparser/config_arg_parser.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-18 03:01:32.504961 cfg-argparser-1.1.4/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-18 03:01:32.000000 cfg-argparser-1.1.4/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-05-18 03:01:32.000000 cfg-argparser-1.1.4/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-18 03:01:32.000000 cfg-argparser-1.1.4/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-18 03:01:32.000000 cfg-argparser-1.1.4/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.1.2/LICENSE` & `cfg-argparser-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.1.2/PKG-INFO` & `cfg-argparser-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.2
+Version: 1.1.4
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cfg_argparser 1.1.1
+# cfg_argparser 1.1.4
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-argparser-1.1.2/README.md` & `cfg-argparser-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cfg_argparser 1.1.1
+# cfg_argparser 1.1.4
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-argparser-1.1.2/pyproject.toml` & `cfg-argparser-1.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-argparser"
-version = "1.1.2"
+version = "1.1.4"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify configurable defaults from argparse."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `cfg-argparser-1.1.2/src/cfg_argparser/config_arg_parser.py` & `cfg-argparser-1.1.4/src/cfg_argparser/config_arg_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 class CfgDict(dict):
     """
     A subclass of `dict` with some useful changes, most notably 
     storing a path to save, and saving methods
     """
 
-    def __init__(self, cfg_path, config: dict = {}, save_on_change: bool = False, sort_on_save: bool = False):
+    def __init__(self, cfg_path, config: dict = {}, save_on_change: bool = False, sort_on_save: bool = False, start_empty=False):
         super().__init__()
         self.cfg_path = cfg_path
         self.save_on_change = False
         self.update(config)
         self.save_on_change = save_on_change
         self.sort_on_save = sort_on_save
-        self.load()
+        if not start_empty:
+            self.load()
 
     def set_path(self, path):
         self.cfg_path = path
         return self
 
     def save(self, out_dict=None, indent=4):
         if not isinstance(out_dict, dict):
```

### Comparing `cfg-argparser-1.1.2/src/cfg_argparser.egg-info/PKG-INFO` & `cfg-argparser-1.1.4/src/cfg_argparser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.2
+Version: 1.1.4
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cfg_argparser 1.1.1
+# cfg_argparser 1.1.4
 
 a config wrapper I made to be easily applied to argparse objects.
 
 ## Installation
 
 ```bash
 # from pypi:
```

