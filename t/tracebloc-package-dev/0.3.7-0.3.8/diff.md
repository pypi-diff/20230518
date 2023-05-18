# Comparing `tmp/tracebloc_package-dev-0.3.7.tar.gz` & `tmp/tracebloc_package-dev-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.3.7.tar", last modified: Thu May 18 06:01:48 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.3.8.tar", last modified: Thu May 18 06:24:20 2023, max compression
```

## Comparing `tracebloc_package-dev-0.3.7.tar` & `tracebloc_package-dev-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:01:48.668061 tracebloc_package-dev-0.3.7/
--rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.7/LICENSE.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:01:48.668177 tracebloc_package-dev-0.3.7/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.7/README.md
--rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-18 06:01:48.668558 tracebloc_package-dev-0.3.7/setup.cfg
--rw-r--r--   0 divyasingh   (501) staff       (20)      859 2023-05-18 06:01:04.000000 tracebloc_package-dev-0.3.7/setup.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:01:48.666620 tracebloc_package-dev-0.3.7/tracebloc_package/
--rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/__init__.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     5697 2023-03-23 06:34:00.000000 tracebloc_package-dev-0.3.7/tracebloc_package/check_parameters.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    16788 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/functional_test.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    53398 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.3.7/tracebloc_package/messages.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     7029 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/upload.py
--rw-r--r--   0 divyasingh   (501) staff       (20)    10062 2023-03-29 10:34:00.000000 tracebloc_package-dev-0.3.7/tracebloc_package/user.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3832 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.7/tracebloc_package/utils.py
--rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.3.7/tracebloc_package/weights.py
-drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:01:48.667877 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/
--rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 divyasingh   (501) staff       (20)       73 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-18 06:01:48.000000 tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:24:20.633715 tracebloc_package-dev-0.3.8/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.8/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:24:20.633804 tracebloc_package-dev-0.3.8/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.3.8/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-05-18 06:24:20.634100 tracebloc_package-dev-0.3.8/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      859 2023-05-18 06:21:30.000000 tracebloc_package-dev-0.3.8/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:24:20.632388 tracebloc_package-dev-0.3.8/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-03-16 07:45:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5697 2023-03-23 06:34:00.000000 tracebloc_package-dev-0.3.8/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    16788 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    53410 2023-05-18 06:21:00.000000 tracebloc_package-dev-0.3.8/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.3.8/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7029 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10064 2023-05-18 06:23:40.000000 tracebloc_package-dev-0.3.8/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3832 2023-05-18 06:00:22.000000 tracebloc_package-dev-0.3.8/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3203 2022-06-09 14:39:28.000000 tracebloc_package-dev-0.3.8/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-05-18 06:24:20.633559 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)       73 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-05-18 06:24:20.000000 tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.3.7/LICENSE.txt` & `tracebloc_package-dev-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/PKG-INFO` & `tracebloc_package-dev-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.3.7
+Version: 0.3.8
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.3.7/setup.py` & `tracebloc_package-dev-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.3.7",
+    version="0.3.8",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             else:
                 checkeligible = False
                 error_msg = "trainingDatasetSize dictionary must contain all classes that are present in the dataset. Customisation in terms of classes is not allowed."
                 self.__print_error(error_msg)
         if checkeligible:
             self.__trainingClasses = training_dataset
             self.__trainingDatasetSize = getImagesCount(training_dataset)
-            self.__subdataset = {"trainingDatasetSize": self.__trainingDatasetSize, "trainingClasses": self.__trainingClasses}
+            self.__subdataset = json.dumps({"trainingDatasetSize": self.__trainingDatasetSize, "trainingClasses": self.__trainingClasses})
             self.__remove_error_method()
             # recalculate the validation split
             header = {"Authorization": f"Token {self.__token}"}
             data = {
                 "edges_involved": json.dumps(list(self.__total_images.keys())),
                 "images_per_class": json.dumps(training_dataset),
                 "type": "recalculate_image_count_per_edge",
```

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/messages.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/upload.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/user.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             self.__model = modelobj.model
             if self.__modelId == "" or self.__modelId is None:
                 text = colored(f"'{self.__modelName}' upload Failed.", "red")
                 print(text, "\n")
                 self.__weights = False
                 return
             else:
-                text = colored(f"'{self.__modelName}' upload successful.", "green")
+                text = colored(f"\n'{self.__modelName}' upload successful.", "green")
                 print(text, "\n")
 
         except:
             return
 
     def linkModelDataset(self, datasetId: str):
```

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/utils.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package/weights.py` & `tracebloc_package-dev-0.3.8/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.3.7
+Version: 0.3.8
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tracebloc_package-dev-0.3.7/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.3.8/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

