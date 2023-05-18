# Comparing `tmp/forager-toolkit-1.0.2.tar.gz` & `tmp/forager-toolkit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forager-toolkit-1.0.2.tar", last modified: Thu May 18 00:27:39 2023, max compression
+gzip compressed data, was "forager-toolkit-1.0.3.tar", last modified: Thu May 18 03:15:29 2023, max compression
```

## Comparing `forager-toolkit-1.0.2.tar` & `forager-toolkit-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:27:39.040596 forager-toolkit-1.0.2/
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1072 2023-05-10 00:39:29.000000 forager-toolkit-1.0.2/LICENSE.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-18 00:27:39.040911 forager-toolkit-1.0.2/PKG-INFO
--rw-r--r--   0 mkapoor1   (503) staff       (20)      157 2023-05-10 00:38:51.000000 forager-toolkit-1.0.2/README.md
--rw-r--r--   0 mkapoor1   (503) staff       (20)       85 2023-05-10 00:47:14.000000 forager-toolkit-1.0.2/pyproject.toml
--rw-r--r--   0 mkapoor1   (503) staff       (20)      703 2023-05-18 00:27:39.042927 forager-toolkit-1.0.2/setup.cfg
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1135 2023-05-18 00:27:06.000000 forager-toolkit-1.0.2/setup.py
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:27:39.020276 forager-toolkit-1.0.2/src/
--rw-r--r--   0 mkapoor1   (503) staff       (20)    13222 2023-05-18 00:23:14.000000 forager-toolkit-1.0.2/src/forager.py
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:27:39.029168 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/
--rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-18 00:27:38.000000 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 mkapoor1   (503) staff       (20)      534 2023-05-18 00:27:39.000000 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)        1 2023-05-18 00:27:38.000000 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)       41 2023-05-18 00:27:38.000000 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)       16 2023-05-18 00:27:38.000000 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/requires.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)       20 2023-05-18 00:27:38.000000 forager-toolkit-1.0.2/src/forager_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:27:39.036069 forager-toolkit-1.0.2/src/models/
--rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:51.000000 forager-toolkit-1.0.2/src/models/__init__.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1584 2023-03-21 20:33:03.000000 forager-toolkit-1.0.2/src/models/alpine.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     9539 2023-04-15 20:50:16.000000 forager-toolkit-1.0.2/src/models/date.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     5198 2023-04-08 15:54:11.000000 forager-toolkit-1.0.2/src/models/hashforest.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     5915 2023-04-15 21:54:41.000000 forager-toolkit-1.0.2/src/models/maple.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1494 2023-03-21 20:51:09.000000 forager-toolkit-1.0.2/src/models/palm.py
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:27:39.039701 forager-toolkit-1.0.2/src/util/
--rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:45.000000 forager-toolkit-1.0.2/src/util/__init__.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     8668 2022-10-28 17:05:42.000000 forager-toolkit-1.0.2/src/util/parser.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     6182 2022-10-28 17:15:02.000000 forager-toolkit-1.0.2/src/util/payload.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     4563 2022-12-08 11:28:02.000000 forager-toolkit-1.0.2/src/util/test.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 03:15:29.631482 forager-toolkit-1.0.3/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1072 2023-05-10 00:39:29.000000 forager-toolkit-1.0.3/LICENSE.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-18 03:15:29.631789 forager-toolkit-1.0.3/PKG-INFO
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      157 2023-05-10 00:38:51.000000 forager-toolkit-1.0.3/README.md
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       85 2023-05-10 00:47:14.000000 forager-toolkit-1.0.3/pyproject.toml
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      703 2023-05-18 03:15:29.633302 forager-toolkit-1.0.3/setup.cfg
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1135 2023-05-18 03:13:53.000000 forager-toolkit-1.0.3/setup.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 03:15:29.534822 forager-toolkit-1.0.3/src/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)    13171 2023-05-18 03:13:20.000000 forager-toolkit-1.0.3/src/forager.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 03:15:29.547716 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-18 03:15:29.000000 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      534 2023-05-18 03:15:29.000000 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)        1 2023-05-18 03:15:29.000000 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       41 2023-05-18 03:15:29.000000 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       16 2023-05-18 03:15:29.000000 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/requires.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       20 2023-05-18 03:15:29.000000 forager-toolkit-1.0.3/src/forager_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 03:15:29.586293 forager-toolkit-1.0.3/src/models/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:51.000000 forager-toolkit-1.0.3/src/models/__init__.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1584 2023-03-21 20:33:03.000000 forager-toolkit-1.0.3/src/models/alpine.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     9539 2023-05-18 00:45:27.000000 forager-toolkit-1.0.3/src/models/date.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     5363 2023-05-18 03:13:10.000000 forager-toolkit-1.0.3/src/models/hashforest.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     5903 2023-05-18 03:06:33.000000 forager-toolkit-1.0.3/src/models/maple.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1491 2023-05-18 01:46:08.000000 forager-toolkit-1.0.3/src/models/palm.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 03:15:29.622553 forager-toolkit-1.0.3/src/util/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:45.000000 forager-toolkit-1.0.3/src/util/__init__.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     8668 2022-10-28 17:05:42.000000 forager-toolkit-1.0.3/src/util/parser.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     6182 2022-10-28 17:15:02.000000 forager-toolkit-1.0.3/src/util/payload.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     4563 2022-12-08 11:28:02.000000 forager-toolkit-1.0.3/src/util/test.py
```

### Comparing `forager-toolkit-1.0.2/LICENSE.txt` & `forager-toolkit-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.2/PKG-INFO` & `forager-toolkit-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forager-toolkit
-Version: 1.0.2
+Version: 1.0.3
 Summary: A network traffic classification toolkit
 Home-page: https://github.com/mayakapoor/forager
 Author: Maya Kapoor
 Author-email: mkapoor1@uncc.edu
 Project-URL: Bug Tracker, https://github.com/mayakapoor/forager/issues
 Project-URL: Documentation, https://forager-toolkit.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `forager-toolkit-1.0.2/setup.cfg` & `forager-toolkit-1.0.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forager-toolkit
-version = 1.0.2
+version = 1.0.3
 author = Maya Kapoor
 author_email = mkapoor1@uncc.edu
 description = A network traffic classification toolkit
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mayakapoor/forager
 project_urls =
```

### Comparing `forager-toolkit-1.0.2/setup.py` & `forager-toolkit-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "forager-toolkit",
-    version = "1.0.2",
+    version = "1.0.3",
     author = "Maya Kapoor",
     author_email = "mkapoor1@uncc.edu",
     description = "A network traffic classification toolkit",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mayakapoor/forager",
     project_urls = {
```

### Comparing `forager-toolkit-1.0.2/src/forager.py` & `forager-toolkit-1.0.3/src/forager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pylibmagic
 import magic
 import pickle
 import numpy as np
 from pick import pick
 from pandas import read_csv, concat, DataFrame
 from sklearn.preprocessing import OneHotEncoder
+from statistics import mode
 import models.alpine as ALPINE
 import models.palm as PALM
 import models.maple as MAPLE
 import models.date as DATE
 
 import rexactor
 import tapcap
@@ -30,23 +31,20 @@
 maple_json = maple_cache + "/maple.json"
 maple_labels = maple_cache + "/labels.txt"
 date_h5 = date_cache + "/date.h5"
 date_json = date_cache + "/date.json"
 date_labels = date_cache + "/labels.txt"
 
 def vote(voters):
-    joined = voters[0]
-    for i in range(1, len(voters)-1):
-        joined = np.concatenate((joined, voters[i]), axis=1)
+    joined = np.array([np.array(v) for v in voters[0]])
+    for i in range (1, len(voters)-1):
+        joined = np.column_stack((joined, np.array([np.array(v) for v in voters[i]])))
     ballot = []
     for votes in joined:
-        if not isinstance(votes, list):
-            ballot.append(max(set(votes), key=votes.tolist().count))
-        else:
-            ballot.append(max(set(votes), key=votes.count))
+        ballot.append(mode(votes.tolist()))
     return ballot
 
 def main():
     if not os.path.exists(root_cache):
         os.makedirs(root_cache)
     if not os.path.exists(results_cache):
         os.makedirs(results_cache)
```

### Comparing `forager-toolkit-1.0.2/src/forager_toolkit.egg-info/PKG-INFO` & `forager-toolkit-1.0.3/src/forager_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forager-toolkit
-Version: 1.0.2
+Version: 1.0.3
 Summary: A network traffic classification toolkit
 Home-page: https://github.com/mayakapoor/forager
 Author: Maya Kapoor
 Author-email: mkapoor1@uncc.edu
 Project-URL: Bug Tracker, https://github.com/mayakapoor/forager/issues
 Project-URL: Documentation, https://forager-toolkit.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `forager-toolkit-1.0.2/src/forager_toolkit.egg-info/SOURCES.txt` & `forager-toolkit-1.0.3/src/forager_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.2/src/models/alpine.py` & `forager-toolkit-1.0.3/src/models/alpine.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.2/src/models/date.py` & `forager-toolkit-1.0.3/src/models/date.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.2/src/models/hashforest.py` & `forager-toolkit-1.0.3/src/models/hashforest.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,18 +140,23 @@
 
         Return:
             a list of lists where each list is the forests' votes for a sample from the input data
         """
         data = self._process_data(data)
         minhashes = self.hash(data)
         all_arrs = []
+        first = True
         for m in minhashes:
             arr = np.array(self.my_forest.query(m, self.my_num_votes))
             lookup_results = []
             for ret in arr:
                 lookup_results.append(self.my_lookup_table[ret])
-            if len(lookup_results) == 0:
+
+            if len(lookup_results) < self.my_num_votes:
+                remain = self.my_num_votes - len(lookup_results)
                 #print("WARNING: no close proximity match found. Using random result")
                 choice = random.choice(range(0, len(self.my_lookup_table)))
-                lookup_results.append(self.my_lookup_table[choice])
+                supplement = [self.my_lookup_table[choice]] * remain
+                lookup_results = lookup_results + supplement
+
             all_arrs.append(lookup_results)
         return all_arrs
```

### Comparing `forager-toolkit-1.0.2/src/models/maple.py` & `forager-toolkit-1.0.3/src/models/maple.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             dense1 = keras.layers.Dense(64, activation = 'relu')(flatten)
             drop = keras.layers.Dropout(.2)(dense1)
             dense2 = keras.layers.Dense(32, activation = 'relu')(drop)
             drop2 = keras.layers.Dropout(.2)(dense2)
             output = keras.layers.Dense(len(self.labels), activation = 'softmax')(drop2)
             maple = keras.Model(inputs,output)
             return maple
-            
+
         if (self.use_existing and os.path.exists(self.weights_path) and os.path.exists(self.json_path)):
             json_file = open(self.json_path, 'r')
             loaded_model_json = json_file.read()
             json_file.close()
             maple = model_from_json(loaded_model_json)
             maple.load_weights(self.weights_path)
             print("Using existing model at " + str(self.json_path) + ".")
```

### Comparing `forager-toolkit-1.0.2/src/models/palm.py` & `forager-toolkit-1.0.3/src/models/palm.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from datasketch import MinHash
 
 class Palm(HashForest):
     """
     Classifies packets based on a hash of the payload.
     """
-    def __init__(self, hash="sha1", col_name="payload"):
+    def __init__(self, hash="sha1", col_name="text"):
         """
         Initialize the PALM model.
 
         Args:
             hash     optional parameter to change the hash type, can be xxhash, farmhash, or mm3hash
             col_name the name of the column containing the text payload
         """
```

### Comparing `forager-toolkit-1.0.2/src/util/parser.py` & `forager-toolkit-1.0.3/src/util/parser.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.2/src/util/payload.py` & `forager-toolkit-1.0.3/src/util/payload.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.2/src/util/test.py` & `forager-toolkit-1.0.3/src/util/test.py`

 * *Files identical despite different names*

