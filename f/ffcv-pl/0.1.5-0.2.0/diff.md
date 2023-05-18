# Comparing `tmp/ffcv_pl-0.1.5.tar.gz` & `tmp/ffcv_pl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffcv_pl-0.1.5.tar", last modified: Tue Mar 21 09:41:26 2023, max compression
+gzip compressed data, was "ffcv_pl-0.2.0.tar", last modified: Thu May 18 07:37:39 2023, max compression
```

## Comparing `ffcv_pl-0.1.5.tar` & `ffcv_pl-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     5960 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/PKG-INFO
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/ffcv_pl/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.1.5/ffcv_pl/__init__.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/ffcv_pl/datasets/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.1.5/ffcv_pl/datasets/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     3200 2023-01-24 12:03:42.000000 ffcv_pl-0.1.5/ffcv_pl/datasets/image.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     4481 2023-03-21 09:03:08.000000 ffcv_pl-0.1.5/ffcv_pl/datasets/image_array.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     3909 2023-02-07 07:36:50.000000 ffcv_pl-0.1.5/ffcv_pl/datasets/image_label.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/ffcv_pl/ffcv_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.1.5/ffcv_pl/ffcv_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.1.5/ffcv_pl/ffcv_utils/custom_augmentations.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     4545 2023-03-21 09:12:40.000000 ffcv_pl-0.1.5/ffcv_pl/ffcv_utils/generate_dataset.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/ffcv_pl.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     5960 2023-03-21 09:41:26.000000 ffcv_pl-0.1.5/ffcv_pl.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      414 2023-03-21 09:41:26.000000 ffcv_pl-0.1.5/ffcv_pl.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-03-21 09:41:26.000000 ffcv_pl-0.1.5/ffcv_pl.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-03-10 09:34:56.000000 ffcv_pl-0.1.5/ffcv_pl.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-03-21 09:41:26.000000 ffcv_pl-0.1.5/ffcv_pl.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-03-21 09:41:26.358924 ffcv_pl-0.1.5/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      518 2023-03-21 09:39:47.000000 ffcv_pl-0.1.5/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:37:39.460096 ffcv_pl-0.2.0/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     4749 2023-05-18 07:37:39.460096 ffcv_pl-0.2.0/PKG-INFO
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:37:39.460096 ffcv_pl-0.2.0/ffcv_pl/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.2.0/ffcv_pl/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    11040 2023-05-17 14:35:34.000000 ffcv_pl-0.2.0/ffcv_pl/data_loading.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:37:39.460096 ffcv_pl-0.2.0/ffcv_pl/ffcv_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.2.0/ffcv_pl/ffcv_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.2.0/ffcv_pl/ffcv_utils/augmentations.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      935 2023-05-17 14:39:06.000000 ffcv_pl-0.2.0/ffcv_pl/ffcv_utils/decoders.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      446 2023-05-10 14:49:01.000000 ffcv_pl-0.2.0/ffcv_pl/ffcv_utils/utils.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     2304 2023-05-17 12:45:28.000000 ffcv_pl-0.2.0/ffcv_pl/generate_dataset.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:37:39.460096 ffcv_pl-0.2.0/ffcv_pl.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     4749 2023-05-18 07:37:39.000000 ffcv_pl-0.2.0/ffcv_pl.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      360 2023-05-18 07:37:39.000000 ffcv_pl-0.2.0/ffcv_pl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-05-18 07:37:39.000000 ffcv_pl-0.2.0/ffcv_pl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-03-10 09:34:56.000000 ffcv_pl-0.2.0/ffcv_pl.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-05-18 07:37:39.000000 ffcv_pl-0.2.0/ffcv_pl.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-05-18 07:37:39.460096 ffcv_pl-0.2.0/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      518 2023-05-18 07:24:57.000000 ffcv_pl-0.2.0/setup.py
```

### Comparing `ffcv_pl-0.1.5/ffcv_pl/ffcv_utils/custom_augmentations.py` & `ffcv_pl-0.2.0/ffcv_pl/ffcv_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.1.5/setup.py` & `ffcv_pl-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 # set readme
 this_directory = Path(__file__).parent
 long_description = (this_directory / "../readme.md").read_text()
 
 setup(name='ffcv_pl',
-      version='0.1.5',
+      version='0.2.0',
       description='manage fast data loading with ffcv and pytorch lightning',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/SerezD/ffcv_pytorch_lightning',
       author='DSerez',
       license='MIT',
       zip_safe=False)
```

