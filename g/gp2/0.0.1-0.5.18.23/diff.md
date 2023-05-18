# Comparing `tmp/gp2-0.0.1.tar.gz` & `tmp/gp2-0.5.18.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2-0.0.1.tar", last modified: Thu May 18 20:29:15 2023, max compression
+gzip compressed data, was "gp2-0.5.18.23.tar", last modified: Thu May 18 20:42:55 2023, max compression
```

## Comparing `gp2-0.0.1.tar` & `gp2-0.5.18.23.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:22:04.000000 gp2-0.0.1/
--rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.0.1/LICENSE
--rw-r--r--   0  1981811  1981811      626 2023-05-18 20:22:04.000000 gp2-0.0.1/PKG-INFO
--rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.0.1/README.md
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:21:43.000000 gp2-0.0.1/gp2/
--rw-rw-r--   0  1981811  1981811      597 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/__init__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:21:49.000000 gp2-0.0.1/gp2/data/
--rw-rw-r--   0  1981811  1981811      666 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/data/__init__.py
--rw-rw-r--   0  1981811  1981811     2970 2023-05-03 06:40:53.000000 gp2-0.0.1/gp2/data/collection.py
--rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.0.1/gp2/data/manager.py
--rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.0.1/gp2/data/point.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:21:51.000000 gp2-0.0.1/gp2/gp2/
--rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/__init__.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:22:01.000000 gp2-0.0.1/gp2/gp2/classifiers/
--rw-rw-r--   0  1981811  1981811     1026 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/__init__.py
--rw-rw-r--   0  1981811  1981811     3918 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
--rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/classifier.py
--rw-rw-r--   0  1981811  1981811     7114 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_att_unet2d.py
--rw-rw-r--   0  1981811  1981811     5010 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_r2_unet2d.py
--rw-rw-r--   0  1981811  1981811     5786 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_res_unet2d.py
--rw-rw-r--   0  1981811  1981811     5564 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_unet.py
--rw-rw-r--   0  1981811  1981811     6349 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_unet2d.py
--rw-rw-r--   0  1981811  1981811     8242 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_unet3_plus2d.py
--rw-rw-r--   0  1981811  1981811     6692 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_unet_plus2d.py
--rw-rw-r--   0  1981811  1981811     5124 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/k_vnet2d.py
--rw-rw-r--   0  1981811  1981811    10246 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/unet.py
--rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/classifiers/unet_plus.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:22:04.000000 gp2-0.0.1/gp2/gp2/discriminators/
--rw-rw-r--   0  1981811  1981811      774 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/discriminators/__init__.py
--rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/discriminators/base_cnn_discriminator.py
--rw-rw-r--   0  1981811  1981811     3660 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/discriminators/cnn_discriminator_plus.py
--rw-rw-r--   0  1981811  1981811     5157 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/discriminators/cnndiscriminator.py
--rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/discriminators/discriminator.py
--rw-rw-r--   0  1981811  1981811     7567 2023-05-03 03:30:40.000000 gp2-0.0.1/gp2/gp2/util.py
--rw-rw-r--   0  1981811  1981811    28994 2023-05-18 17:38:30.000000 gp2-0.0.1/gp2/runner.py
-drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:21:46.000000 gp2-0.0.1/gp2.egg-info/
--rw-r--r--   0  1981811  1981811      626 2023-05-18 20:21:37.000000 gp2-0.0.1/gp2.egg-info/PKG-INFO
--rw-r--r--   0  1981811  1981811      959 2023-05-18 20:21:39.000000 gp2-0.0.1/gp2.egg-info/SOURCES.txt
--rw-r--r--   0  1981811  1981811        1 2023-05-18 20:21:37.000000 gp2-0.0.1/gp2.egg-info/dependency_links.txt
--rw-r--r--   0  1981811  1981811        4 2023-05-18 20:21:38.000000 gp2-0.0.1/gp2.egg-info/top_level.txt
--rw-r--r--   0  1981811  1981811       38 2023-05-18 20:22:04.000000 gp2-0.0.1/setup.cfg
--rw-r--r--   0  1981811  1981811     2583 2023-05-18 20:20:33.000000 gp2-0.0.1/setup.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:44.000000 gp2-0.5.18.23/
+-rw-rw-r--   0  1981811  1981811     1068 2023-05-03 06:05:46.000000 gp2-0.5.18.23/LICENSE
+-rw-r--r--   0  1981811  1981811      630 2023-05-18 20:35:44.000000 gp2-0.5.18.23/PKG-INFO
+-rw-rw-r--   0  1981811  1981811     3677 2023-05-03 06:16:48.000000 gp2-0.5.18.23/README.md
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:31.000000 gp2-0.5.18.23/gp2/
+-rw-rw-r--   0  1981811  1981811      597 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/__init__.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:35.000000 gp2-0.5.18.23/gp2/data/
+-rw-rw-r--   0  1981811  1981811      666 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/data/__init__.py
+-rw-rw-r--   0  1981811  1981811     2970 2023-05-03 06:40:53.000000 gp2-0.5.18.23/gp2/data/collection.py
+-rw-rw-r--   0  1981811  1981811     5051 2023-05-03 06:31:35.000000 gp2-0.5.18.23/gp2/data/manager.py
+-rw-rw-r--   0  1981811  1981811      296 2023-05-03 06:25:06.000000 gp2-0.5.18.23/gp2/data/point.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:36.000000 gp2-0.5.18.23/gp2/gp2/
+-rw-rw-r--   0  1981811  1981811      118 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/__init__.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:42.000000 gp2-0.5.18.23/gp2/gp2/classifiers/
+-rw-rw-r--   0  1981811  1981811     1026 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/__init__.py
+-rw-rw-r--   0  1981811  1981811     3918 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py
+-rw-rw-r--   0  1981811  1981811      829 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/classifier.py
+-rw-rw-r--   0  1981811  1981811     7114 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_att_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5010 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_r2_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5786 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_res_unet2d.py
+-rw-rw-r--   0  1981811  1981811     5564 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_unet.py
+-rw-rw-r--   0  1981811  1981811     6349 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_unet2d.py
+-rw-rw-r--   0  1981811  1981811     8242 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_unet3_plus2d.py
+-rw-rw-r--   0  1981811  1981811     6692 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_unet_plus2d.py
+-rw-rw-r--   0  1981811  1981811     5124 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/k_vnet2d.py
+-rw-rw-r--   0  1981811  1981811    10246 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/unet.py
+-rw-rw-r--   0  1981811  1981811     6248 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/classifiers/unet_plus.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:44.000000 gp2-0.5.18.23/gp2/gp2/discriminators/
+-rw-rw-r--   0  1981811  1981811      774 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/discriminators/__init__.py
+-rw-rw-r--   0  1981811  1981811     4430 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/discriminators/base_cnn_discriminator.py
+-rw-rw-r--   0  1981811  1981811     3660 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/discriminators/cnn_discriminator_plus.py
+-rw-rw-r--   0  1981811  1981811     5157 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/discriminators/cnndiscriminator.py
+-rw-rw-r--   0  1981811  1981811      505 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/discriminators/discriminator.py
+-rw-rw-r--   0  1981811  1981811     7567 2023-05-03 03:30:40.000000 gp2-0.5.18.23/gp2/gp2/util.py
+-rw-rw-r--   0  1981811  1981811    28998 2023-05-18 20:34:47.000000 gp2-0.5.18.23/gp2/runner.py
+drwxr-xr-x   0  1981811  1981811        0 2023-05-18 20:35:33.000000 gp2-0.5.18.23/gp2.egg-info/
+-rw-r--r--   0  1981811  1981811      630 2023-05-18 20:35:19.000000 gp2-0.5.18.23/gp2.egg-info/PKG-INFO
+-rw-r--r--   0  1981811  1981811      985 2023-05-18 20:35:22.000000 gp2-0.5.18.23/gp2.egg-info/SOURCES.txt
+-rw-r--r--   0  1981811  1981811        1 2023-05-18 20:35:20.000000 gp2-0.5.18.23/gp2.egg-info/dependency_links.txt
+-rw-r--r--   0  1981811  1981811       55 2023-05-18 20:35:20.000000 gp2-0.5.18.23/gp2.egg-info/requires.txt
+-rw-r--r--   0  1981811  1981811        4 2023-05-18 20:35:20.000000 gp2-0.5.18.23/gp2.egg-info/top_level.txt
+-rw-r--r--   0  1981811  1981811       38 2023-05-18 20:35:44.000000 gp2-0.5.18.23/setup.cfg
+-rw-r--r--   0  1981811  1981811      933 2023-05-18 20:33:19.000000 gp2-0.5.18.23/setup.py
```

### Comparing `gp2-0.0.1/LICENSE` & `gp2-0.5.18.23/LICENSE`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/PKG-INFO` & `gp2-0.5.18.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2
-Version: 0.0.1
+Version: 0.5.18.23
 Summary: A framework for tuning segmentation classifiers and discriminators
 Home-page: https://github.com/RyanZurrin/CS410-GP2
 Author: mpsych lab
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gp2-0.0.1/README.md` & `gp2-0.5.18.23/README.md`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/__init__.py` & `gp2-0.5.18.23/gp2/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/data/__init__.py` & `gp2-0.5.18.23/gp2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/data/collection.py` & `gp2-0.5.18.23/gp2/data/collection.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/data/manager.py` & `gp2-0.5.18.23/gp2/data/manager.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/__init__.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/base_keras_segmentation_classifier.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/base_keras_segmentation_classifier.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/classifier.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/classifier.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_att_unet2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_att_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_r2_unet2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_r2_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_res_unet2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_res_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_unet.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_unet.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_unet2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_unet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_unet3_plus2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_unet3_plus2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_unet_plus2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_unet_plus2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/k_vnet2d.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/k_vnet2d.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/unet.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/unet.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/classifiers/unet_plus.py` & `gp2-0.5.18.23/gp2/gp2/classifiers/unet_plus.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/discriminators/__init__.py` & `gp2-0.5.18.23/gp2/gp2/discriminators/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/discriminators/base_cnn_discriminator.py` & `gp2-0.5.18.23/gp2/gp2/discriminators/base_cnn_discriminator.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/discriminators/cnn_discriminator_plus.py` & `gp2-0.5.18.23/gp2/gp2/discriminators/cnn_discriminator_plus.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/discriminators/cnndiscriminator.py` & `gp2-0.5.18.23/gp2/gp2/discriminators/cnndiscriminator.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/gp2/util.py` & `gp2-0.5.18.23/gp2/gp2/util.py`

 * *Files identical despite different names*

### Comparing `gp2-0.0.1/gp2/runner.py` & `gp2-0.5.18.23/gp2/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     CNNDiscriminatorPLUS, Util
 import time
 import numpy as np
 import os
 import tempfile
 
 # set the version number
-__version__ = '0.0.1'
+__version__ = '0.5.18.23'
 
 def validate_weights(weights, tolerance=1e-6):
     """ Validate the weights for training.
 
     What must be verified:
         A_train + A_val + A_test = 1. \n
         B_train + B_val + B_test = 1. \n
```

### Comparing `gp2-0.0.1/gp2.egg-info/PKG-INFO` & `gp2-0.5.18.23/gp2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gp2
-Version: 0.0.1
+Version: 0.5.18.23
 Summary: A framework for tuning segmentation classifiers and discriminators
 Home-page: https://github.com/RyanZurrin/CS410-GP2
 Author: mpsych lab
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gp2-0.0.1/gp2.egg-info/SOURCES.txt` & `gp2-0.5.18.23/gp2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 gp2/__init__.py
 gp2/runner.py
 gp2.egg-info/PKG-INFO
 gp2.egg-info/SOURCES.txt
 gp2.egg-info/dependency_links.txt
+gp2.egg-info/requires.txt
 gp2.egg-info/top_level.txt
 gp2/data/__init__.py
 gp2/data/collection.py
 gp2/data/manager.py
 gp2/data/point.py
 gp2/gp2/__init__.py
 gp2/gp2/util.py
```

