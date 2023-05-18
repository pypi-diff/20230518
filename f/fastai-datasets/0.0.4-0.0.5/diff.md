# Comparing `tmp/fastai-datasets-0.0.4.tar.gz` & `tmp/fastai-datasets-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.4.tar", last modified: Sat Apr 29 20:46:54 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.5.tar", last modified: Thu May 18 08:47:32 2023, max compression
```

## Comparing `fastai-datasets-0.0.4.tar` & `fastai-datasets-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.4/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.4/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3894 2023-04-25 14:46:07.000000 fastai-datasets-0.0.4/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-29 20:46:54.345998 fastai-datasets-0.0.4/fastai_datasets/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.4/fastai_datasets/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/cifar10.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/imagenette.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/lfw.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/mnist.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3675 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/pairs.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5767 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/patches.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/pfr.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/fastai_datasets.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-04-29 20:46:54.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-04-29 20:44:50.000000 fastai-datasets-0.0.4/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.4/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.5/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.5/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5493 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3895 2023-05-15 14:03:48.000000 fastai-datasets-0.0.5/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.5/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/cifar10.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3675 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5827 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5493 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-05-18 08:46:47.000000 fastai-datasets-0.0.5/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.5/setup.py
```

### Comparing `fastai-datasets-0.0.4/LICENSE` & `fastai-datasets-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/PKG-INFO` & `fastai-datasets-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.4
+Version: 0.0.5
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
-        # Docs
+        ## Docs
         
         See https://irad-zehavi.github.io/fastai-datasets/
         
         ## Install
         
         ``` sh
         pip install fastai_datasets
```

### Comparing `fastai-datasets-0.0.4/README.md` & `fastai-datasets-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 fastai-datasets
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-# Docs
+## Docs
 
 See https://irad-zehavi.github.io/fastai-datasets/
 
 ## Install
 
 ``` sh
 pip install fastai_datasets
```

### Comparing `fastai-datasets-0.0.4/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.5/fastai_datasets/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets/imagenette.py` & `fastai-datasets-0.0.5/fastai_datasets/imagenette.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets/lfw.py` & `fastai-datasets-0.0.5/fastai_datasets/lfw.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets/mnist.py` & `fastai-datasets-0.0.5/fastai_datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets/pairs.py` & `fastai-datasets-0.0.5/fastai_datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets/patches.py` & `fastai-datasets-0.0.5/fastai_datasets/patches.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,54 +100,52 @@
     if not hasattr(self, '_by_target'):
         targets = [int(t) for t in progress_bar(self.i2t)]
         class_map = groupby(enumerate(targets), key=1, val=0)
         self._by_target = {self.vocab[c]: self.sub_dsets(indices)
                            for c, indices in progress_bar(class_map.items())}
     return self._by_target
 
-
 # %% ../nbs/Core/patches.ipynb 37
 import matplotlib.pyplot as plt
 
 @patch()
 def plot_class_distribution(self: Datasets):
     for split in self.subsets:
         plt.bar(self.vocab, [len(split.by_target[c]) for c in self.vocab])
 
 # %% ../nbs/Core/patches.ipynb 41
 class ListToTuple(Transform):
     """Transforms lists to tuples, useful for fixing a bug in pytorch (pin_memory turns inner tuples into lists)"""
     def encodes(self, o:list):
         return tuple(o)
 
-
 # %% ../nbs/Core/patches.ipynb 42
 dl_defaults = {'pin_memory': default_device() != torch.device('cpu'), 'device': default_device(),
                'after_item': [ToTensor], 'after_batch': [ListToTuple, IntToFloatTensor]}
 
 # %% ../nbs/Core/patches.ipynb 44
-def _dl_args(kwargs):
+def _dl_args(**kwargs):
+    kwargs = deepcopy(kwargs)
     args = deepcopy(dl_defaults)
     for event in ['after_item', 'after_batch']:
         if event in kwargs:
-            tfms = kwargs[event]
+            tfms = kwargs.pop(event)
             args[event] += tfms if isinstance(tfms, Sequence) else [tfms]
+    args.update(kwargs)
     return args
 
-
 @patch
 def dls(self: Datasets, **kwargs) -> DataLoaders:
     """Calls `Datasets.dataloaders` with defaults from `dl_defaults`"""
-    return self.dataloaders(**_dl_args(kwargs))
-
+    return self.dataloaders(**_dl_args(**kwargs))
 
 @patch
 def dl(self: Datasets, **kwargs) -> DataLoader:
     """Creates a `DataLoader` (ignoring splits) with defaults from `dl_defaults`"""
-    return self._dl_type(self, **_dl_args(kwargs))
+    return self._dl_type(self, **_dl_args(**kwargs))
 
 # %% ../nbs/Core/patches.ipynb 46
 @patch
 def load(self: Datasets, **kwargs):
     return first(self.dl(bs=len(self), **kwargs))
 
 # %% ../nbs/Core/patches.ipynb 49
```

### Comparing `fastai-datasets-0.0.4/fastai_datasets/pfr.py` & `fastai-datasets-0.0.5/fastai_datasets/pfr.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets/utils.py` & `fastai-datasets-0.0.5/fastai_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/fastai_datasets.egg-info/PKG-INFO` & `fastai-datasets-0.0.5/fastai_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.4
+Version: 0.0.5
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
-        # Docs
+        ## Docs
         
         See https://irad-zehavi.github.io/fastai-datasets/
         
         ## Install
         
         ``` sh
         pip install fastai_datasets
```

### Comparing `fastai-datasets-0.0.4/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.5/fastai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.4/settings.ini` & `fastai-datasets-0.0.5/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastai-datasets
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastai_datasets
```

### Comparing `fastai-datasets-0.0.4/setup.py` & `fastai-datasets-0.0.5/setup.py`

 * *Files identical despite different names*

