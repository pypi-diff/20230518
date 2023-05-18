# Comparing `tmp/tracebloc_package-dev-0.3.6.tar.gz` & `tmp/tracebloc_package-dev-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.3.6.tar", last modified: Fri Apr 14 07:24:26 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.3.7.tar", last modified: Thu May 18 06:01:48 2023, max compression
```

## Comparing `tracebloc_package-dev-0.3.6.tar` & `tracebloc_package-dev-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-04-14 07:24:26.918223 tracebloc_package-dev-0.3.6/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.3.6/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-04-14 07:24:26.918519 tracebloc_package-dev-0.3.6/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.3.6/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-04-14 07:24:26.919491 tracebloc_package-dev-0.3.6/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      859 2023-04-14 07:23:43.000000 tracebloc_package-dev-0.3.6/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-04-14 07:24:26.916744 tracebloc_package-dev-0.3.6/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.3.6/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5697 2023-03-20 10:56:57.000000 tracebloc_package-dev-0.3.6/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    16788 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.6/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    53195 2023-04-14 07:22:52.000000 tracebloc_package-dev-0.3.6/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.3.6/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)     7029 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.6/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10062 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.6/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     3832 2023-03-20 08:05:24.000000 tracebloc_package-dev-0.3.6/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.3.6/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-04-14 07:24:26.918048 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)       73 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:01:48.668061 tracebloc_package-dev-0.3.7/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.7/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:01:48.668177 tracebloc_package-dev-0.3.7/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.7/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-18 06:01:48.668558 tracebloc_package-dev-0.3.7/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      859 2023-05-18 06:01:04.000000 tracebloc_package-dev-0.3.7/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:01:48.666620 tracebloc_package-dev-0.3.7/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5697 2023-03-23 06:34:00.000000 tracebloc_package-dev-0.3.7/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    16788 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    53398 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.3.7/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7029 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10062 2023-03-29 10:34:00.000000 tracebloc_package-dev-0.3.7/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3832 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.3.7/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:01:48.667877 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)       73 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.3.6/LICENSE.txt` & `tracebloc_package-dev-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/PKG-INFO` & `tracebloc_package-dev-0.3.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.3.6/setup.py` & `tracebloc_package-dev-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.3.6",
+    version="0.3.7",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         self.__model = model
         self.__image_shape = 224
         self.__image_type = "rgb"
         self.__optimizer = "sgd"
         self.__totalDatasetSize = totalDatasetSize
         self.__trainingDatasetSize = totalDatasetSize
         self.__trainingClasses = class_names
+        self.__subdataset = {}
         self.__lossFunction = {TYPE: STANDARD, VALUE: "categorical_crossentropy"}
         self.__learningRate = {TYPE: CONSTANT, VALUE: 0.001}
         self.__seed = False
         self.__total_images = total_images
         self.__num_classes = num_classes
         self.__class_names = class_names
         self.__batchSize = self.__default_batchSize()
@@ -195,14 +196,15 @@
             else:
                 checkeligible = False
                 error_msg = "trainingDatasetSize dictionary must contain all classes that are present in the dataset. Customisation in terms of classes is not allowed."
                 self.__print_error(error_msg)
         if checkeligible:
             self.__trainingClasses = training_dataset
             self.__trainingDatasetSize = getImagesCount(training_dataset)
+            self.__subdataset = {"trainingDatasetSize": self.__trainingDatasetSize, "trainingClasses": self.__trainingClasses}
             self.__remove_error_method()
             # recalculate the validation split
             header = {"Authorization": f"Token {self.__token}"}
             data = {
                 "edges_involved": json.dumps(list(self.__total_images.keys())),
                 "images_per_class": json.dumps(training_dataset),
                 "type": "recalculate_image_count_per_edge",
@@ -1288,14 +1290,15 @@
             "objective": self.__objective,
             "name": self.__name,
             "modelType": self.__modelType,
             "category": self.__category,
             "upperboundTime": self.__upperboundTime,
             "callbacks": self.__callbacks,
             "pre_trained_weights": self.__weights,
+            "subdataset": self.__subdataset,
             "images_per_class": self.__images_per_class,
             "image_shape": self.__image_shape,
             "image_type": self.__image_type,
         }
 
         return parameters
```

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/messages.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/upload.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/user.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/utils.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package/weights.py` & `tracebloc_package-dev-0.3.7/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

