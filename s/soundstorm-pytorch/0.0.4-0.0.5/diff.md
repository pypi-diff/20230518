# Comparing `tmp/soundstorm-pytorch-0.0.4.tar.gz` & `tmp/soundstorm-pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundstorm-pytorch-0.0.4.tar", last modified: Wed May 17 21:10:58 2023, max compression
+gzip compressed data, was "soundstorm-pytorch-0.0.5.tar", last modified: Thu May 18 17:16:54 2023, max compression
```

## Comparing `soundstorm-pytorch-0.0.4.tar` & `soundstorm-pytorch-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:10:58.052738 soundstorm-pytorch-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 21:10:43.000000 soundstorm-pytorch-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 21:10:58.052738 soundstorm-pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-17 21:10:43.000000 soundstorm-pytorch-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:10:58.052738 soundstorm-pytorch-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-17 21:10:43.000000 soundstorm-pytorch-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:10:58.052738 soundstorm-pytorch-0.0.4/soundstorm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-17 21:10:43.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-17 21:10:43.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-17 21:10:43.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch/soundstorm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:10:58.052738 soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 21:10:58.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-17 21:10:58.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:10:58.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 21:10:58.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 21:10:58.000000 soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/soundstorm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-18 17:16:37.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch/soundstorm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:16:54.503322 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 17:16:54.000000 soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/top_level.txt
```

### Comparing `soundstorm-pytorch-0.0.4/LICENSE` & `soundstorm-pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.4/PKG-INFO` & `soundstorm-pytorch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `soundstorm-pytorch-0.0.4/setup.py` & `soundstorm-pytorch-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'soundstorm-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/soundstorm-pytorch',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'transformers',
     'attention mechanism',
     'audio generation'
   ],
   install_requires=[
+    'accelerate',
     'audiolm-pytorch>=1.0.0',
     'beartype',
     'conformer>=0.3.2',
     'einops>=0.6.1',
     'torch>=1.6',
   ],
   classifiers=[
```

### Comparing `soundstorm-pytorch-0.0.4/soundstorm_pytorch/attend.py` & `soundstorm-pytorch-0.0.5/soundstorm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `soundstorm-pytorch-0.0.4/soundstorm_pytorch.egg-info/PKG-INFO` & `soundstorm-pytorch-0.0.5/soundstorm_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soundstorm-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: SoundStorm - Efficient Parallel Audio Generation from Google Deepmind, in Pytorch
 Home-page: https://github.com/lucidrains/soundstorm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

