# Comparing `tmp/lightgbm_callbacks-0.1.0.tar.gz` & `tmp/lightgbm_callbacks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightgbm_callbacks-0.1.0.tar", max compression
+gzip compressed data, was "lightgbm_callbacks-0.1.1.tar", max compression
```

## Comparing `lightgbm_callbacks-0.1.0.tar` & `lightgbm_callbacks-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1114 2023-05-18 13:19:52.409314 lightgbm_callbacks-0.1.0/LICENSE
--rw-r--r--   0        0        0     7542 2023-05-18 13:19:52.409314 lightgbm_callbacks-0.1.0/README.md
--rw-r--r--   0        0        0     2477 2023-05-18 13:19:53.545327 lightgbm_callbacks-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      614 2023-05-18 13:19:53.481326 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/__init__.py
--rw-r--r--   0        0        0      308 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/_base.py
--rw-r--r--   0        0        0    14015 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/_early_stopping_callback.py
--rw-r--r--   0        0        0     4387 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/_tqdm_callback.py
--rw-r--r--   0        0        0        0 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/py.typed
--rw-r--r--   0        0        0      362 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/_base.py
--rw-r--r--   0        0        0     3430 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/_dart_early_stopping_wrapper.py
--rw-r--r--   0        0        0    14790 2023-05-18 13:19:52.413314 lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/_early_stopping.py
--rw-r--r--   0        0        0     8802 1970-01-01 00:00:00.000000 lightgbm_callbacks-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-05-18 13:54:01.109009 lightgbm_callbacks-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7542 2023-05-18 13:54:01.109009 lightgbm_callbacks-0.1.1/README.md
+-rw-r--r--   0        0        0     2477 2023-05-18 13:54:02.337083 lightgbm_callbacks-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      614 2023-05-18 13:54:02.261078 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/_base.py
+-rw-r--r--   0        0        0    14015 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/_early_stopping_callback.py
+-rw-r--r--   0        0        0     4387 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/_tqdm_callback.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/py.typed
+-rw-r--r--   0        0        0      362 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/_base.py
+-rw-r--r--   0        0        0     3430 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/_dart_early_stopping_wrapper.py
+-rw-r--r--   0        0        0    14790 2023-05-18 13:54:01.113010 lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/_early_stopping.py
+-rw-r--r--   0        0        0     8802 1970-01-01 00:00:00.000000 lightgbm_callbacks-0.1.1/PKG-INFO
```

### Comparing `lightgbm_callbacks-0.1.0/LICENSE` & `lightgbm_callbacks-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightgbm_callbacks-0.1.0/README.md` & `lightgbm_callbacks-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lightgbm_callbacks-0.1.0/pyproject.toml` & `lightgbm_callbacks-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightgbm-callbacks"
-version = "0.1.0"
+version = "0.1.1"
 description = "A collection of LightGBM callbacks."
 authors = ["34j <34j.95a2p@simplelogin.com>", "Microsoft Corporation"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/lightgbm-callbacks"
 documentation = "https://lightgbm-callbacks.readthedocs.io"
 classifiers = [
```

### Comparing `lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/__init__.py` & `lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 from ._base import CallbackBase
 from ._early_stopping_callback import DartEarlyStoppingCallback, EarlyStoppingCallback
 from ._tqdm_callback import ProgressBarCallback
 from .sklearn import (
     EstimatorWrapperBase,
     LGBMDartEarlyStoppingEstimator,
     LGBMDartEarlyStoppingSimpleWrapper,
```

### Comparing `lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/_early_stopping_callback.py` & `lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/_early_stopping_callback.py`

 * *Files identical despite different names*

### Comparing `lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/_tqdm_callback.py` & `lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/_tqdm_callback.py`

 * *Files identical despite different names*

### Comparing `lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/_base.py` & `lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     def __getitem__(self, __key: str) -> Any:
         return self.estimator.__getitem__(__key)
 
     # Due to the bug in Python, __instancecheck__ does not work.
     # https://bugs.python.org/issue35083
 
-    @property
+    # This makes the class sklearn.clone() incompatible.
+    """@property
     def __class__(self) -> Any:
         return self.estimator.__class__
 
     @__class__.setter
     def __class__(self, __class__: Any) -> None:  # noqa
-        self.estimator.__class__ = __class__
+        self.estimator.__class__ = __class__"""
```

### Comparing `lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/_dart_early_stopping_wrapper.py` & `lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/_dart_early_stopping_wrapper.py`

 * *Files identical despite different names*

### Comparing `lightgbm_callbacks-0.1.0/src/lightgbm_callbacks/sklearn/_early_stopping.py` & `lightgbm_callbacks-0.1.1/src/lightgbm_callbacks/sklearn/_early_stopping.py`

 * *Files identical despite different names*

### Comparing `lightgbm_callbacks-0.1.0/PKG-INFO` & `lightgbm_callbacks-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightgbm-callbacks
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of LightGBM callbacks.
 Home-page: https://github.com/34j/lightgbm-callbacks
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightgbm-callbacks Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: lightgbm-callbacks Version: 0.1.1 Summary: A
 collection of LightGBM callbacks. Home-page: https://github.com/34j/lightgbm-
 callbacks License: MIT Author: 34j Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

