# Comparing `tmp/trivial_torch_tools-0.5.0.tar.gz` & `tmp/trivial_torch_tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trivial_torch_tools-0.5.0.tar", last modified: Mon Apr 11 14:55:48 2022, max compression
+gzip compressed data, was "dist/trivial_torch_tools-0.5.1.tar", last modified: Sun Apr 17 20:25:59 2022, max compression
```

## Comparing `trivial_torch_tools-0.5.0.tar` & `trivial_torch_tools-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-04-11 14:55:48.751871 trivial_torch_tools-0.5.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3554 2022-04-11 14:55:48.751253 trivial_torch_tools-0.5.0/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-04-11 14:55:48.752031 trivial_torch_tools-0.5.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1216 2022-04-11 14:53:44.000000 trivial_torch_tools-0.5.0/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-04-11 14:55:48.739689 trivial_torch_tools-0.5.0/trivial_torch_tools/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-03-02 13:43:36.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4740 2022-03-12 00:41:27.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/core.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8851 2022-04-11 14:53:05.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/generics.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1328 2022-03-04 13:18:09.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/image.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1014 2022-03-12 00:41:39.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/main.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1958 2022-03-28 17:43:25.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/misc.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8943 2022-04-11 14:52:32.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/model.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1765 2022-03-04 16:30:04.000000 trivial_torch_tools-0.5.0/trivial_torch_tools/one_hots.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-04-11 14:55:48.749140 trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3554 2022-04-11 14:55:48.000000 trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      460 2022-04-11 14:55:48.000000 trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-04-11 14:55:48.000000 trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       65 2022-04-11 14:55:48.000000 trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       20 2022-04-11 14:55:48.000000 trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/top_level.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-04-17 20:25:59.629049 trivial_torch_tools-0.5.1/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3554 2022-04-17 20:25:59.627968 trivial_torch_tools-0.5.1/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-04-17 20:25:59.631014 trivial_torch_tools-0.5.1/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1216 2022-04-11 14:53:44.000000 trivial_torch_tools-0.5.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-04-17 20:25:59.620200 trivial_torch_tools-0.5.1/trivial_torch_tools/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-03-02 13:43:36.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4740 2022-03-12 00:41:27.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/core.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8851 2022-04-11 14:53:05.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/generics.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1328 2022-03-04 13:18:09.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/image.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1014 2022-03-12 00:41:39.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/main.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1958 2022-03-28 17:43:25.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/misc.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8964 2022-04-17 20:21:53.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/model.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1765 2022-03-04 16:30:04.000000 trivial_torch_tools-0.5.1/trivial_torch_tools/one_hots.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-04-17 20:25:59.625328 trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3554 2022-04-17 20:25:58.000000 trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      460 2022-04-17 20:25:58.000000 trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-04-17 20:25:58.000000 trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       65 2022-04-17 20:25:58.000000 trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       20 2022-04-17 20:25:58.000000 trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/top_level.txt
```

### Comparing `trivial_torch_tools-0.5.0/PKG-INFO` & `trivial_torch_tools-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivial_torch_tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Decorators for reducing pytorch boilerplate
 Home-page: https://github.com/jeff-hykin/trivial-torch-tools.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Description: # What is this?
```

### Comparing `trivial_torch_tools-0.5.0/setup.py` & `trivial_torch_tools-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/core.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/core.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/generics.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/generics.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/image.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/image.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/main.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/main.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/misc.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/misc.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/model.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             # attach method
             self.forward = forward
             
             # call original __init__()
             return function_being_wrapped(self, *args, **kwargs)
         return wrapper
     
-    def save_and_load_methods(basic_attributes, model_attributes, path_attribute="path"):
+    def save_and_load_methods(basic_attributes, model_attributes=[], path_attribute="path"):
         def wrapper1(function_being_wrapped):
             # wrapper2 will be the new __init__()
             def wrapper2(self, *args, **kwargs):
                 # create methods
                 def save(path=None):
                     model_data = tuple(getattr(self, each_attribute).state_dict() for each_attribute in model_attributes)
                     normal_data = tuple(getattr(self, each_attribute)               for each_attribute in basic_attributes)
@@ -101,20 +101,20 @@
                 
                 def unfreeze():
                     for child in self.children():
                         for param in child.parameters():
                             param.requires_grad = True
                 
                 class WithObj(object):
-                    def __init__(*args, **kwargs):
+                    def __init__(self_, *args, **kwargs):
                         pass
-                    def __enter__(_):
+                    def __enter__(self_, *_):
                         self.freeze()
                         return self
-                    def __exit__(_, __, error, traceback):
+                    def __exit__(self_, _, error, traceback):
                         self.unfreeze()
                         # normal cleanup HERE
                         if error is not None:
                             # error cleanup HERE
                             raise error
                 # attach methods
                 self.freeze = freeze
```

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools/one_hots.py` & `trivial_torch_tools-0.5.1/trivial_torch_tools/one_hots.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.5.0/trivial_torch_tools.egg-info/PKG-INFO` & `trivial_torch_tools-0.5.1/trivial_torch_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trivial-torch-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Decorators for reducing pytorch boilerplate
 Home-page: https://github.com/jeff-hykin/trivial-torch-tools.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Description: # What is this?
```

