# Comparing `tmp/forager-toolkit-1.0.0.tar.gz` & `tmp/forager-toolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forager-toolkit-1.0.0.tar", last modified: Sun May 14 20:43:43 2023, max compression
+gzip compressed data, was "forager-toolkit-1.0.1.tar", last modified: Thu May 18 00:20:58 2023, max compression
```

## Comparing `forager-toolkit-1.0.0.tar` & `forager-toolkit-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-14 20:43:43.693283 forager-toolkit-1.0.0/
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1072 2023-05-10 00:39:29.000000 forager-toolkit-1.0.0/LICENSE.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-14 20:43:43.693584 forager-toolkit-1.0.0/PKG-INFO
--rw-r--r--   0 mkapoor1   (503) staff       (20)      157 2023-05-10 00:38:51.000000 forager-toolkit-1.0.0/README.md
--rw-r--r--   0 mkapoor1   (503) staff       (20)       85 2023-05-10 00:47:14.000000 forager-toolkit-1.0.0/pyproject.toml
--rw-r--r--   0 mkapoor1   (503) staff       (20)      703 2023-05-14 20:43:43.695331 forager-toolkit-1.0.0/setup.cfg
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1135 2023-05-14 20:43:13.000000 forager-toolkit-1.0.0/setup.py
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-14 20:43:43.674432 forager-toolkit-1.0.0/src/
--rw-r--r--   0 mkapoor1   (503) staff       (20)    13125 2023-05-14 20:42:22.000000 forager-toolkit-1.0.0/src/forager.py
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-14 20:43:43.683407 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/
--rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-14 20:43:43.000000 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 mkapoor1   (503) staff       (20)      534 2023-05-14 20:43:43.000000 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)        1 2023-05-14 20:43:43.000000 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)       41 2023-05-14 20:43:43.000000 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)       16 2023-05-14 20:43:43.000000 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/requires.txt
--rw-r--r--   0 mkapoor1   (503) staff       (20)       20 2023-05-14 20:43:43.000000 forager-toolkit-1.0.0/src/forager_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-14 20:43:43.689237 forager-toolkit-1.0.0/src/models/
--rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:51.000000 forager-toolkit-1.0.0/src/models/__init__.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1584 2023-03-21 20:33:03.000000 forager-toolkit-1.0.0/src/models/alpine.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     9539 2023-04-15 20:50:16.000000 forager-toolkit-1.0.0/src/models/date.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     5198 2023-04-08 15:54:11.000000 forager-toolkit-1.0.0/src/models/hashforest.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     5915 2023-04-15 21:54:41.000000 forager-toolkit-1.0.0/src/models/maple.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     1494 2023-03-21 20:51:09.000000 forager-toolkit-1.0.0/src/models/palm.py
-drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-14 20:43:43.692621 forager-toolkit-1.0.0/src/util/
--rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:45.000000 forager-toolkit-1.0.0/src/util/__init__.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     8668 2022-10-28 17:05:42.000000 forager-toolkit-1.0.0/src/util/parser.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     6182 2022-10-28 17:15:02.000000 forager-toolkit-1.0.0/src/util/payload.py
--rw-r--r--   0 mkapoor1   (503) staff       (20)     4563 2022-12-08 11:28:02.000000 forager-toolkit-1.0.0/src/util/test.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:20:58.166705 forager-toolkit-1.0.1/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1072 2023-05-10 00:39:29.000000 forager-toolkit-1.0.1/LICENSE.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-18 00:20:58.166997 forager-toolkit-1.0.1/PKG-INFO
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      157 2023-05-10 00:38:51.000000 forager-toolkit-1.0.1/README.md
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       85 2023-05-10 00:47:14.000000 forager-toolkit-1.0.1/pyproject.toml
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      703 2023-05-18 00:20:58.168605 forager-toolkit-1.0.1/setup.cfg
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1135 2023-05-18 00:20:38.000000 forager-toolkit-1.0.1/setup.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:20:58.139424 forager-toolkit-1.0.1/src/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)    13243 2023-05-18 00:16:51.000000 forager-toolkit-1.0.1/src/forager.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:20:58.146876 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      752 2023-05-18 00:20:58.000000 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 mkapoor1   (503) staff       (20)      534 2023-05-18 00:20:58.000000 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)        1 2023-05-18 00:20:58.000000 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       41 2023-05-18 00:20:58.000000 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       16 2023-05-18 00:20:58.000000 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/requires.txt
+-rw-r--r--   0 mkapoor1   (503) staff       (20)       20 2023-05-18 00:20:58.000000 forager-toolkit-1.0.1/src/forager_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:20:58.159251 forager-toolkit-1.0.1/src/models/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:51.000000 forager-toolkit-1.0.1/src/models/__init__.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1584 2023-03-21 20:33:03.000000 forager-toolkit-1.0.1/src/models/alpine.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     9539 2023-04-15 20:50:16.000000 forager-toolkit-1.0.1/src/models/date.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     5198 2023-04-08 15:54:11.000000 forager-toolkit-1.0.1/src/models/hashforest.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     5915 2023-04-15 21:54:41.000000 forager-toolkit-1.0.1/src/models/maple.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     1494 2023-03-21 20:51:09.000000 forager-toolkit-1.0.1/src/models/palm.py
+drwxr-xr-x   0 mkapoor1   (503) staff       (20)        0 2023-05-18 00:20:58.165354 forager-toolkit-1.0.1/src/util/
+-rw-r--r--   0 mkapoor1   (503) staff       (20)        0 2022-10-22 01:23:45.000000 forager-toolkit-1.0.1/src/util/__init__.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     8668 2022-10-28 17:05:42.000000 forager-toolkit-1.0.1/src/util/parser.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     6182 2022-10-28 17:15:02.000000 forager-toolkit-1.0.1/src/util/payload.py
+-rw-r--r--   0 mkapoor1   (503) staff       (20)     4563 2022-12-08 11:28:02.000000 forager-toolkit-1.0.1/src/util/test.py
```

### Comparing `forager-toolkit-1.0.0/LICENSE.txt` & `forager-toolkit-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/PKG-INFO` & `forager-toolkit-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forager-toolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A network traffic classification toolkit
 Home-page: https://github.com/mayakapoor/forager
 Author: Maya Kapoor
 Author-email: mkapoor1@uncc.edu
 Project-URL: Bug Tracker, https://github.com/mayakapoor/forager/issues
 Project-URL: Documentation, https://forager-toolkit.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `forager-toolkit-1.0.0/setup.cfg` & `forager-toolkit-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forager-toolkit
-version = 1.0.0
+version = 1.0.1
 author = Maya Kapoor
 author_email = mkapoor1@uncc.edu
 description = A network traffic classification toolkit
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mayakapoor/forager
 project_urls =
```

### Comparing `forager-toolkit-1.0.0/setup.py` & `forager-toolkit-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "forager-toolkit",
-    version = "1.0.0",
+    version = "1.0.1",
     author = "Maya Kapoor",
     author_email = "mkapoor1@uncc.edu",
     description = "A network traffic classification toolkit",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/mayakapoor/forager",
     project_urls = {
```

### Comparing `forager-toolkit-1.0.0/src/forager.py` & `forager-toolkit-1.0.1/src/forager.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,18 @@
 
 def vote(voters):
     joined = voters[0]
     for i in range(1, len(voters)-1):
         joined = np.concatenate((joined, voters[i]), axis=1)
     ballot = []
     for votes in joined:
-        ballot.append(max(set(votes), key=votes.tolist().count))
+        if not isinstance(votes, list):
+            ballot.append(max(set(votes), key=votes.tolist().count))
+        else:
+            ballot.append(max(set(votes), key=votes.count))
     return ballot
 
 def main():
     if not os.path.exists(root_cache):
         os.makedirs(root_cache)
     if not os.path.exists(results_cache):
         os.makedirs(results_cache)
```

### Comparing `forager-toolkit-1.0.0/src/forager_toolkit.egg-info/PKG-INFO` & `forager-toolkit-1.0.1/src/forager_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forager-toolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A network traffic classification toolkit
 Home-page: https://github.com/mayakapoor/forager
 Author: Maya Kapoor
 Author-email: mkapoor1@uncc.edu
 Project-URL: Bug Tracker, https://github.com/mayakapoor/forager/issues
 Project-URL: Documentation, https://forager-toolkit.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `forager-toolkit-1.0.0/src/forager_toolkit.egg-info/SOURCES.txt` & `forager-toolkit-1.0.1/src/forager_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/models/alpine.py` & `forager-toolkit-1.0.1/src/models/alpine.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/models/date.py` & `forager-toolkit-1.0.1/src/models/date.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/models/hashforest.py` & `forager-toolkit-1.0.1/src/models/hashforest.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/models/maple.py` & `forager-toolkit-1.0.1/src/models/maple.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/models/palm.py` & `forager-toolkit-1.0.1/src/models/palm.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/util/parser.py` & `forager-toolkit-1.0.1/src/util/parser.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/util/payload.py` & `forager-toolkit-1.0.1/src/util/payload.py`

 * *Files identical despite different names*

### Comparing `forager-toolkit-1.0.0/src/util/test.py` & `forager-toolkit-1.0.1/src/util/test.py`

 * *Files identical despite different names*

