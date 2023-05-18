# Comparing `tmp/ifctester-0.0.230509.tar.gz` & `tmp/ifctester-0.0.230518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.230509.tar", last modified: Tue May  9 10:50:00 2023, max compression
+gzip compressed data, was "ifctester-0.0.230518.tar", last modified: Thu May 18 01:25:05 2023, max compression
```

## Comparing `ifctester-0.0.230509.tar` & `ifctester-0.0.230518.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:50:00.964173 ifctester-0.0.230509/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-09 10:50:00.964173 ifctester-0.0.230509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-09 10:49:47.000000 ifctester-0.0.230509/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:50:00.964173 ifctester-0.0.230509/ifctester/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-09 10:49:47.000000 ifctester-0.0.230509/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-09 10:49:47.000000 ifctester-0.0.230509/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40890 2023-05-09 10:49:47.000000 ifctester-0.0.230509/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-09 10:49:47.000000 ifctester-0.0.230509/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-09 10:49:47.000000 ifctester-0.0.230509/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:50:00.964173 ifctester-0.0.230509/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-09 10:50:00.000000 ifctester-0.0.230509/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 10:50:00.000000 ifctester-0.0.230509/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:50:00.000000 ifctester-0.0.230509/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 10:50:00.000000 ifctester-0.0.230509/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 10:50:00.000000 ifctester-0.0.230509/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 10:49:51.000000 ifctester-0.0.230509/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:50:00.964173 ifctester-0.0.230509/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:50:00.964173 ifctester-0.0.230509/test/
--rw-r--r--   0 runner    (1001) docker     (123)    88513 2023-05-09 10:49:47.000000 ifctester-0.0.230509/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-09 10:49:47.000000 ifctester-0.0.230509/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:25:05.366142 ifctester-0.0.230518/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-18 01:25:05.366142 ifctester-0.0.230518/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-18 01:24:52.000000 ifctester-0.0.230518/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:25:05.362142 ifctester-0.0.230518/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-18 01:24:52.000000 ifctester-0.0.230518/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-18 01:24:52.000000 ifctester-0.0.230518/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40890 2023-05-18 01:24:52.000000 ifctester-0.0.230518/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-18 01:24:52.000000 ifctester-0.0.230518/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-18 01:24:52.000000 ifctester-0.0.230518/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:25:05.366142 ifctester-0.0.230518/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-18 01:25:05.000000 ifctester-0.0.230518/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 01:25:05.000000 ifctester-0.0.230518/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 01:25:05.000000 ifctester-0.0.230518/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 01:25:05.000000 ifctester-0.0.230518/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 01:25:05.000000 ifctester-0.0.230518/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-18 01:24:56.000000 ifctester-0.0.230518/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 01:25:05.366142 ifctester-0.0.230518/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:25:05.366142 ifctester-0.0.230518/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    88513 2023-05-18 01:24:52.000000 ifctester-0.0.230518/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-18 01:24:52.000000 ifctester-0.0.230518/test/test_ids.py
```

### Comparing `ifctester-0.0.230509/PKG-INFO` & `ifctester-0.0.230518/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230509
+Version: 0.0.230518
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `ifctester-0.0.230509/README.md` & `ifctester-0.0.230518/README.md`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/ifctester/__init__.py` & `ifctester-0.0.230518/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/ifctester/__main__.py` & `ifctester-0.0.230518/ifctester/__main__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/ifctester/facet.py` & `ifctester-0.0.230518/ifctester/facet.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/ifctester/ids.py` & `ifctester-0.0.230518/ifctester/ids.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/ifctester/reporter.py` & `ifctester-0.0.230518/ifctester/reporter.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/ifctester.egg-info/PKG-INFO` & `ifctester-0.0.230518/ifctester.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230509
+Version: 0.0.230518
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `ifctester-0.0.230509/pyproject.toml` & `ifctester-0.0.230518/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ifctester"
-version = "0.0.230509"
+version = "0.0.230518"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC model auditing tool with support for IDS"
 readme = "README.md"
 keywords = ["IFC", "IDS", "BIM"]
 classifiers = [
```

### Comparing `ifctester-0.0.230509/test/test_facet.py` & `ifctester-0.0.230518/test/test_facet.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230509/test/test_ids.py` & `ifctester-0.0.230518/test/test_ids.py`

 * *Files identical despite different names*

