# Comparing `tmp/cliptry1-0.1.4.tar.gz` & `tmp/cliptry1-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliptry1-0.1.4.tar", last modified: Thu May 18 09:36:49 2023, max compression
+gzip compressed data, was "cliptry1-0.1.5.tar", last modified: Thu May 18 09:56:41 2023, max compression
```

## Comparing `cliptry1-0.1.4.tar` & `cliptry1-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 09:36:49.412921 cliptry1-0.1.4/
--rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      236 2023-05-18 09:36:49.409922 cliptry1-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.1.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 09:36:49.377925 cliptry1-0.1.4/cliptry1.egg-info/
--rw-rw-rw-   0        0        0      236 2023-05-18 09:36:48.000000 cliptry1-0.1.4/cliptry1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-18 09:36:49.000000 cliptry1-0.1.4/cliptry1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      124 2023-05-18 09:36:48.000000 cliptry1-0.1.4/cliptry1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-18 09:36:48.000000 cliptry1-0.1.4/cliptry1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 09:36:48.000000 cliptry1-0.1.4/cliptry1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 09:36:49.387923 cliptry1-0.1.4/jaical/
--rw-rw-rw-   0        0        0     2710 2023-05-18 09:36:06.000000 cliptry1-0.1.4/jaical/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-18 09:36:49.413922 cliptry1-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      526 2023-05-18 09:36:20.000000 cliptry1-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:56:41.181779 cliptry1-0.1.5/
+-rw-rw-rw-   0        0        0       25 2020-04-19 14:59:35.000000 cliptry1-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      236 2023-05-18 09:56:41.175778 cliptry1-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      106 2020-04-19 14:58:18.000000 cliptry1-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 09:56:41.153779 cliptry1-0.1.5/cliptry1.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-05-18 09:56:40.000000 cliptry1-0.1.5/cliptry1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-18 09:56:40.000000 cliptry1-0.1.5/cliptry1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      124 2023-05-18 09:56:40.000000 cliptry1-0.1.5/cliptry1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-18 09:56:40.000000 cliptry1-0.1.5/cliptry1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 09:56:40.000000 cliptry1-0.1.5/cliptry1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 09:56:41.167779 cliptry1-0.1.5/jaical/
+-rw-rw-rw-   0        0        0     2104 2023-05-18 09:56:13.000000 cliptry1-0.1.5/jaical/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 09:56:41.185778 cliptry1-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      526 2023-05-18 09:56:22.000000 cliptry1-0.1.5/setup.py
```

### Comparing `cliptry1-0.1.4/jaical/__init__.py` & `cliptry1-0.1.5/jaical/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,12 @@
 import os
 import clip
 import torch
 #from torchvision.datasets import CIFAR100
 import PIL.Image as Image
-import numpy as np
-def add_numbers(num1, num2):
-    return num1 + num2
-
-def subtract_numbers(num1, num2):
-    return num1 - num2
-
-def multiply_numbers(num1, num2):
-    return num1 * num2
-
-def divide_numbers(num1, num2):
-    return num1 / num2
-
-def deg_to_Rad(num1):
-    return np.deg2rad(num1)
-
-def power(num1,num2):
-    return np.power(num1,num2)
-
-def list_models():
-    return clip.available_models()
-def apna_model():
-    device = "cuda" if torch.cuda.is_available() else "cpu"
-    model, preprocess = clip.load('ViT-B/32', device)
-    print("model loaded successfully")
-   
 device = "cuda" if torch.cuda.is_available() else "cpu"
 model, preprocess = clip.load('ViT-B/32', device)
 answer=[]
 image_pair={}
 def image_pair_Dir(path):
     folder_dir = path
     img_path=[]
@@ -66,22 +40,22 @@
     text_answer.append(text_features.T)
     return text_answer
 def similar_f(path,txt):
     final_ans=[]
     text_answer=[]
     if(len(answer) == 0):
         image_feature_extract(path)
-        print(answer)
+        #print(answer)
     else:
         x= len(answer)
-        print(x)
+        #print(x)
     text_answer = text_feature(txt)
     with torch.no_grad():
         for k in range(0, len(answer)):
             ans = (answer[k] @ text_answer[0])
             #print(ans)
             if(ans >25):
                 #print(ans)
                if k in image_pair:
                    i = image_pair[k]
                    final_ans.append(i)
-        return(final_ans)
+    return(final_ans)
```

### Comparing `cliptry1-0.1.4/setup.py` & `cliptry1-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup (
   name='cliptry1',
-  version='0.1.4',
+  version='0.1.5',
   description='A very basic calculator',
   url='',  
   author='jaideep ',
   author_email='jaideepkaushal2@gmail.com',
   license='MIT', 
   keywords='calculator', 
   packages=find_packages(),
```

