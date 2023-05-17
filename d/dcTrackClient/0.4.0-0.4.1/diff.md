# Comparing `tmp/dctrackclient-0.4.0.tar.gz` & `tmp/dctrackclient-0.4.1.tar.gz`

## Comparing `dctrackclient-0.4.0.tar` & `dctrackclient-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.4.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.4.0/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 dctrackclient-0.4.0/../README.md
--rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 dctrackclient-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.4.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.4.1/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 dctrackclient-0.4.1/../README.md
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 dctrackclient-0.4.1/PKG-INFO
```

### Comparing `dctrackclient-0.4.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.4.1/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.4.0/pyproject.toml` & `dctrackclient-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.4.0/../README.md` & `dctrackclient-0.4.1/../README.md`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.4.0/PKG-INFO` & `dctrackclient-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.4.0
+Version: 0.4.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

