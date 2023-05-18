# Comparing `tmp/cellgeometry-0.1.0.tar.gz` & `tmp/cellgeometry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellgeometry-0.1.0.tar", max compression
+gzip compressed data, was "cellgeometry-0.1.1.tar", max compression
```

## Comparing `cellgeometry-0.1.0.tar` & `cellgeometry-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      192 2023-04-21 16:55:26.217313 cellgeometry-0.1.0/README.md
--rw-r--r--   0        0        0      633 2023-05-12 08:50:34.861687 cellgeometry-0.1.0/cellgeometry/Hello.py
--rw-r--r--   0        0        0        0 2023-04-21 08:29:04.415769 cellgeometry-0.1.0/cellgeometry/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-12 10:21:58.312224 cellgeometry-0.1.0/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py
--rw-r--r--   0        0        0     3579 2023-05-12 12:07:45.106598 cellgeometry-0.1.0/cellgeometry/pages/1-Load_Data.py
--rw-r--r--   0        0        0     3119 2023-05-12 12:11:02.657968 cellgeometry-0.1.0/cellgeometry/pages/Cell_Shear.py
--rw-r--r--   0        0        0      833 2023-04-28 10:21:32.130658 cellgeometry-0.1.0/cellgeometry/utils/basic.py
--rw-r--r--   0        0        0     3053 2023-05-12 11:37:16.304501 cellgeometry-0.1.0/cellgeometry/utils/data_utils.py
--rw-r--r--   0        0        0    10885 2023-05-12 10:58:27.165188 cellgeometry-0.1.0/cellgeometry/utils/experimental.py
--rw-r--r--   0        0        0      543 2023-05-18 00:26:56.801913 cellgeometry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 cellgeometry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      192 2023-04-21 16:55:26.217313 cellgeometry-0.1.1/README.md
+-rw-r--r--   0        0        0      633 2023-05-12 08:50:34.861687 cellgeometry-0.1.1/cellgeometry/Hello.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:29:04.415769 cellgeometry-0.1.1/cellgeometry/__init__.py
+-rw-r--r--   0        0        0     7069 2023-05-12 10:21:58.312224 cellgeometry-0.1.1/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py
+-rw-r--r--   0        0        0     3579 2023-05-12 12:07:45.106598 cellgeometry-0.1.1/cellgeometry/pages/1-Load_Data.py
+-rw-r--r--   0        0        0     3119 2023-05-12 12:11:02.657968 cellgeometry-0.1.1/cellgeometry/pages/Cell_Shear.py
+-rw-r--r--   0        0        0      833 2023-04-28 10:21:32.130658 cellgeometry-0.1.1/cellgeometry/utils/basic.py
+-rw-r--r--   0        0        0     3053 2023-05-12 11:37:16.304501 cellgeometry-0.1.1/cellgeometry/utils/data_utils.py
+-rw-r--r--   0        0        0    10885 2023-05-12 10:58:27.165188 cellgeometry-0.1.1/cellgeometry/utils/experimental.py
+-rw-r--r--   0        0        0      663 2023-05-18 00:37:52.731562 cellgeometry-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 cellgeometry-0.1.1/PKG-INFO
```

### Comparing `cellgeometry-0.1.0/cellgeometry/Hello.py` & `cellgeometry-0.1.1/cellgeometry/Hello.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py` & `cellgeometry-0.1.1/cellgeometry/pages/ Elastic_Metric_for_Cell_Boundary_Analysis.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/cellgeometry/pages/1-Load_Data.py` & `cellgeometry-0.1.1/cellgeometry/pages/1-Load_Data.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/cellgeometry/pages/Cell_Shear.py` & `cellgeometry-0.1.1/cellgeometry/pages/Cell_Shear.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/cellgeometry/utils/basic.py` & `cellgeometry-0.1.1/cellgeometry/utils/basic.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/cellgeometry/utils/data_utils.py` & `cellgeometry-0.1.1/cellgeometry/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/cellgeometry/utils/experimental.py` & `cellgeometry-0.1.1/cellgeometry/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `cellgeometry-0.1.0/pyproject.toml` & `cellgeometry-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "cellgeometry"
-version = "0.1.0"
+version = "0.1.1"
 description = "Statistical Cell Shape Analysis"
-authors = ["Amil Khan <amil@ucsb.edu>"]
+authors = ["Amil Khan <amil@ucsb.edu>", "Samuel Feinstein <sdfeinstein@ucsb.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/bioshape-lab/cells"
+homepage = "https://github.com/bioshape-lab/cells/tree/main/cells/streamlit"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.21.0"
 numpy = "1.23.0"
 geomstats = "^2.5.0"
 scikit-image = "^0.20.0"
```

### Comparing `cellgeometry-0.1.0/PKG-INFO` & `cellgeometry-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cellgeometry
-Version: 0.1.0
+Version: 0.1.1
 Summary: Statistical Cell Shape Analysis
-Home-page: https://github.com/bioshape-lab/cells
+Home-page: https://github.com/bioshape-lab/cells/tree/main/cells/streamlit
 License: MIT
 Author: Amil Khan
 Author-email: amil@ucsb.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

