# Comparing `tmp/data_eng_utils-0.11.0.tar.gz` & `tmp/data_eng_utils-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_eng_utils-0.11.0.tar", max compression
+gzip compressed data, was "data_eng_utils-0.11.1.tar", max compression
```

## Comparing `data_eng_utils-0.11.0.tar` & `data_eng_utils-0.11.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     6881 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/README.md
--rw-r--r--   0        0        0      942 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/__init__.py
--rwxr-xr-x   0        0        0      134 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/_de_utils_exception.py
--rw-r--r--   0        0        0     1245 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/_logging_utils.py
--rw-r--r--   0        0        0     2766 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/_utils.py
--rwxr-xr-x   0        0        0       23 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/_version.py
--rwxr-xr-x   0        0        0      544 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/catalog_utils/__init__.py
--rwxr-xr-x   0        0        0     5844 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/catalog_utils/_catalog_utils.py
--rwxr-xr-x   0        0        0      440 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/__init__.py
--rw-r--r--   0        0        0     7752 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/_csv_loader.py
--rwxr-xr-x   0        0        0     6587 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/_excel_mapper.py
--rw-r--r--   0        0        0    17949 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/_fwf_loader.py
--rwxr-xr-x   0        0        0     3626 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/_fwf_schema_manager.py
--rwxr-xr-x   0        0        0    22805 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/_schema_manager.py
--rwxr-xr-x   0        0        0    34428 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/_table_loader.py
--rwxr-xr-x   0        0        0     8212 2023-05-18 13:22:57.476933 data_eng_utils-0.11.0/de_utils/engineering_utils/common_test_data.py
--rwxr-xr-x   0        0        0      810 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/hdfs_utils/__init__.py
--rw-r--r--   0        0        0    18822 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/hdfs_utils/_filename_handler.py
--rwxr-xr-x   0        0        0     4081 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/hdfs_utils/_filter_files_by_date.py
--rw-r--r--   0        0        0     7160 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/hdfs_utils/_hdfs_utils.py
--rwxr-xr-x   0        0        0      223 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/hdfs_utils/_hdfs_utils_exception.py
--rw-r--r--   0        0        0     1032 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/hdfs_utils/_manifest.py
--rwxr-xr-x   0        0        0      207 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/lookups/__init__.py
--rw-r--r--   0        0        0    11161 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/lookups/_lookups.py
--rw-r--r--   0        0        0     1126 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/spark_utils/__init__.py
--rw-r--r--   0        0        0     2919 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/spark_utils/_column_utils.py
--rw-r--r--   0        0        0     4472 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/spark_utils/_nspl.py
--rw-r--r--   0        0        0    14963 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/spark_utils/_spark_utils.py
--rw-r--r--   0        0        0     1387 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/spark_utils/_standardisation.py
--rwxr-xr-x   0        0        0     1852 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/spark_utils/_validation.py
--rwxr-xr-x   0        0        0     5126 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/README.md
--rw-r--r--   0        0        0      187 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/__init__.py
--rwxr-xr-x   0        0        0      490 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/__init__.py
--rwxr-xr-x   0        0        0     9734 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/base_columns.py
--rwxr-xr-x   0        0        0      902 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/date_column.py
--rwxr-xr-x   0        0        0     4242 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/decimal_column.py
--rw-r--r--   0        0        0     1264 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/numeric_columns.py
--rwxr-xr-x   0        0        0     8434 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/string_column.py
--rwxr-xr-x   0        0        0      932 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/columns/timestamp_column.py
--rwxr-xr-x   0        0        0     5757 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/common.py
--rw-r--r--   0        0        0    10211 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/de_utils/test_data_generation/table_generator.py
--rw-r--r--   0        0        0      773 2023-05-18 13:22:57.480933 data_eng_utils-0.11.0/pyproject.toml
--rw-r--r--   0        0        0     7775 1970-01-01 00:00:00.000000 data_eng_utils-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0     6881 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/README.md
+-rw-r--r--   0        0        0      942 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/__init__.py
+-rwxr-xr-x   0        0        0      134 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/_de_utils_exception.py
+-rw-r--r--   0        0        0     1245 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/_logging_utils.py
+-rw-r--r--   0        0        0     2766 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/_utils.py
+-rwxr-xr-x   0        0        0       23 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/_version.py
+-rwxr-xr-x   0        0        0      544 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/catalog_utils/__init__.py
+-rwxr-xr-x   0        0        0     5844 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/catalog_utils/_catalog_utils.py
+-rwxr-xr-x   0        0        0      440 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/__init__.py
+-rw-r--r--   0        0        0     7752 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/_csv_loader.py
+-rwxr-xr-x   0        0        0     6587 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/_excel_mapper.py
+-rw-r--r--   0        0        0    17949 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/_fwf_loader.py
+-rwxr-xr-x   0        0        0     3626 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/_fwf_schema_manager.py
+-rwxr-xr-x   0        0        0    22805 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/_schema_manager.py
+-rwxr-xr-x   0        0        0    34428 2023-05-18 14:57:58.081399 data_eng_utils-0.11.1/de_utils/engineering_utils/_table_loader.py
+-rwxr-xr-x   0        0        0     8212 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/engineering_utils/common_test_data.py
+-rwxr-xr-x   0        0        0      810 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/hdfs_utils/__init__.py
+-rw-r--r--   0        0        0    18822 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/hdfs_utils/_filename_handler.py
+-rwxr-xr-x   0        0        0     4081 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/hdfs_utils/_filter_files_by_date.py
+-rw-r--r--   0        0        0     7160 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/hdfs_utils/_hdfs_utils.py
+-rwxr-xr-x   0        0        0      223 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/hdfs_utils/_hdfs_utils_exception.py
+-rw-r--r--   0        0        0     1032 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/hdfs_utils/_manifest.py
+-rwxr-xr-x   0        0        0      207 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/lookups/__init__.py
+-rw-r--r--   0        0        0    11161 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/lookups/_lookups.py
+-rw-r--r--   0        0        0     1126 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/spark_utils/__init__.py
+-rw-r--r--   0        0        0     2919 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/spark_utils/_column_utils.py
+-rw-r--r--   0        0        0     4472 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/spark_utils/_nspl.py
+-rw-r--r--   0        0        0    14963 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/spark_utils/_spark_utils.py
+-rw-r--r--   0        0        0     1387 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/spark_utils/_standardisation.py
+-rwxr-xr-x   0        0        0     1852 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/spark_utils/_validation.py
+-rwxr-xr-x   0        0        0     5126 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/README.md
+-rw-r--r--   0        0        0      187 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/__init__.py
+-rwxr-xr-x   0        0        0      490 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/__init__.py
+-rwxr-xr-x   0        0        0     9734 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/base_columns.py
+-rwxr-xr-x   0        0        0      902 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/date_column.py
+-rwxr-xr-x   0        0        0     4242 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/decimal_column.py
+-rw-r--r--   0        0        0     1264 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/numeric_columns.py
+-rwxr-xr-x   0        0        0     8434 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/string_column.py
+-rwxr-xr-x   0        0        0      932 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/columns/timestamp_column.py
+-rwxr-xr-x   0        0        0     5757 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/common.py
+-rw-r--r--   0        0        0    10211 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/de_utils/test_data_generation/table_generator.py
+-rw-r--r--   0        0        0      773 2023-05-18 14:57:58.085399 data_eng_utils-0.11.1/pyproject.toml
+-rw-r--r--   0        0        0     7775 1970-01-01 00:00:00.000000 data_eng_utils-0.11.1/PKG-INFO
```

### Comparing `data_eng_utils-0.11.0/README.md` & `data_eng_utils-0.11.1/README.md`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/__init__.py` & `data_eng_utils-0.11.1/de_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/_logging_utils.py` & `data_eng_utils-0.11.1/de_utils/_logging_utils.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/_utils.py` & `data_eng_utils-0.11.1/de_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/catalog_utils/__init__.py` & `data_eng_utils-0.11.1/de_utils/catalog_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/catalog_utils/_catalog_utils.py` & `data_eng_utils-0.11.1/de_utils/catalog_utils/_catalog_utils.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/_csv_loader.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/_csv_loader.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/_excel_mapper.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/_excel_mapper.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/_fwf_loader.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/_fwf_loader.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/_fwf_schema_manager.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/_fwf_schema_manager.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/_schema_manager.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/_schema_manager.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/_table_loader.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/_table_loader.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/engineering_utils/common_test_data.py` & `data_eng_utils-0.11.1/de_utils/engineering_utils/common_test_data.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/hdfs_utils/__init__.py` & `data_eng_utils-0.11.1/de_utils/hdfs_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/hdfs_utils/_filename_handler.py` & `data_eng_utils-0.11.1/de_utils/hdfs_utils/_filename_handler.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/hdfs_utils/_filter_files_by_date.py` & `data_eng_utils-0.11.1/de_utils/hdfs_utils/_filter_files_by_date.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/hdfs_utils/_hdfs_utils.py` & `data_eng_utils-0.11.1/de_utils/hdfs_utils/_hdfs_utils.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/hdfs_utils/_manifest.py` & `data_eng_utils-0.11.1/de_utils/hdfs_utils/_manifest.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/lookups/_lookups.py` & `data_eng_utils-0.11.1/de_utils/lookups/_lookups.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/spark_utils/__init__.py` & `data_eng_utils-0.11.1/de_utils/spark_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/spark_utils/_column_utils.py` & `data_eng_utils-0.11.1/de_utils/spark_utils/_column_utils.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/spark_utils/_nspl.py` & `data_eng_utils-0.11.1/de_utils/spark_utils/_nspl.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/spark_utils/_spark_utils.py` & `data_eng_utils-0.11.1/de_utils/spark_utils/_spark_utils.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/spark_utils/_standardisation.py` & `data_eng_utils-0.11.1/de_utils/spark_utils/_standardisation.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/spark_utils/_validation.py` & `data_eng_utils-0.11.1/de_utils/spark_utils/_validation.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/README.md` & `data_eng_utils-0.11.1/de_utils/test_data_generation/README.md`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/columns/base_columns.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/columns/base_columns.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/columns/date_column.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/columns/date_column.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/columns/decimal_column.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/columns/decimal_column.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/columns/numeric_columns.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/columns/numeric_columns.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/columns/string_column.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/columns/string_column.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/columns/timestamp_column.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/columns/timestamp_column.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/common.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/common.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/de_utils/test_data_generation/table_generator.py` & `data_eng_utils-0.11.1/de_utils/test_data_generation/table_generator.py`

 * *Files identical despite different names*

### Comparing `data_eng_utils-0.11.0/pyproject.toml` & `data_eng_utils-0.11.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-eng-utils"
-version = "0.11.0"
+version = "0.11.1"
 description = "de_utils is a package that contains collections of useful functions grouped by theme e.g. HDFS, Spark, Python, etc... and a data engineering framework under the engineering_utils sub-package."
 authors = ["Office for National Statistics - Data Engineering"]
 license = ""
 readme = "README.md"
 packages = [{include = "de_utils"}]
 
 [tool.poetry.dependencies]
```

### Comparing `data_eng_utils-0.11.0/PKG-INFO` & `data_eng_utils-0.11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-eng-utils
-Version: 0.11.0
+Version: 0.11.1
 Summary: de_utils is a package that contains collections of useful functions grouped by theme e.g. HDFS, Spark, Python, etc... and a data engineering framework under the engineering_utils sub-package.
 Author: Office for National Statistics - Data Engineering
 Requires-Python: >=3.6.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

