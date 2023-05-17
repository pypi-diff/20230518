# Comparing `tmp/rai_test_utils-0.1.0.tar.gz` & `tmp/rai_test_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rai_test_utils-0.1.0.tar", last modified: Wed Feb  8 23:14:47 2023, max compression
+gzip compressed data, was "dist/rai_test_utils-0.2.0.tar", last modified: Wed May 17 22:20:03 2023, max compression
```

## Comparing `rai_test_utils-0.1.0.tar` & `rai_test_utils-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/datasets/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/datasets/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/datasets/tabular/tabular_data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/models/lightgbm/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/lightgbm/lightgbm_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/models/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/sklearn/sklearn_model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/models/xgboost/xgboost_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/rai_test_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/rai_test_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:14:47.000000 rai_test_utils-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-08 23:14:05.000000 rai_test_utils-0.1.0/tests/test_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/tabular_data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/lightgbm/lightgbm_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/sklearn/sklearn_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/models/xgboost/xgboost_model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/rai_test_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/rai_test_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:20:03.000000 rai_test_utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/tests/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-17 22:19:19.000000 rai_test_utils-0.2.0/tests/test_utils.py
```

### Comparing `rai_test_utils-0.1.0/LICENSE` & `rai_test_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.1.0/PKG-INFO` & `rai_test_utils-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: rai_test_utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common basic test utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Gaurav Gupta
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Responsible AI test utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
 
 The Responsible AI Test Utilities package contains common testing utilities and functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets, ml-wrappers and other packages.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `rai_test_utils-0.1.0/rai_test_utils/datasets/tabular/__init__.py` & `rai_test_utils-0.2.0/rai_test_utils/datasets/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.1.0/rai_test_utils/models/sklearn/__init__.py` & `rai_test_utils-0.2.0/rai_test_utils/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.1.0/rai_test_utils.egg-info/PKG-INFO` & `rai_test_utils-0.2.0/rai_test_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: rai-test-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common basic test utilities used across various RAI tools
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Gaurav Gupta
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Responsible AI test utilities for Python
 
-### This package has been tested with Python 3.6, 3.7, 3.8 and 3.9
+### This package has been tested with Python 3.6, 3.7, 3.8, 3.9 and 3.10
 
 The Responsible AI Test Utilities package contains common testing utilities and functions shared across various RAI tools, including fairlearn, interpret-community, responsibleai, raiwidgets, ml-wrappers and other packages.
 
 Please see the main documentation website:
 https://responsibleaitoolbox.ai/
 
 The open source code can be found here:
```

### Comparing `rai_test_utils-0.1.0/rai_test_utils.egg-info/SOURCES.txt` & `rai_test_utils-0.2.0/rai_test_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,9 +17,12 @@
 rai_test_utils/models/model_utils.py
 rai_test_utils/models/lightgbm/__init__.py
 rai_test_utils/models/lightgbm/lightgbm_model_utils.py
 rai_test_utils/models/sklearn/__init__.py
 rai_test_utils/models/sklearn/sklearn_model_utils.py
 rai_test_utils/models/xgboost/__init__.py
 rai_test_utils/models/xgboost/xgboost_model_utils.py
+rai_test_utils/utilities/__init__.py
+rai_test_utils/utilities/utils.py
 tests/test_data_utils.py
-tests/test_model_utils.py
+tests/test_model_utils.py
+tests/test_utils.py
```

### Comparing `rai_test_utils-0.1.0/setup.py` & `rai_test_utils-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,13 @@
     python_requires='>=3.6',
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha"
     ]
 )
```

### Comparing `rai_test_utils-0.1.0/tests/test_data_utils.py` & `rai_test_utils-0.2.0/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `rai_test_utils-0.1.0/tests/test_model_utils.py` & `rai_test_utils-0.2.0/tests/test_model_utils.py`

 * *Files identical despite different names*

