# Comparing `tmp/notebook-doc-0.2.0.tar.gz` & `tmp/notebook-doc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook-doc-0.2.0.tar", last modified: Mon Apr 17 12:07:20 2023, max compression
+gzip compressed data, was "notebook-doc-0.2.1.tar", last modified: Thu May 18 11:37:06 2023, max compression
```

## Comparing `notebook-doc-0.2.0.tar` & `notebook-doc-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/
--rw-rw-rw-   0        0        0     1089 2023-03-20 12:16:45.000000 notebook-doc-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2037 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1459 2023-03-21 13:48:14.000000 notebook-doc-0.2.0/README.md
--rw-rw-rw-   0        0        0     1186 2023-04-17 12:04:44.000000 notebook-doc-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.021616 notebook-doc-0.2.0/src/
--rw-rw-rw-   0        0        0       53 2023-04-17 12:04:44.000000 notebook-doc-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.033024 notebook-doc-0.2.0/src/notebook_doc/
--rw-rw-rw-   0        0        0       88 2023-04-17 12:04:44.000000 notebook-doc-0.2.0/src/notebook_doc/__init__.py
--rw-rw-rw-   0        0        0    14834 2023-04-17 11:55:40.000000 notebook-doc-0.2.0/src/notebook_doc/doc_functions.py
--rw-rw-rw-   0        0        0     4827 2023-03-24 10:22:31.000000 notebook-doc-0.2.0/src/notebook_doc/test.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/src/notebook_doc.egg-info/
--rw-rw-rw-   0        0        0     2037 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 11:37:06.863416 notebook-doc-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2023-03-20 12:16:45.000000 notebook-doc-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2037 2023-05-18 11:37:06.859696 notebook-doc-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1459 2023-03-21 13:48:14.000000 notebook-doc-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1186 2023-05-18 11:35:01.000000 notebook-doc-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 11:37:06.863416 notebook-doc-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 11:37:06.682330 notebook-doc-0.2.1/src/
+-rw-rw-rw-   0        0        0       53 2023-05-18 11:35:01.000000 notebook-doc-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:37:06.693067 notebook-doc-0.2.1/src/notebook_doc/
+-rw-rw-rw-   0        0        0       84 2023-05-18 11:35:01.000000 notebook-doc-0.2.1/src/notebook_doc/__init__.py
+-rw-rw-rw-   0        0        0    14834 2023-04-17 11:55:40.000000 notebook-doc-0.2.1/src/notebook_doc/doc_functions.py
+-rw-rw-rw-   0        0        0     4827 2023-03-24 10:22:31.000000 notebook-doc-0.2.1/src/notebook_doc/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:37:06.854494 notebook-doc-0.2.1/src/notebook_doc.egg-info/
+-rw-rw-rw-   0        0        0     2037 2023-05-18 11:37:06.000000 notebook-doc-0.2.1/src/notebook_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-18 11:37:06.000000 notebook-doc-0.2.1/src/notebook_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:37:06.000000 notebook-doc-0.2.1/src/notebook_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-18 11:37:06.000000 notebook-doc-0.2.1/src/notebook_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-18 11:37:06.000000 notebook-doc-0.2.1/src/notebook_doc.egg-info/top_level.txt
```

### Comparing `notebook-doc-0.2.0/LICENSE` & `notebook-doc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-doc-0.2.0/PKG-INFO` & `notebook-doc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-doc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to create documentation for functions in Databricks notebooks
 Author-email: Hiran Hasanka <hiranhasanka@gmail.com>
 Project-URL: Homepage, https://github.com/theSLWayne/notebook-doc
 Project-URL: Bug Tracker, https://github.com/theSLWayne/notebook-doc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notebook-doc-0.2.0/README.md` & `notebook-doc-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `notebook-doc-0.2.0/pyproject.toml` & `notebook-doc-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "Jinja2>=3.1.0", "docstring_parser>=0.15"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notebook-doc"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
   "Jinja2>=3.1.0",
   "docstring_parser>=0.15"
 ]
 authors = [
   { name="Hiran Hasanka", email="hiranhasanka@gmail.com" },
 ]
@@ -22,15 +22,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/theSLWayne/notebook-doc"
 "Bug Tracker" = "https://github.com/theSLWayne/notebook-doc/issues"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `notebook-doc-0.2.0/src/notebook_doc/doc_functions.py` & `notebook-doc-0.2.1/src/notebook_doc/doc_functions.py`

 * *Files identical despite different names*

### Comparing `notebook-doc-0.2.0/src/notebook_doc/test.py` & `notebook-doc-0.2.1/src/notebook_doc/test.py`

 * *Files identical despite different names*

### Comparing `notebook-doc-0.2.0/src/notebook_doc.egg-info/PKG-INFO` & `notebook-doc-0.2.1/src/notebook_doc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-doc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package to create documentation for functions in Databricks notebooks
 Author-email: Hiran Hasanka <hiranhasanka@gmail.com>
 Project-URL: Homepage, https://github.com/theSLWayne/notebook-doc
 Project-URL: Bug Tracker, https://github.com/theSLWayne/notebook-doc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

