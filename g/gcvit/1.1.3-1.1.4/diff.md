# Comparing `tmp/gcvit-1.1.3.tar.gz` & `tmp/gcvit-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcvit-1.1.3.tar", last modified: Sun May  7 18:27:50 2023, max compression
+gzip compressed data, was "gcvit-1.1.4.tar", last modified: Thu May 18 13:19:11 2023, max compression
```

## Comparing `gcvit-1.1.3.tar` & `gcvit-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.172021 gcvit-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 18:27:41.000000 gcvit-1.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-07 18:27:50.172021 gcvit-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-07 18:27:41.000000 gcvit-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.168021 gcvit-1.1.3/gcvit/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.172021 gcvit-1.1.3/gcvit/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/layers/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.172021 gcvit-1.1.3/gcvit/models/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/models/gcvit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.172021 gcvit-1.1.3/gcvit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/utils/conv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/utils/gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 18:27:41.000000 gcvit-1.1.3/gcvit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.172021 gcvit-1.1.3/gcvit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-07 18:27:50.000000 gcvit-1.1.3/gcvit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-07 18:27:50.000000 gcvit-1.1.3/gcvit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:27:50.000000 gcvit-1.1.3/gcvit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 18:27:50.000000 gcvit-1.1.3/gcvit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 18:27:50.000000 gcvit-1.1.3/gcvit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 18:27:50.172021 gcvit-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-07 18:27:41.000000 gcvit-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:27:50.172021 gcvit-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-07 18:27:41.000000 gcvit-1.1.3/tests/test_gcvit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.035433 gcvit-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 13:19:02.000000 gcvit-1.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-18 13:19:11.035433 gcvit-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-18 13:19:02.000000 gcvit-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.031433 gcvit-1.1.4/gcvit/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.031433 gcvit-1.1.4/gcvit/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/layers/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.031433 gcvit-1.1.4/gcvit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/models/gcvit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.035433 gcvit-1.1.4/gcvit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/utils/conv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/utils/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 13:19:02.000000 gcvit-1.1.4/gcvit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.031433 gcvit-1.1.4/gcvit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-18 13:19:11.000000 gcvit-1.1.4/gcvit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-18 13:19:11.000000 gcvit-1.1.4/gcvit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:19:11.000000 gcvit-1.1.4/gcvit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 13:19:11.000000 gcvit-1.1.4/gcvit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 13:19:11.000000 gcvit-1.1.4/gcvit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 13:19:11.035433 gcvit-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-18 13:19:02.000000 gcvit-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:19:11.035433 gcvit-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-18 13:19:02.000000 gcvit-1.1.4/tests/test_gcvit.py
```

### Comparing `gcvit-1.1.3/LICENSE.md` & `gcvit-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/PKG-INFO` & `gcvit-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcvit
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tensorflow 2.0 Implementation of GCViT: Global Context Vision Transformer. https://github.com/awsaf49/gcvit-tf
 Home-page: https://github.com/awsaf49/gcvit-tf
 Author: Awsaf
 Author-email: awsaf49@gmail.com
 License: MIT
 Keywords: tensorflow computer_vision image classification transformer
 Classifier: Development Status :: 3 - Alpha
@@ -122,15 +122,15 @@
 ```
 Feature map:
 ```py
 (None, 7, 7, 512)
 ```
 
 ## Kaggle Models
-These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models with downloading, thus can be used without internet in Kaggle.
+These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models without downloading, thus can be used without internet in Kaggle.
 ```py
 from gcvit import GCViTTiny
 model = GCViTTiny(pretrain=True, from_kaggle=True)
 ```
 
 ## Live-Demo
 * For live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click <a target="_blank" href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="https://img.shields.io/badge/Try%20on-Gradio-orange"></a> powered by 🤗 Space and Gradio. here's an example,
@@ -144,15 +144,15 @@
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/flower_gradcam.PNG" height=500>
 
 
 
 ## To Do
 - [ ] Segmentation Pipeline
-- [ ] Support for `Kaggle Models`
+- [x] Support for `Kaggle Models`
 - [x] Remove `tensorflow_addons`
 - [x] New updated weights have been added.
 - [x] Working training example in Colab & Kaggle.
 - [x] GradCAM showcase.
 - [x] Gradio Demo.
 - [x] Build model with `tf.keras.Model`.
 - [x] Port weights from official repo.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gcvit Version: 1.1.3 Summary: Tensorflow 2.0
+Metadata-Version: 2.1 Name: gcvit Version: 1.1.4 Summary: Tensorflow 2.0
 Implementation of GCViT: Global Context Vision Transformer. https://github.com/
 awsaf49/gcvit-tf Home-page: https://github.com/awsaf49/gcvit-tf Author: Awsaf
 Author-email: awsaf49@gmail.com License: MIT Keywords: tensorflow
 computer_vision image classification transformer Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.6 Classifier:
@@ -52,24 +52,24 @@
 num_classes must be 1000 model.reset_classifier(num_classes=0, head_act=None)
 feature = model(img) print(feature.shape) ``` Feature: ```py (None, 512) ```
 For feature map: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 feature = model.forward_features(img) print
 (feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Kaggle Models
 These pre-trained models can also be loaded using [Kaggle Models](https://
 www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will
-enforce model to load weights from Kaggle Models with downloading, thus can be
-used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
+enforce model to load weights from Kaggle Models without downloading, thus can
+be used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
 GCViTTiny(pretrain=True, from_kaggle=True) ``` ## Live-Demo * For live demo on
 Image Classification & Grad-CAM, with **ImageNet** weights, click [https://
 img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and Gradio.
 here's an example, [image/gradio_demo.JPG] ## Example For working training
 example checkout these notebooks on **Google Colab** [Open_In_Colab] &
 **Kaggle** [Open_In_Kaggle]. Here is grad-cam result after training on Flower
 Classification Dataset, [https://raw.githubusercontent.com/awsaf49/gcvit-tf/
-main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [ ]
+main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [x]
 Support for `Kaggle Models` - [x] Remove `tensorflow_addons` - [x] New updated
 weights have been added. - [x] Working training example in Colab & Kaggle. -
 [x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
 `tf.keras.Model`. - [x] Port weights from official repo. - [x] Support for
 `TPU`. ## Acknowledgement * [GCVit](https://github.com/NVlabs/GCVit) (Official)
 * [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF) *
 [tfgcvit](https://github.com/shkarupa-alex/tfgcvit/tree/develop/tfgcvit) *
```

### Comparing `gcvit-1.1.3/README.md` & `gcvit-1.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 ```
 Feature map:
 ```py
 (None, 7, 7, 512)
 ```
 
 ## Kaggle Models
-These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models with downloading, thus can be used without internet in Kaggle.
+These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models without downloading, thus can be used without internet in Kaggle.
 ```py
 from gcvit import GCViTTiny
 model = GCViTTiny(pretrain=True, from_kaggle=True)
 ```
 
 ## Live-Demo
 * For live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click <a target="_blank" href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="https://img.shields.io/badge/Try%20on-Gradio-orange"></a> powered by 🤗 Space and Gradio. here's an example,
@@ -119,15 +119,15 @@
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/flower_gradcam.PNG" height=500>
 
 
 
 ## To Do
 - [ ] Segmentation Pipeline
-- [ ] Support for `Kaggle Models`
+- [x] Support for `Kaggle Models`
 - [x] Remove `tensorflow_addons`
 - [x] New updated weights have been added.
 - [x] Working training example in Colab & Kaggle.
 - [x] GradCAM showcase.
 - [x] Gradio Demo.
 - [x] Build model with `tf.keras.Model`.
 - [x] Port weights from official repo.
```

#### html2text {}

```diff
@@ -38,24 +38,24 @@
 num_classes must be 1000 model.reset_classifier(num_classes=0, head_act=None)
 feature = model(img) print(feature.shape) ``` Feature: ```py (None, 512) ```
 For feature map: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 feature = model.forward_features(img) print
 (feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Kaggle Models
 These pre-trained models can also be loaded using [Kaggle Models](https://
 www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will
-enforce model to load weights from Kaggle Models with downloading, thus can be
-used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
+enforce model to load weights from Kaggle Models without downloading, thus can
+be used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
 GCViTTiny(pretrain=True, from_kaggle=True) ``` ## Live-Demo * For live demo on
 Image Classification & Grad-CAM, with **ImageNet** weights, click [https://
 img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and Gradio.
 here's an example, [image/gradio_demo.JPG] ## Example For working training
 example checkout these notebooks on **Google Colab** [Open_In_Colab] &
 **Kaggle** [Open_In_Kaggle]. Here is grad-cam result after training on Flower
 Classification Dataset, [https://raw.githubusercontent.com/awsaf49/gcvit-tf/
-main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [ ]
+main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [x]
 Support for `Kaggle Models` - [x] Remove `tensorflow_addons` - [x] New updated
 weights have been added. - [x] Working training example in Colab & Kaggle. -
 [x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
 `tf.keras.Model`. - [x] Port weights from official repo. - [x] Support for
 `TPU`. ## Acknowledgement * [GCVit](https://github.com/NVlabs/GCVit) (Official)
 * [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF) *
 [tfgcvit](https://github.com/shkarupa-alex/tfgcvit/tree/develop/tfgcvit) *
```

### Comparing `gcvit-1.1.3/gcvit/layers/attention.py` & `gcvit-1.1.4/gcvit/layers/attention.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/block.py` & `gcvit-1.1.4/gcvit/layers/block.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/drop.py` & `gcvit-1.1.4/gcvit/layers/drop.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/embedding.py` & `gcvit-1.1.4/gcvit/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/feature.py` & `gcvit-1.1.4/gcvit/layers/feature.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/level.py` & `gcvit-1.1.4/gcvit/layers/level.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/pooling.py` & `gcvit-1.1.4/gcvit/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/layers/window.py` & `gcvit-1.1.4/gcvit/layers/window.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/models/gcvit.py` & `gcvit-1.1.4/gcvit/models/gcvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 BASE_URL = "https://github.com/awsaf49/gcvit-tf/releases/download"
 TAG = "v1.1.1"
 
 # Params for Kaggle Models (KM)
 KM_DIR = "/kaggle/input/gcvit-tf/tensorflow2"
 KM_VERSION = "1"
 NAME2TITLE = {
-    "gcvit_xxtiny": "GCViT-XXTiny",
-    "gcvit_xtiny": "GCViT-XTiny",
-    "gcvit_tiny": "GCViT-Tiny",
-    "gcvit_small": "GCViT-Small",
-    "gcvit_base": "GCViT-Base",
-    "gcvit_large": "GCViT-Large",
+    "gcvit_xxtiny": "gcvit-xxtiny",
+    "gcvit_xtiny": "gcvit-xtiny",
+    "gcvit_tiny": "gcvit-tiny",
+    "gcvit_small": "gcvit-small",
+    "gcvit_base": "gcvit-base",
+    "gcvit_large": "gcvit-large",
 }
 
 NAME2CONFIG = {
     "gcvit_xxtiny": {
         "window_size": (7, 7, 14, 7),
         "dim": 64,
         "depths": (2, 2, 6, 2),
```

### Comparing `gcvit-1.1.3/gcvit/utils/conv_utils.py` & `gcvit-1.1.4/gcvit/utils/conv_utils.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit/utils/gradcam.py` & `gcvit-1.1.4/gcvit/utils/gradcam.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/gcvit.egg-info/PKG-INFO` & `gcvit-1.1.4/gcvit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcvit
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tensorflow 2.0 Implementation of GCViT: Global Context Vision Transformer. https://github.com/awsaf49/gcvit-tf
 Home-page: https://github.com/awsaf49/gcvit-tf
 Author: Awsaf
 Author-email: awsaf49@gmail.com
 License: MIT
 Keywords: tensorflow computer_vision image classification transformer
 Classifier: Development Status :: 3 - Alpha
@@ -122,15 +122,15 @@
 ```
 Feature map:
 ```py
 (None, 7, 7, 512)
 ```
 
 ## Kaggle Models
-These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models with downloading, thus can be used without internet in Kaggle.
+These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models without downloading, thus can be used without internet in Kaggle.
 ```py
 from gcvit import GCViTTiny
 model = GCViTTiny(pretrain=True, from_kaggle=True)
 ```
 
 ## Live-Demo
 * For live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click <a target="_blank" href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="https://img.shields.io/badge/Try%20on-Gradio-orange"></a> powered by 🤗 Space and Gradio. here's an example,
@@ -144,15 +144,15 @@
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/flower_gradcam.PNG" height=500>
 
 
 
 ## To Do
 - [ ] Segmentation Pipeline
-- [ ] Support for `Kaggle Models`
+- [x] Support for `Kaggle Models`
 - [x] Remove `tensorflow_addons`
 - [x] New updated weights have been added.
 - [x] Working training example in Colab & Kaggle.
 - [x] GradCAM showcase.
 - [x] Gradio Demo.
 - [x] Build model with `tf.keras.Model`.
 - [x] Port weights from official repo.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gcvit Version: 1.1.3 Summary: Tensorflow 2.0
+Metadata-Version: 2.1 Name: gcvit Version: 1.1.4 Summary: Tensorflow 2.0
 Implementation of GCViT: Global Context Vision Transformer. https://github.com/
 awsaf49/gcvit-tf Home-page: https://github.com/awsaf49/gcvit-tf Author: Awsaf
 Author-email: awsaf49@gmail.com License: MIT Keywords: tensorflow
 computer_vision image classification transformer Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.6 Classifier:
@@ -52,24 +52,24 @@
 num_classes must be 1000 model.reset_classifier(num_classes=0, head_act=None)
 feature = model(img) print(feature.shape) ``` Feature: ```py (None, 512) ```
 For feature map: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 feature = model.forward_features(img) print
 (feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Kaggle Models
 These pre-trained models can also be loaded using [Kaggle Models](https://
 www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will
-enforce model to load weights from Kaggle Models with downloading, thus can be
-used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
+enforce model to load weights from Kaggle Models without downloading, thus can
+be used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
 GCViTTiny(pretrain=True, from_kaggle=True) ``` ## Live-Demo * For live demo on
 Image Classification & Grad-CAM, with **ImageNet** weights, click [https://
 img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and Gradio.
 here's an example, [image/gradio_demo.JPG] ## Example For working training
 example checkout these notebooks on **Google Colab** [Open_In_Colab] &
 **Kaggle** [Open_In_Kaggle]. Here is grad-cam result after training on Flower
 Classification Dataset, [https://raw.githubusercontent.com/awsaf49/gcvit-tf/
-main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [ ]
+main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [x]
 Support for `Kaggle Models` - [x] Remove `tensorflow_addons` - [x] New updated
 weights have been added. - [x] Working training example in Colab & Kaggle. -
 [x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
 `tf.keras.Model`. - [x] Port weights from official repo. - [x] Support for
 `TPU`. ## Acknowledgement * [GCVit](https://github.com/NVlabs/GCVit) (Official)
 * [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF) *
 [tfgcvit](https://github.com/shkarupa-alex/tfgcvit/tree/develop/tfgcvit) *
```

### Comparing `gcvit-1.1.3/gcvit.egg-info/SOURCES.txt` & `gcvit-1.1.4/gcvit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/setup.py` & `gcvit-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.3/tests/test_gcvit.py` & `gcvit-1.1.4/tests/test_gcvit.py`

 * *Files identical despite different names*

