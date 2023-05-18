# Comparing `tmp/torchfitter-4.2.2.tar.gz` & `tmp/torchfitter-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchfitter-4.2.2.tar", last modified: Tue Apr 18 14:07:18 2023, max compression
+gzip compressed data, was "torchfitter-4.3.0.tar", last modified: Thu May 18 17:57:53 2023, max compression
```

## Comparing `torchfitter-4.2.2.tar` & `torchfitter-4.3.0.tar`

### file list

```diff
@@ -1,42 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 14:07:03.000000 torchfitter-4.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-18 14:07:18.131214 torchfitter-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-18 14:07:03.000000 torchfitter-4.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 14:07:18.131214 torchfitter-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-18 14:07:03.000000 torchfitter-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.127214 torchfitter-4.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/progress/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/progress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/regularization/
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/regularization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/callbacks/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/callbacks/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/conventions.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/trainer/_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/trainer/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-18 14:07:03.000000 torchfitter-4.2.2/src/torchfitter/utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:18.131214 torchfitter-4.2.2/src/torchfitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 14:07:18.000000 torchfitter-4.2.2/src/torchfitter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70466 2023-04-18 14:07:03.000000 torchfitter-4.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 17:57:42.000000 torchfitter-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-18 17:57:53.192166 torchfitter-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-18 17:57:42.000000 torchfitter-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 17:57:53.192166 torchfitter-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-18 17:57:42.000000 torchfitter-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.188166 torchfitter-4.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/callbacks/_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16329 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/callbacks/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/callbacks/progress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/callbacks/regularization/
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/callbacks/regularization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/callbacks/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/callbacks/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/trainer/_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/trainer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/utils/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-18 17:57:42.000000 torchfitter-4.3.0/src/torchfitter/utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:53.192166 torchfitter-4.3.0/src/torchfitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-18 17:57:53.000000 torchfitter-4.3.0/src/torchfitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-18 17:57:53.000000 torchfitter-4.3.0/src/torchfitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:57:53.000000 torchfitter-4.3.0/src/torchfitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 17:57:53.000000 torchfitter-4.3.0/src/torchfitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 17:57:53.000000 torchfitter-4.3.0/src/torchfitter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    70466 2023-05-18 17:57:42.000000 torchfitter-4.3.0/versioneer.py
```

### Comparing `torchfitter-4.2.2/PKG-INFO` & `torchfitter-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchfitter
-Version: 4.2.2
+Version: 4.3.0
 Summary: Trainer to optimize PyTorch models
 Author: Alejandro Pérez-Sanjuán
 Requires-Python: >=3.7,
 Description-Content-Type: text/markdown
 
 
 <p align="center">
@@ -104,15 +104,15 @@
     scheduler=optim.lr_scheduler.StepLR(optimizer, step_size=500, gamma=0.9)
 )
 
 trainer = Trainer(
     model=model, 
     criterion=criterion,
     optimizer=optimizer,
-    mixed_precision=True,
+    mixed_precision="fp16",
     accumulate_iter=4, # accumulate gradient every 4 iterations,
     gradient_clipping='norm',
     gradient_clipping_kwrgs={'max_norm': 1.0, 'norm_type': 2.0},
     callbacks=[l1_reg, scheduler, early_stopping, logger]
 )
 
 history = trainer.fit(train_loader, val_loader, epochs=1000)
```

### Comparing `torchfitter-4.2.2/README.md` & `torchfitter-4.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     scheduler=optim.lr_scheduler.StepLR(optimizer, step_size=500, gamma=0.9)
 )
 
 trainer = Trainer(
     model=model, 
     criterion=criterion,
     optimizer=optimizer,
-    mixed_precision=True,
+    mixed_precision="fp16",
     accumulate_iter=4, # accumulate gradient every 4 iterations,
     gradient_clipping='norm',
     gradient_clipping_kwrgs={'max_norm': 1.0, 'norm_type': 2.0},
     callbacks=[l1_reg, scheduler, early_stopping, logger]
 )
 
 history = trainer.fit(train_loader, val_loader, epochs=1000)
```

### Comparing `torchfitter-4.2.2/setup.py` & `torchfitter-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,13 @@
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     author="Alejandro Pérez-Sanjuán",
     python_requires=">=3.7,",
     install_requires=[
         "rich",
         "numpy>=1.20.0",
-        "accelerate>=0.11.0",
+        "accelerate>=0.19.0",
         "scikit-learn",
         "torchmetrics",
-        "torch>=1.1.0",
+        "torch>=1.6",
     ],
 )
```

### Comparing `torchfitter-4.2.2/src/torchfitter/callbacks/__init__.py` & `torchfitter-4.3.0/src/torchfitter/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/callbacks/_callbacks.py` & `torchfitter-4.3.0/src/torchfitter/callbacks/_callbacks.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/callbacks/base.py` & `torchfitter-4.3.0/src/torchfitter/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/callbacks/progress/__init__.py` & `torchfitter-4.3.0/src/torchfitter/callbacks/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/callbacks/regularization/__init__.py` & `torchfitter-4.3.0/src/torchfitter/callbacks/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/callbacks/scheduling/__init__.py` & `torchfitter-4.3.0/src/torchfitter/callbacks/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/conventions.py` & `torchfitter-4.3.0/src/torchfitter/conventions.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/io.py` & `torchfitter-4.3.0/src/torchfitter/io.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/testing.py` & `torchfitter-4.3.0/src/torchfitter/testing.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/trainer/_trainer.py` & `torchfitter-4.3.0/src/torchfitter/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/trainer/_utils.py` & `torchfitter-4.3.0/src/torchfitter/trainer/_utils.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/utils/convenience.py` & `torchfitter-4.3.0/src/torchfitter/utils/convenience.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/utils/data.py` & `torchfitter-4.3.0/src/torchfitter/utils/data.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter/utils/preprocessing.py` & `torchfitter-4.3.0/src/torchfitter/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `torchfitter-4.2.2/src/torchfitter.egg-info/PKG-INFO` & `torchfitter-4.3.0/src/torchfitter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchfitter
-Version: 4.2.2
+Version: 4.3.0
 Summary: Trainer to optimize PyTorch models
 Author: Alejandro Pérez-Sanjuán
 Requires-Python: >=3.7,
 Description-Content-Type: text/markdown
 
 
 <p align="center">
@@ -104,15 +104,15 @@
     scheduler=optim.lr_scheduler.StepLR(optimizer, step_size=500, gamma=0.9)
 )
 
 trainer = Trainer(
     model=model, 
     criterion=criterion,
     optimizer=optimizer,
-    mixed_precision=True,
+    mixed_precision="fp16",
     accumulate_iter=4, # accumulate gradient every 4 iterations,
     gradient_clipping='norm',
     gradient_clipping_kwrgs={'max_norm': 1.0, 'norm_type': 2.0},
     callbacks=[l1_reg, scheduler, early_stopping, logger]
 )
 
 history = trainer.fit(train_loader, val_loader, epochs=1000)
```

### Comparing `torchfitter-4.2.2/src/torchfitter.egg-info/SOURCES.txt` & `torchfitter-4.3.0/src/torchfitter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 src/torchfitter.egg-info/top_level.txt
 src/torchfitter/callbacks/__init__.py
 src/torchfitter/callbacks/_callbacks.py
 src/torchfitter/callbacks/base.py
 src/torchfitter/callbacks/progress/__init__.py
 src/torchfitter/callbacks/regularization/__init__.py
 src/torchfitter/callbacks/scheduling/__init__.py
-src/torchfitter/manager/__init__.py
-src/torchfitter/manager/_manager.py
 src/torchfitter/trainer/__init__.py
 src/torchfitter/trainer/_trainer.py
 src/torchfitter/trainer/_utils.py
 src/torchfitter/utils/__init__.py
 src/torchfitter/utils/convenience.py
 src/torchfitter/utils/data.py
 src/torchfitter/utils/preprocessing.py
```

### Comparing `torchfitter-4.2.2/versioneer.py` & `torchfitter-4.3.0/versioneer.py`

 * *Files identical despite different names*

