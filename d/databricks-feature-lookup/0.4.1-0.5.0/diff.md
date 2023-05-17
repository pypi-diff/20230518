# Comparing `tmp/databricks-feature-lookup-0.4.1.tar.gz` & `tmp/databricks-feature-lookup-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-feature-lookup-0.4.1.tar", last modified: Thu Apr 20 18:14:44 2023, max compression
+gzip compressed data, was "databricks-feature-lookup-0.5.0.tar", last modified: Wed May 17 21:54:31 2023, max compression
```

## Comparing `databricks-feature-lookup-0.4.1.tar` & `databricks-feature-lookup-0.5.0.tar`

### file list

```diff
@@ -1,76 +1,84 @@
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.009162 databricks-feature-lookup-0.4.1/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2414 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/LICENSE.md
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      426 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/NOTICE.md
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     4219 2023-04-20 18:14:44.008973 databricks-feature-lookup-0.4.1/PKG-INFO
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     3488 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/README.md
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.981344 databricks-feature-lookup-0.4.1/databricks/
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.984541 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      166 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/__init__.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.984928 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.987155 databricks-feature-lookup-0.4.1/databricks/feature_store/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1980 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/__init__.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.996674 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/__init__.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1309 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_feature_store_object.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1489 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_proto_enum_entity.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      444 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/cloud.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     3039 2023-04-12 14:15:52.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/column_info.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      913 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/data_type.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2553 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_column_info.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    19284 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      715 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec_constants.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1055 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_table_info.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     3635 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_tables_for_serving.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      891 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/function_info.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1978 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/on_demand_column_info.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     6817 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_feature_table.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     5484 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_store_for_serving.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      489 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/query_mode.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      855 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/source_data_column_info.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      607 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/entities/store_type.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      139 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/feature_lookup_version.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:43.999448 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      753 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/__init__.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     7740 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    21707 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      923 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_engine.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2832 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     7533 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2130 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    27030 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1638 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model_constants.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    10759 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/online_lookup_client.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.000581 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/__init__.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     6382 2023-04-20 18:14:29.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_spec_pb2.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    20655 2023-04-20 18:14:29.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_store_serving_pb2.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.006364 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)        0 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/__init__.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     3871 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/converter_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1736 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_type_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      949 2023-04-20 01:23:16.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      765 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/data_type_details_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1739 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_type_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     4955 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      347 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/feature_serving_patch.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2302 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/feature_spec_test_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2631 2023-04-14 03:58:25.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/metrics_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    11749 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/pandas_type_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     8049 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/serving_test_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1278 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/sql_type_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      318 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/test_utils_common.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     8595 2023-04-20 18:08:03.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/uc_utils.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     1539 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/databricks/feature_store/utils/utils_common.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.007946 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     4219 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/PKG-INFO
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     3113 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 aakrati.talati   (502) staff       (20)        1 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 aakrati.talati   (502) staff       (20)       94 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/requires.txt
--rw-r--r--   0 aakrati.talati   (502) staff       (20)       11 2023-04-20 18:14:43.000000 databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/top_level.txt
--rw-r--r--   0 aakrati.talati   (502) staff       (20)       38 2023-04-20 18:14:44.009214 databricks-feature-lookup-0.4.1/setup.cfg
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     2724 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/setup.py
-drwxr-xr-x   0 aakrati.talati   (502) staff       (20)        0 2023-04-20 18:14:44.008686 databricks-feature-lookup-0.4.1/tests/
--rw-r--r--   0 aakrati.talati   (502) staff       (20)    65035 2023-04-20 18:13:39.000000 databricks-feature-lookup-0.4.1/tests/test_mlflow_model.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)      369 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/tests/test_mlflow_model_constants.py
--rw-r--r--   0 aakrati.talati   (502) staff       (20)     8686 2023-03-21 00:53:58.000000 databricks-feature-lookup-0.4.1/tests/test_online_lookup_client.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.681590 databricks-feature-lookup-0.5.0/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2414 2022-08-15 17:42:42.000000 databricks-feature-lookup-0.5.0/LICENSE.md
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      426 2022-08-15 17:42:42.000000 databricks-feature-lookup-0.5.0/NOTICE.md
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     4219 2023-05-17 21:54:31.681404 databricks-feature-lookup-0.5.0/PKG-INFO
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     3488 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/README.md
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.654343 databricks-feature-lookup-0.5.0/databricks/
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.656854 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      166 2022-11-08 00:41:08.000000 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/__init__.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.657193 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2022-11-08 00:41:08.000000 databricks-feature-lookup-0.5.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.658837 databricks-feature-lookup-0.5.0/databricks/feature_store/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1980 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/__init__.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.667921 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/__init__.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1309 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_feature_store_object.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1489 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_proto_enum_entity.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      444 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/cloud.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     3039 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/column_info.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      913 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/data_type.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2553 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_column_info.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     3971 2023-04-20 18:30:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_functions_for_serving.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    19367 2023-04-26 18:25:23.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      715 2023-03-13 18:56:02.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec_constants.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1544 2023-04-26 18:25:23.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_table_info.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     4065 2023-04-26 18:25:23.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_tables_for_serving.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      673 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/function_info.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1978 2023-04-20 23:09:44.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/on_demand_column_info.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     6817 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_feature_table.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     5484 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_store_for_serving.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      489 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/query_mode.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      855 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/source_data_column_info.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      659 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/entities/store_type.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.668459 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     7556 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/feature_function_executor.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2817 2023-04-21 16:15:58.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/feature_function_loader.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.669018 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2023-04-21 16:15:58.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/__init__.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1855 2023-04-21 16:15:58.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_functions/utils/codegen_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      139 2023-05-17 20:30:14.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/feature_lookup_version.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.670990 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      753 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/__init__.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     7961 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    21707 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      923 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_engine.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2832 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     7533 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2130 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    32490 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2066 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model_constants.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    10759 2023-04-23 22:18:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/online_lookup_client.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.671747 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2022-08-15 17:42:42.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/__init__.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     6396 2023-05-17 21:53:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_spec_pb2.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    21337 2023-05-17 21:53:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_store_serving_pb2.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.677855 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)        0 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/__init__.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     3871 2023-04-26 02:11:21.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/converter_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1736 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_type_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      949 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      765 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/data_type_details_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1739 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_type_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     4955 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     3117 2023-05-17 18:04:44.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_function_type_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      347 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_serving_patch.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2317 2023-05-04 17:42:39.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_spec_test_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2631 2023-04-11 17:04:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/metrics_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    11740 2023-04-26 02:11:21.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/pandas_type_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     8049 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/serving_test_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1278 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/sql_type_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      374 2023-05-05 16:47:48.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/test_utils_common.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    10305 2023-04-20 18:30:22.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/uc_utils.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     1539 2023-04-03 22:23:57.000000 databricks-feature-lookup-0.5.0/databricks/feature_store/utils/utils_common.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.679374 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     4219 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     3511 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 avesh.singh   (502) staff       (20)        1 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      107 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/requires.txt
+-rw-r--r--   0 avesh.singh   (502) staff       (20)       11 2023-05-17 21:54:31.000000 databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/top_level.txt
+-rw-r--r--   0 avesh.singh   (502) staff       (20)       38 2023-05-17 21:54:31.681653 databricks-feature-lookup-0.5.0/setup.cfg
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     2724 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/setup.py
+drwxr-xr-x   0 avesh.singh   (502) staff       (20)        0 2023-05-17 21:54:31.680943 databricks-feature-lookup-0.5.0/tests/
+-rw-r--r--   0 avesh.singh   (502) staff       (20)    88854 2023-05-16 17:08:40.000000 databricks-feature-lookup-0.5.0/tests/test_mlflow_model.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)      369 2023-03-13 18:17:52.000000 databricks-feature-lookup-0.5.0/tests/test_mlflow_model_constants.py
+-rw-r--r--   0 avesh.singh   (502) staff       (20)     8686 2023-04-20 18:13:49.000000 databricks-feature-lookup-0.5.0/tests/test_online_lookup_client.py
```

### Comparing `databricks-feature-lookup-0.4.1/LICENSE.md` & `databricks-feature-lookup-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/PKG-INFO` & `databricks-feature-lookup-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.4.1
+Version: 0.5.0
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.4.1/README.md` & `databricks-feature-lookup-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/__init__.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_feature_store_object.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_feature_store_object.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/_proto_enum_entity.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/_proto_enum_entity.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/column_info.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/data_type.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/data_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_column_info.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,21 @@
 # 1. Initial.
 # 2. (2021/06/16): Record feature_store_client_version to help us make backward compatible changes in the future.
 # 3. (2021/08/25): Record table_id to handle feature table lineage stability if tables are deleted.
 # 4. (2021/09/25): Record timestamp_lookup_key to handle point-in-time lookups.
 # 5. (2021/02/15): Record include flag for column info if False.
 #                  Record input functions as FunctionInfo and function computation as OnDemandColumnInfo.
 #                  Remove redundant fields: table_name from table_infos, output_name from column_infos.
+# 6. (2023/04/21): Record lookback_window in table info for point-in-time lookups.
 
 
 class FeatureSpec(_FeatureStoreObject):
 
     FEATURE_ARTIFACT_FILE = "feature_spec.yaml"
-    SERIALIZATION_VERSION_NUMBER = 5
+    SERIALIZATION_VERSION_NUMBER = 6
 
     def __init__(
         self,
         column_infos: List[ColumnInfo],
         table_infos: List[FeatureTableInfo],
         function_infos: List[FunctionInfo],
         workspace_id: int,
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_spec_constants.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_spec_constants.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/feature_tables_for_serving.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/feature_tables_for_serving.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,18 @@
         """
         Loads a binary serialized ProtoFeatureTablesForServing protocol buffer.
 
         :param path: Root path to the binary file.
         :return: :py:class:`~databricks.feature_store.entities.feature_tables_for_serving.FeatureTablesForServing`
         """
         proto = ProtoFeatureTablesForServing()
+        # The load path may be None when the model is packaged by Feature Store, but did not use any
+        # feature tables (eg just feature functions)
+        if not path:
+            return cls.from_proto(proto)
         with open(os.path.join(path, cls.DATA_FILE), "rb") as f:
             proto.ParseFromString(f.read())
         return cls.from_proto(proto)
 
 
 class FeatureTablesForSageMakerServing(AbstractFeatureTablesForServing):
     DATA_FILE = "feature_tables_for_sagemaker_serving.dat"
@@ -91,10 +95,14 @@
         """
         Loads a binary serialized FeatureTablesForSageMakerServing protocol buffer.
 
         :param path: Root path to the binary file.
         :return: :py:class:`~databricks.feature_store.entities.feature_tables_for_serving.FeatureTablesForSageMakerServing`
         """
         proto = ProtoFeatureTablesForSageMakerServing()
+        # load may be passed None when the model is packaged by Feature Store, but did not use any
+        # feature tables (eg just feature functions)
+        if not path:
+            return cls.from_proto(proto)
         with open(os.path.join(path, cls.DATA_FILE), "rb") as f:
             proto.ParseFromString(f.read())
         return cls.from_proto(proto)
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/function_info.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/function_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 from databricks.feature_store.entities._feature_store_object import _FeatureStoreObject
 from databricks.feature_store.protos.feature_spec_pb2 import (
     FunctionInfo as ProtoFunctionInfo,
 )
 
 
 class FunctionInfo(_FeatureStoreObject):
-    def __init__(self, udf_name: str, md5: str):
+    def __init__(self, udf_name: str):
         if not udf_name:
             raise ValueError("udf_name must be non-empty.")
-        if not md5:
-            raise ValueError("md5 must be non-empty.")
         self._udf_name = udf_name
-        self._md5 = md5
 
     @property
     def udf_name(self) -> str:
         return self._udf_name
 
-    @property
-    def md5(self) -> str:
-        return self._md5
-
     @classmethod
     def from_proto(cls, function_info_proto):
-        return cls(udf_name=function_info_proto.udf_name, md5=function_info_proto.md5)
+        return cls(udf_name=function_info_proto.udf_name)
 
     def to_proto(self):
-        return ProtoFunctionInfo(udf_name=self.udf_name, md5=self.md5)
+        return ProtoFunctionInfo(udf_name=self.udf_name)
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/on_demand_column_info.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/on_demand_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_feature_table.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_feature_table.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/online_store_for_serving.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/online_store_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/source_data_column_info.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/source_data_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/entities/store_type.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/entities/store_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,11 +10,12 @@
     """Online store types."""
 
     AURORA_MYSQL = ProtoStoreType.Value("AURORA_MYSQL")
     SQL_SERVER = ProtoStoreType.Value("SQL_SERVER")
     MYSQL = ProtoStoreType.Value("MYSQL")
     DYNAMODB = ProtoStoreType.Value("DYNAMODB")
     COSMOSDB = ProtoStoreType.Value("COSMOSDB")
+    BRICKSTORE = ProtoStoreType.Value("BRICKSTORE")
 
     @classmethod
     def _enum_type(cls) -> Any:
         return ProtoStoreType
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/__init__.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,19 @@
     def __init__(
         self, online_feature_table: OnlineFeatureTable, authorization_key: str
     ):
         """
         :param online_feature_table: OnlineFeatureTable to look up feature values from.
         :param authorization_key: Uses this authorization key to authenticate with Cosmos DB.
         """
-        # The online feature table name is of the format database_name.container_name.
+        # The online feature table name is 2L for HMS tables and either 2L or 3L for UC tables.
+        # 2L name "database.table" is mapped to Cosmos DB database="database", container="table".
+        # 3L name "catalog.schema.table" is mapped to Cosmos DB database="catalog.schema", container="table".
         self.online_table_name = online_feature_table.online_feature_table_name
-        self.database_name, self.container_name = self.online_table_name.split(".")
+        self.database_name, self.container_name = self.online_table_name.rsplit(".", 1)
 
         # Retrieve the relevant configuration and helpers needed for lookup.
         self.account_uri = online_feature_table.online_store.extra_configs.account_uri
         self.query_mode = online_feature_table.online_store.query_mode
         self.timestamp_keys = online_feature_table.timestamp_keys
         self.primary_keys_to_type_converter = {
             pk.name: COSMOSDB_DATA_TYPE_CONVERTER_FACTORY.get_converter(pk)
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_engine.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+import functools
 import itertools
 import os
 from collections import Counter, defaultdict
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import mlflow
 import pandas as pd
 from mlflow.models.container import SERVING_ENVIRONMENT
 from mlflow.sagemaker import SAGEMAKER_SERVING_ENVIRONMENT
 from mlflow.utils import databricks_utils
 
 from databricks.feature_store import mlflow_model_constants
 from databricks.feature_store.entities.feature_column_info import FeatureColumnInfo
+from databricks.feature_store.entities.feature_functions_for_serving import (
+    FeatureFunctionsForServing,
+)
 from databricks.feature_store.entities.feature_spec import FeatureSpec
 from databricks.feature_store.entities.feature_tables_for_serving import (
     AbstractFeatureTablesForServing,
     FeatureTablesForSageMakerServing,
     FeatureTablesForServing,
 )
 from databricks.feature_store.entities.online_feature_table import (
     AbstractOnlineFeatureTable,
     OnlineFeatureTable,
     PrimaryKeyDetails,
 )
 from databricks.feature_store.entities.store_type import StoreType
+from databricks.feature_store.feature_functions.feature_function_executor import (
+    FeatureFunctionExecutor,
+)
 from databricks.feature_store.feature_lookup_version import VERSION
 from databricks.feature_store.online_lookup_client import (
     OnlineLookupClient,
     is_primary_key_lookup,
     tables_share_dynamodb_access_keys,
 )
 from databricks.feature_store.utils.feature_serving_patch import (
@@ -44,14 +51,19 @@
 
 # The provisioner of this model is expected to set an environment variable with the path to a
 # feature_tables_for_serving.dat file.
 FEATURE_TABLES_FOR_SERVING_FILEPATH_ENV = "FEATURE_TABLES_FOR_SERVING_FILEPATH"
 # should match LOOKUP_CLIENT_INSTRUMENTATION_ENABLED_ENV in
 # model-serving/model-serving-common/src/main/scala/com/databricks/mlflow/utils/serving/FeatureStoreConstants.scala
 LOOKUP_CLIENT_INSTRUMENTATION_ENABLED_ENV = "LOOKUP_CLIENT_INSTRUMENTATION_ENABLED"
+# should match LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED_ENV in
+# model-serving/model-serving-common/src/main/scala/com/databricks/mlflow/utils/serving/FeatureStoreConstants.scala
+LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED_ENV = (
+    "LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED"
+)
 
 FEATURE_SERVING_RESPONSE_FORMAT_ENABLED = False
 
 LookupKeyType = Tuple[str, ...]
 LookupKeyToFeatureColumnInfosType = Dict[LookupKeyType, List[FeatureColumnInfo]]
 
 
@@ -77,15 +89,15 @@
 def _load_raw_model(path):
     raw_model_path = os.path.join(path, mlflow_model_constants.RAW_MODEL_FOLDER)
     return mlflow.pyfunc.load_model(raw_model_path)
 
 
 class _FeatureStoreModelWrapper:
     def __init__(self, path: str):
-        print(f"Initializing feature store lookup client: ${VERSION}")
+        print(f"Initializing feature store lookup client: {VERSION}")
         self._check_support()
         self.serving_environment = self._get_serving_environment()
         feature_tables_for_serving = self._load_feature_tables_for_serving(
             self.serving_environment, path
         )
 
         self.raw_model = _load_raw_model(path)
@@ -115,14 +127,36 @@
         if self.is_model_eligible_for_batch_lookup:
             self.batch_lookup_client = self._create_batch_lookup_client(
                 self.ft_metadata
             )
         else:
             self.ft_to_lookup_client = self._create_lookup_clients(self.ft_metadata)
 
+        if self._is_lookup_client_feature_function_evaluation_enabled():
+            self.has_feature_functions = self._has_feature_functions(path)
+            if self.has_feature_functions:
+                feature_function_dir = os.path.join(
+                    path, mlflow_model_constants.FEATURE_STORE_INTERNAL_DATA_DIR
+                )
+                feature_functions_for_serving = FeatureFunctionsForServing.load(
+                    feature_function_dir
+                )
+                self.feature_function_executor = FeatureFunctionExecutor(
+                    feature_functions_for_serving,
+                    self.feature_spec.on_demand_column_infos,
+                )
+
+    def _has_feature_functions(self, path):
+        feature_function_dir = os.path.join(
+            path, mlflow_model_constants.FEATURE_STORE_INTERNAL_DATA_DIR
+        )
+        return os.path.isfile(
+            os.path.join(feature_function_dir, FeatureFunctionsForServing.DATA_FILE)
+        )
+
     # true if all feature tables using DynamoDB under same authorization (ie same region and keys)
     # this is true by default for customers using Sagemaker
     def _is_model_eligible_for_batch_lookup(
         self, ft_metadata: Dict[str, _FeatureTableMetadata]
     ):
         env = self._get_serving_environment()
         online_feature_tables = [meta.online_ft for _, meta in ft_metadata.items()]
@@ -158,44 +192,60 @@
 
     @staticmethod
     def _is_lookup_client_instrumentation_enabled() -> bool:
         # environment variables stored as string, rather than boolean
         return os.getenv(LOOKUP_CLIENT_INSTRUMENTATION_ENABLED_ENV) == "true"
 
     @staticmethod
+    def _is_lookup_client_feature_function_evaluation_enabled() -> bool:
+        return (
+            os.getenv(LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED_ENV) == "true"
+        )
+
+    @staticmethod
     def _check_support():
         if (
             databricks_utils.is_in_databricks_notebook()
             or databricks_utils.is_in_databricks_job()
         ):
             raise NotImplementedError(
                 "Feature Store packaged models cannot be loaded with MLflow APIs. For batch "
                 "inference, use FeatureStoreClient.score_batch."
             )
 
     @staticmethod
-    def _validate_ft_metadata(ft_metadata):
+    def _validate_ft_metadata(ft_metadata: Dict[str, _FeatureTableMetadata]):
         for (ft, meta) in ft_metadata.items():
             for lookup_key in meta.feature_col_infos_by_lookup_key.keys():
                 if len(lookup_key) != len(meta.online_ft.primary_keys):
                     raise Exception(
                         f"Internal error: Online feature table has primary keys "
                         f"{meta.online_ft.primary_keys}, however FeatureSpec specifies "
                         f"{len(lookup_key)} lookup_keys: {lookup_key}."
                     )
 
-    def _create_lookup_clients(self, ft_metadata):
+    def _create_lookup_clients(
+        self, ft_metadata: Dict[str, _FeatureTableMetadata]
+    ) -> Dict[str, OnlineLookupClient]:
         ft_to_lookup_client = {}
         for ft, meta in ft_metadata.items():
             ft_to_lookup_client[ft] = OnlineLookupClient(
                 meta.online_ft, serving_environment=self.serving_environment
             )
         return ft_to_lookup_client
 
-    def _create_batch_lookup_client(self, ft_metadata):
+    def _create_batch_lookup_client(
+        self, ft_metadata: Dict[str, _FeatureTableMetadata]
+    ) -> Optional[OnlineLookupClient]:
+        """
+        Creates and returns an OnlineLookupClient for batch lookup, or None if `ft_metadata` is
+        empty.
+        """
+        if not ft_metadata:
+            return None
         online_fts = []
         for ft, meta in ft_metadata.items():
             online_fts.append(meta.online_ft)
 
         return OnlineLookupClient(
             online_fts, serving_environment=self.serving_environment
         )
@@ -204,19 +254,45 @@
         self._validate_input(df)
 
         # if enabled, use metrics class to record metric values in child function calls
         output_metrics = None
         if self._is_lookup_client_instrumentation_enabled():
             output_metrics = LookupClientMetrics({})
 
-        augment_with_features = lookup_call_maybe_with_metrics(
-            self._augment_with_features, output_metrics, measuring_e2e_latency=True
+        augment_with_materialized_features = lookup_call_maybe_with_metrics(
+            self._augment_with_materialized_features,
+            output_metrics,
+            measuring_e2e_latency=True,
         )
 
-        model_input_df = augment_with_features(df, metrics=output_metrics)
+        # Add materialized features to `df`. This call does not do input column filtering, which is
+        # important as Feature Functions may require inputs with include=False, so filtering must
+        # be done after Feature Function execution. See _augment_with_materialized_features
+        # docstring for details.
+        df_with_materialized_features = augment_with_materialized_features(
+            df, metrics=output_metrics
+        )
+        if (
+            self._is_lookup_client_feature_function_evaluation_enabled()
+            and self.has_feature_functions
+        ):
+            feature_functions_df = self._compute_feature_functions(
+                df_with_materialized_features, df
+            )
+
+            model_input_unordered = pd.concat(
+                [df_with_materialized_features, feature_functions_df], axis=1
+            )
+        else:
+            model_input_unordered = df_with_materialized_features
+
+        output_cols = [
+            ci.output_name for ci in self.feature_spec.column_infos if ci.include
+        ]
+        model_input_df = model_input_unordered[output_cols]
         prediction = self.raw_model.predict(model_input_df)
 
         # will add any captured metrics to output via pandas series attributes
         if output_metrics:
             # if prediction is not pandas object (aka list or np array), convert prediction to panda series so it will have pandas attributes
             if not isinstance(prediction, pd.DataFrame) and not isinstance(
                 prediction, pd.Series
@@ -358,23 +434,45 @@
         if cols_with_nulls:
             raise ValueError(
                 f"Failed to lookup feature values due to null values for lookup_key columns "
                 f"{cols_with_nulls}. The following columns cannot contain null values: "
                 f"{lookup_key_columns}"
             )
 
-    def _augment_with_features(
+    def _augment_with_materialized_features(
         self, df: pd.DataFrame, *, metrics: LookupClientMetrics = None
-    ):
+    ) -> pd.DataFrame:
         """
+        Adds materialized features to `df`. This function does not filter out ColumnInfos with
+        include=False, however it will drop any columns in `df` that are not in the FeatureSpec.
+
+        For example, a FeatureSpec may include
+
+            - revenue:
+                include: false
+                source: training_data
+            - cost:
+                include: false
+                source: training_data
+            - profit:
+                udf_name: prod.math.subtract
+                input_bindings:
+                  x: sales
+                  y: cost
+                source: on_demand_feature
+
+         In this case, the DataFrame returned by this method will include columns `revenue` and
+         `cost`. This is required to compute the Feature Function `profit` at a later stage.
+
         :param df: Pandas DataFrame provided by user as model input. This is expected to contain
         columns for each SourceColumnInfo, and for each lookup key of a FeatureColumnInfo. Columns
         with the same name as FeatureColumnInfo output_names will override those features, meaning
         they will not be queried from the online store.
-        :return: Pandas DataFrame containing all features specified in the FeatureSpec, in order.
+        :return: Pandas DataFrame containing all materialized features specified in the FeatureSpec,
+          including features with include=False (see example above).
         """
         feature_dfs = []
         overridden_features_count = 0
         (
             fully_overridden_feature_output_names,
             partially_overridden_feature_output_names,
         ) = self._get_overridden_feature_output_names(df)
@@ -494,17 +592,43 @@
         model_input_unordered = pd.concat(
             feature_dfs + [source_data_df, overridden_features_df], axis=1
         )
 
         if metrics:
             metrics.increase_metric(OVERRIDEN_FEATURE_COUNT, overridden_features_count)
 
-        output_cols = [ci.output_name for ci in self.feature_spec.column_infos]
-        model_input_df = model_input_unordered[output_cols]
-        return model_input_df
+        return model_input_unordered
+
+    def _compute_feature_functions(
+        self, ff_inputs: pd.DataFrame, ff_overrides: pd.DataFrame
+    ) -> pd.DataFrame:
+        """
+        Executes Feature Functions specified by FeatureSpec.
+
+        :param ff_inputs: A DataFrame containing all inputs required to evaluate Feature Functions.
+          Additional columns are permitted.
+        :param ff_overrides: A DataFrame containing overrides to Feature Functions. When a Feature
+          Function output name is included as a column in `ff_overrides`, the function is computed
+          only for rows where the override is `np.nan`.
+        :return: DataFrame containing computed Feature Function columns
+        """
+        # TODO(ML-30619): Short-circuit Feature Function execution when overridden
+        feature_function_df = self.feature_function_executor.execute_feature_functions(
+            ff_inputs
+        )
+        overridden_ff_outputs = [
+            odci.output_name
+            for odci in self.feature_spec.on_demand_column_infos
+            if odci.output_name in ff_overrides.columns
+        ]
+        overridden_ff_df = ff_overrides[overridden_ff_outputs]
+        # As with materialized features, Feature Functions may be fully or partially
+        # overridden, where a partial override means that some rows have null override value.
+        # Merge the overridden values with the computed feature values:
+        return overridden_ff_df.combine_first(feature_function_df)
 
     def _get_primary_key_df(
         self,
         lookup_key: LookupKeyType,
         primary_key: List[PrimaryKeyDetails],
         df: pd.DataFrame,
     ):
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/mlflow_model_constants.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/mlflow_model_constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,7 +29,12 @@
 # Minor version
 FEATURE_LOOKUP_CLIENT_ALPHA_MINOR_VERSION = 3
 # Micro version
 FEATURE_LOOKUP_CLIENT_ALPHA_MICRO_VERSION = 1
 
 DATABRICKS = "Databricks"
 SAGEMAKER = "SageMaker"
+
+# Model artifact directory where we expect Feature Store internal artifacts to live. This must
+# match the directory specified in ModelServingUtils:
+# https://src.dev.databricks.com/databricks/universe@4dff77c752b546579f239815e520d566d2dbda20/-/blob/model-serving/model-serving-common/src/main/scala/com/databricks/modelservingcommon/utils/ModelServingUtils.scala?L117
+FEATURE_STORE_INTERNAL_DATA_DIR = "_databricks_internal/"
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/online_lookup_client.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/online_lookup_client.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_spec_pb2.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_spec_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from mlflow.protos.scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2
 from mlflow.protos import databricks_pb2 as databricks__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x66\x65\x61ture_spec.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\x1a\x10\x64\x61tabricks.proto\"$\n\x14SourceDataColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x46\x65\x61tureColumnInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x12\n\nlookup_key\x18\x03 \x03(\t\x12\x13\n\x0boutput_name\x18\x04 \x01(\t\x12\x1c\n\x14timestamp_lookup_key\x18\x05 \x03(\t\"3\n\x0cInputBinding\x12\x11\n\tparameter\x18\x01 \x01(\t\x12\x10\n\x08\x62ound_to\x18\x02 \x01(\t\"u\n\x12OnDemandColumnInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\x12\x38\n\x0einput_bindings\x18\x02 \x03(\x0b\x32 .featurestorecommon.InputBinding\x12\x13\n\x0boutput_name\x18\x03 \x01(\t\"\x87\x02\n\nColumnInfo\x12K\n\x17source_data_column_info\x18\x01 \x01(\x0b\x32(.featurestorecommon.SourceDataColumnInfoH\x00\x12\x44\n\x13\x66\x65\x61ture_column_info\x18\x02 \x01(\x0b\x32%.featurestorecommon.FeatureColumnInfoH\x00\x12G\n\x15on_demand_column_info\x18\x03 \x01(\x0b\x32&.featurestorecommon.OnDemandColumnInfoH\x00\x12\x15\n\x07include\x18\n \x01(\x08:\x04trueB\x06\n\x04info\"8\n\x10\x46\x65\x61tureTableInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x10\n\x08table_id\x18\x02 \x01(\t\"-\n\x0c\x46unctionInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\x12\x0b\n\x03md5\x18\x02 \x01(\t\"\x96\x02\n\x0b\x46\x65\x61tureSpec\x12\x35\n\rinput_columns\x18\x01 \x03(\x0b\x32\x1e.featurestorecommon.ColumnInfo\x12\x1d\n\x15serialization_version\x18\x02 \x01(\x05\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\x03\x12$\n\x1c\x66\x65\x61ture_store_client_version\x18\x04 \x01(\t\x12:\n\x0cinput_tables\x18\x05 \x03(\x0b\x32$.featurestorecommon.FeatureTableInfo\x12\x39\n\x0finput_functions\x18\x06 \x03(\x0b\x32 .featurestorecommon.FunctionInfoBC\n\'com.databricks.proto.featurestorecommonB\x10\x46\x65\x61tureSpecProto\xa0\x01\x01\xe2?\x02\x10\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x66\x65\x61ture_spec.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\x1a\x10\x64\x61tabricks.proto\"$\n\x14SourceDataColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x46\x65\x61tureColumnInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x12\n\nlookup_key\x18\x03 \x03(\t\x12\x13\n\x0boutput_name\x18\x04 \x01(\t\x12\x1c\n\x14timestamp_lookup_key\x18\x05 \x03(\t\"3\n\x0cInputBinding\x12\x11\n\tparameter\x18\x01 \x01(\t\x12\x10\n\x08\x62ound_to\x18\x02 \x01(\t\"u\n\x12OnDemandColumnInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\x12\x38\n\x0einput_bindings\x18\x02 \x03(\x0b\x32 .featurestorecommon.InputBinding\x12\x13\n\x0boutput_name\x18\x03 \x01(\t\"\x87\x02\n\nColumnInfo\x12K\n\x17source_data_column_info\x18\x01 \x01(\x0b\x32(.featurestorecommon.SourceDataColumnInfoH\x00\x12\x44\n\x13\x66\x65\x61ture_column_info\x18\x02 \x01(\x0b\x32%.featurestorecommon.FeatureColumnInfoH\x00\x12G\n\x15on_demand_column_info\x18\x03 \x01(\x0b\x32&.featurestorecommon.OnDemandColumnInfoH\x00\x12\x15\n\x07include\x18\n \x01(\x08:\x04trueB\x06\n\x04info\"Q\n\x10\x46\x65\x61tureTableInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x10\n\x08table_id\x18\x02 \x01(\t\x12\x17\n\x0flookback_window\x18\x03 \x01(\x03\" \n\x0c\x46unctionInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\"\x96\x02\n\x0b\x46\x65\x61tureSpec\x12\x35\n\rinput_columns\x18\x01 \x03(\x0b\x32\x1e.featurestorecommon.ColumnInfo\x12\x1d\n\x15serialization_version\x18\x02 \x01(\x05\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\x03\x12$\n\x1c\x66\x65\x61ture_store_client_version\x18\x04 \x01(\t\x12:\n\x0cinput_tables\x18\x05 \x03(\x0b\x32$.featurestorecommon.FeatureTableInfo\x12\x39\n\x0finput_functions\x18\x06 \x03(\x0b\x32 .featurestorecommon.FunctionInfoBC\n\'com.databricks.proto.featurestorecommonB\x10\x46\x65\x61tureSpecProto\xa0\x01\x01\xe2?\x02\x10\x01')
 
 
 
 _SOURCEDATACOLUMNINFO = DESCRIPTOR.message_types_by_name['SourceDataColumnInfo']
 _FEATURECOLUMNINFO = DESCRIPTOR.message_types_by_name['FeatureColumnInfo']
 _INPUTBINDING = DESCRIPTOR.message_types_by_name['InputBinding']
 _ONDEMANDCOLUMNINFO = DESCRIPTOR.message_types_by_name['OnDemandColumnInfo']
@@ -95,13 +95,13 @@
   _INPUTBINDING._serialized_start=256
   _INPUTBINDING._serialized_end=307
   _ONDEMANDCOLUMNINFO._serialized_start=309
   _ONDEMANDCOLUMNINFO._serialized_end=426
   _COLUMNINFO._serialized_start=429
   _COLUMNINFO._serialized_end=692
   _FEATURETABLEINFO._serialized_start=694
-  _FEATURETABLEINFO._serialized_end=750
-  _FUNCTIONINFO._serialized_start=752
-  _FUNCTIONINFO._serialized_end=797
-  _FEATURESPEC._serialized_start=800
-  _FEATURESPEC._serialized_end=1078
+  _FEATURETABLEINFO._serialized_end=775
+  _FUNCTIONINFO._serialized_start=777
+  _FUNCTIONINFO._serialized_end=809
+  _FEATURESPEC._serialized_start=812
+  _FEATURESPEC._serialized_end=1090
 # @@protoc_insertion_point(module_scope)
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/protos/feature_store_serving_pb2.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/protos/feature_store_serving_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from mlflow.protos.scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x65\x61ture_store_serving.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\"\xdc\x03\n\x15OnlineStoreForServing\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x1a\n\x12read_secret_prefix\x18\x03 \x01(\t\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x04 \x01(\x03\x12\x33\n\nmysql_conf\x18\x05 \x01(\x0b\x32\x1d.featurestorecommon.MySqlConfH\x00\x12<\n\x0fsql_server_conf\x18\x06 \x01(\x0b\x32!.featurestorecommon.SqlServerConfH\x00\x12\x39\n\rdynamodb_conf\x18\x07 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x39\n\rcosmosdb_conf\x18\x08 \x01(\x0b\x32 .featurestorecommon.CosmosDbConfH\x00\x12\x31\n\nquery_mode\x18\x15 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\'\n\tMySqlConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"+\n\rSqlServerConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x1e\n\x0c\x44ynamoDbConf\x12\x0e\n\x06region\x18\x01 \x01(\t\"#\n\x0c\x43osmosDbConf\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\"j\n\x0e\x46\x65\x61tureDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x19\n\x11\x64\x61ta_type_details\x18\x03 \x01(\t\"R\n\x11PrimaryKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"T\n\x13TimestampKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xe2\x02\n\x12OnlineFeatureTable\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12?\n\x0conline_store\x18\x03 \x01(\x0b\x32).featurestorecommon.OnlineStoreForServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"X\n\x17\x46\x65\x61tureTablesForServing\x12=\n\ronline_tables\x18\x01 \x03(\x0b\x32&.featurestorecommon.OnlineFeatureTable\"+\n\rMySqlMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"/\n\x11SqlServerMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"B\n\x10\x44ynamoDbMetadata\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x11\n\ttable_arn\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"K\n\x10\x43osmosDbMetadata\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\x12\x15\n\rcontainer_uri\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"\xa9\x04\n\x0bOnlineStore\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12;\n\x0emysql_metadata\x18\n \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\x0b \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0c \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\r \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"\xdf\x04\n\x13OnlineStoreDetailed\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\n \x03(\t\x12\x1a\n\x12read_secret_prefix\x18\x0b \x01(\t\x12;\n\x0emysql_metadata\x18\x0c \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\r \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0e \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\x0f \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"t\n FeatureTablesForSageMakerServing\x12P\n\ronline_tables\x18\x01 \x03(\x0b\x32\x39.featurestorecommon.OnlineFeatureTableForSageMakerServing\"\xfe\x02\n%OnlineFeatureTableForSageMakerServing\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12H\n\x0conline_store\x18\x03 \x01(\x0b\x32\x32.featurestorecommon.OnlineStoreForSageMakerServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"\xbe\x01\n\x1eOnlineStoreForSageMakerServing\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x01 \x01(\x03\x12\x39\n\rdynamodb_conf\x18\x02 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x31\n\nquery_mode\x18\x10 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\x83\x01\n\x1c\x46\x65\x61tureFunctionParameterInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\ttype_text\x18\x02 \x01(\t\x12\x11\n\ttype_json\x18\x03 \x01(\t\x12/\n\ttype_name\x18\x04 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xdb\x01\n\x19\x46\x65\x61tureFunctionForServing\x12\x11\n\tfull_name\x18\x01 \x01(\t\x12\x46\n\x0cinput_params\x18\x02 \x03(\x0b\x32\x30.featurestorecommon.FeatureFunctionParameterInfo\x12/\n\tdata_type\x18\x03 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x16\n\x0e\x66ull_data_type\x18\x04 \x01(\t\x12\x1a\n\x12routine_definition\x18\x05 \x01(\t\"c\n\x1a\x46\x65\x61tureFunctionsForServing\x12\x45\n\x0e\x66\x66_for_serving\x18\x01 \x03(\x0b\x32-.featurestorecommon.FeatureFunctionForServing*$\n\x05\x43loud\x12\x07\n\x03\x41WS\x10\x01\x12\t\n\x05\x41ZURE\x10\x02\x12\x07\n\x03GCP\x10\x03*T\n\tStoreType\x12\x10\n\x0c\x41URORA_MYSQL\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\t\n\x05MYSQL\x10\x03\x12\x0c\n\x08\x44YNAMODB\x10\x04\x12\x0c\n\x08\x43OSMOSDB\x10\x05*\xa2\x01\n\x08\x44\x61taType\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x0b\n\x07\x42OOLEAN\x10\x03\x12\n\n\x06STRING\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\x08\n\x04LONG\x10\x06\x12\r\n\tTIMESTAMP\x10\x07\x12\x08\n\x04\x44\x41TE\x10\x08\x12\t\n\x05SHORT\x10\t\x12\t\n\x05\x41RRAY\x10\n\x12\x07\n\x03MAP\x10\x0b\x12\n\n\x06\x42INARY\x10\x0c\x12\x0b\n\x07\x44\x45\x43IMAL\x10\r*4\n\tQueryMode\x12\x16\n\x12PRIMARY_KEY_LOOKUP\x10\x00\x12\x0f\n\x0bRANGE_QUERY\x10\x01\x42\x31\n\'com.databricks.proto.featurestorecommon\xa0\x01\x01\xe2?\x02\x10\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x66\x65\x61ture_store_serving.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\"\x9b\x04\n\x15OnlineStoreForServing\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x1a\n\x12read_secret_prefix\x18\x03 \x01(\t\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x04 \x01(\x03\x12\x33\n\nmysql_conf\x18\x05 \x01(\x0b\x32\x1d.featurestorecommon.MySqlConfH\x00\x12<\n\x0fsql_server_conf\x18\x06 \x01(\x0b\x32!.featurestorecommon.SqlServerConfH\x00\x12\x39\n\rdynamodb_conf\x18\x07 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x39\n\rcosmosdb_conf\x18\x08 \x01(\x0b\x32 .featurestorecommon.CosmosDbConfH\x00\x12=\n\x0f\x62rickstore_conf\x18\t \x01(\x0b\x32\".featurestorecommon.BrickstoreConfH\x00\x12\x31\n\nquery_mode\x18\x15 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\'\n\tMySqlConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"+\n\rSqlServerConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x1e\n\x0c\x44ynamoDbConf\x12\x0e\n\x06region\x18\x01 \x01(\t\"#\n\x0c\x43osmosDbConf\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\",\n\x0e\x42rickstoreConf\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x0e\x46\x65\x61tureDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x19\n\x11\x64\x61ta_type_details\x18\x03 \x01(\t\"R\n\x11PrimaryKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"T\n\x13TimestampKeyDetails\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tdata_type\x18\x02 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xe2\x02\n\x12OnlineFeatureTable\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12?\n\x0conline_store\x18\x03 \x01(\x0b\x32).featurestorecommon.OnlineStoreForServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"X\n\x17\x46\x65\x61tureTablesForServing\x12=\n\ronline_tables\x18\x01 \x03(\x0b\x32&.featurestorecommon.OnlineFeatureTable\"+\n\rMySqlMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"/\n\x11SqlServerMetadata\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"B\n\x10\x44ynamoDbMetadata\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x11\n\ttable_arn\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"K\n\x10\x43osmosDbMetadata\x12\x13\n\x0b\x61\x63\x63ount_uri\x18\x01 \x01(\t\x12\x15\n\rcontainer_uri\x18\x02 \x01(\t\x12\x0b\n\x03ttl\x18\x03 \x01(\x03\"\xa9\x04\n\x0bOnlineStore\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12;\n\x0emysql_metadata\x18\n \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\x0b \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0c \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\r \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"\xdf\x04\n\x13OnlineStoreDetailed\x12(\n\x05\x63loud\x18\x01 \x01(\x0e\x32\x19.featurestorecommon.Cloud\x12\x31\n\nstore_type\x18\x02 \x01(\x0e\x32\x1d.featurestorecommon.StoreType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12\x63reation_timestamp\x18\x04 \x01(\x03\x12\x1e\n\x16last_updated_timestamp\x18\x05 \x01(\x03\x12\x12\n\ncreator_id\x18\x06 \x01(\t\x12\x10\n\x04host\x18\x07 \x01(\tB\x02\x18\x01\x12\x10\n\x04port\x18\x08 \x01(\x05\x42\x02\x18\x01\x12\x1b\n\x13last_update_user_id\x18\t \x01(\t\x12\x10\n\x08\x66\x65\x61tures\x18\n \x03(\t\x12\x1a\n\x12read_secret_prefix\x18\x0b \x01(\t\x12;\n\x0emysql_metadata\x18\x0c \x01(\x0b\x32!.featurestorecommon.MySqlMetadataH\x00\x12\x44\n\x13sql_server_metadata\x18\r \x01(\x0b\x32%.featurestorecommon.SqlServerMetadataH\x00\x12\x41\n\x11\x64ynamodb_metadata\x18\x0e \x01(\x0b\x32$.featurestorecommon.DynamoDbMetadataH\x00\x12\x41\n\x11\x63osmosdb_metadata\x18\x0f \x01(\x0b\x32$.featurestorecommon.CosmosDbMetadataH\x00\x42\x15\n\x13\x61\x64\x64itional_metadata\"t\n FeatureTablesForSageMakerServing\x12P\n\ronline_tables\x18\x01 \x03(\x0b\x32\x39.featurestorecommon.OnlineFeatureTableForSageMakerServing\"\xfe\x02\n%OnlineFeatureTableForSageMakerServing\x12\x1a\n\x12\x66\x65\x61ture_table_name\x18\x01 \x01(\t\x12!\n\x19online_feature_table_name\x18\x02 \x01(\t\x12H\n\x0conline_store\x18\x03 \x01(\x0b\x32\x32.featurestorecommon.OnlineStoreForSageMakerServing\x12;\n\x0cprimary_keys\x18\x04 \x03(\x0b\x32%.featurestorecommon.PrimaryKeyDetails\x12\x18\n\x10\x66\x65\x61ture_table_id\x18\x05 \x01(\t\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".featurestorecommon.FeatureDetails\x12?\n\x0etimestamp_keys\x18\x07 \x03(\x0b\x32\'.featurestorecommon.TimestampKeyDetails\"\xbe\x01\n\x1eOnlineStoreForSageMakerServing\x12\x1d\n\x15\x63reation_timestamp_ms\x18\x01 \x01(\x03\x12\x39\n\rdynamodb_conf\x18\x02 \x01(\x0b\x32 .featurestorecommon.DynamoDbConfH\x00\x12\x31\n\nquery_mode\x18\x10 \x01(\x0e\x32\x1d.featurestorecommon.QueryModeB\x0f\n\rextra_configs\"\x83\x01\n\x1c\x46\x65\x61tureFunctionParameterInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\ttype_text\x18\x02 \x01(\t\x12\x11\n\ttype_json\x18\x03 \x01(\t\x12/\n\ttype_name\x18\x04 \x01(\x0e\x32\x1c.featurestorecommon.DataType\"\xdb\x01\n\x19\x46\x65\x61tureFunctionForServing\x12\x11\n\tfull_name\x18\x01 \x01(\t\x12\x46\n\x0cinput_params\x18\x02 \x03(\x0b\x32\x30.featurestorecommon.FeatureFunctionParameterInfo\x12/\n\tdata_type\x18\x03 \x01(\x0e\x32\x1c.featurestorecommon.DataType\x12\x16\n\x0e\x66ull_data_type\x18\x04 \x01(\t\x12\x1a\n\x12routine_definition\x18\x05 \x01(\t\"c\n\x1a\x46\x65\x61tureFunctionsForServing\x12\x45\n\x0e\x66\x66_for_serving\x18\x01 \x03(\x0b\x32-.featurestorecommon.FeatureFunctionForServing*$\n\x05\x43loud\x12\x07\n\x03\x41WS\x10\x01\x12\t\n\x05\x41ZURE\x10\x02\x12\x07\n\x03GCP\x10\x03*d\n\tStoreType\x12\x10\n\x0c\x41URORA_MYSQL\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\t\n\x05MYSQL\x10\x03\x12\x0c\n\x08\x44YNAMODB\x10\x04\x12\x0c\n\x08\x43OSMOSDB\x10\x05\x12\x0e\n\nBRICKSTORE\x10\x06*\xa2\x01\n\x08\x44\x61taType\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x0b\n\x07\x42OOLEAN\x10\x03\x12\n\n\x06STRING\x10\x04\x12\n\n\x06\x44OUBLE\x10\x05\x12\x08\n\x04LONG\x10\x06\x12\r\n\tTIMESTAMP\x10\x07\x12\x08\n\x04\x44\x41TE\x10\x08\x12\t\n\x05SHORT\x10\t\x12\t\n\x05\x41RRAY\x10\n\x12\x07\n\x03MAP\x10\x0b\x12\n\n\x06\x42INARY\x10\x0c\x12\x0b\n\x07\x44\x45\x43IMAL\x10\r*4\n\tQueryMode\x12\x16\n\x12PRIMARY_KEY_LOOKUP\x10\x00\x12\x0f\n\x0bRANGE_QUERY\x10\x01\x42\x31\n\'com.databricks.proto.featurestorecommon\xa0\x01\x01\xe2?\x02\x10\x01')
 
 _CLOUD = DESCRIPTOR.enum_types_by_name['Cloud']
 Cloud = enum_type_wrapper.EnumTypeWrapper(_CLOUD)
 _STORETYPE = DESCRIPTOR.enum_types_by_name['StoreType']
 StoreType = enum_type_wrapper.EnumTypeWrapper(_STORETYPE)
 _DATATYPE = DESCRIPTOR.enum_types_by_name['DataType']
 DataType = enum_type_wrapper.EnumTypeWrapper(_DATATYPE)
@@ -30,14 +30,15 @@
 AZURE = 2
 GCP = 3
 AURORA_MYSQL = 1
 SQL_SERVER = 2
 MYSQL = 3
 DYNAMODB = 4
 COSMOSDB = 5
+BRICKSTORE = 6
 INTEGER = 1
 FLOAT = 2
 BOOLEAN = 3
 STRING = 4
 DOUBLE = 5
 LONG = 6
 TIMESTAMP = 7
@@ -52,14 +53,15 @@
 
 
 _ONLINESTOREFORSERVING = DESCRIPTOR.message_types_by_name['OnlineStoreForServing']
 _MYSQLCONF = DESCRIPTOR.message_types_by_name['MySqlConf']
 _SQLSERVERCONF = DESCRIPTOR.message_types_by_name['SqlServerConf']
 _DYNAMODBCONF = DESCRIPTOR.message_types_by_name['DynamoDbConf']
 _COSMOSDBCONF = DESCRIPTOR.message_types_by_name['CosmosDbConf']
+_BRICKSTORECONF = DESCRIPTOR.message_types_by_name['BrickstoreConf']
 _FEATUREDETAILS = DESCRIPTOR.message_types_by_name['FeatureDetails']
 _PRIMARYKEYDETAILS = DESCRIPTOR.message_types_by_name['PrimaryKeyDetails']
 _TIMESTAMPKEYDETAILS = DESCRIPTOR.message_types_by_name['TimestampKeyDetails']
 _ONLINEFEATURETABLE = DESCRIPTOR.message_types_by_name['OnlineFeatureTable']
 _FEATURETABLESFORSERVING = DESCRIPTOR.message_types_by_name['FeatureTablesForServing']
 _MYSQLMETADATA = DESCRIPTOR.message_types_by_name['MySqlMetadata']
 _SQLSERVERMETADATA = DESCRIPTOR.message_types_by_name['SqlServerMetadata']
@@ -104,14 +106,21 @@
 CosmosDbConf = _reflection.GeneratedProtocolMessageType('CosmosDbConf', (_message.Message,), {
   'DESCRIPTOR' : _COSMOSDBCONF,
   '__module__' : 'feature_store_serving_pb2'
   # @@protoc_insertion_point(class_scope:featurestorecommon.CosmosDbConf)
   })
 _sym_db.RegisterMessage(CosmosDbConf)
 
+BrickstoreConf = _reflection.GeneratedProtocolMessageType('BrickstoreConf', (_message.Message,), {
+  'DESCRIPTOR' : _BRICKSTORECONF,
+  '__module__' : 'feature_store_serving_pb2'
+  # @@protoc_insertion_point(class_scope:featurestorecommon.BrickstoreConf)
+  })
+_sym_db.RegisterMessage(BrickstoreConf)
+
 FeatureDetails = _reflection.GeneratedProtocolMessageType('FeatureDetails', (_message.Message,), {
   'DESCRIPTOR' : _FEATUREDETAILS,
   '__module__' : 'feature_store_serving_pb2'
   # @@protoc_insertion_point(class_scope:featurestorecommon.FeatureDetails)
   })
 _sym_db.RegisterMessage(FeatureDetails)
 
@@ -235,60 +244,62 @@
   _ONLINESTORE.fields_by_name['host']._serialized_options = b'\030\001'
   _ONLINESTORE.fields_by_name['port']._options = None
   _ONLINESTORE.fields_by_name['port']._serialized_options = b'\030\001'
   _ONLINESTOREDETAILED.fields_by_name['host']._options = None
   _ONLINESTOREDETAILED.fields_by_name['host']._serialized_options = b'\030\001'
   _ONLINESTOREDETAILED.fields_by_name['port']._options = None
   _ONLINESTOREDETAILED.fields_by_name['port']._serialized_options = b'\030\001'
-  _CLOUD._serialized_start=3991
-  _CLOUD._serialized_end=4027
-  _STORETYPE._serialized_start=4029
-  _STORETYPE._serialized_end=4113
-  _DATATYPE._serialized_start=4116
-  _DATATYPE._serialized_end=4278
-  _QUERYMODE._serialized_start=4280
-  _QUERYMODE._serialized_end=4332
+  _CLOUD._serialized_start=4100
+  _CLOUD._serialized_end=4136
+  _STORETYPE._serialized_start=4138
+  _STORETYPE._serialized_end=4238
+  _DATATYPE._serialized_start=4241
+  _DATATYPE._serialized_end=4403
+  _QUERYMODE._serialized_start=4405
+  _QUERYMODE._serialized_end=4457
   _ONLINESTOREFORSERVING._serialized_start=75
-  _ONLINESTOREFORSERVING._serialized_end=551
-  _MYSQLCONF._serialized_start=553
-  _MYSQLCONF._serialized_end=592
-  _SQLSERVERCONF._serialized_start=594
-  _SQLSERVERCONF._serialized_end=637
-  _DYNAMODBCONF._serialized_start=639
-  _DYNAMODBCONF._serialized_end=669
-  _COSMOSDBCONF._serialized_start=671
-  _COSMOSDBCONF._serialized_end=706
-  _FEATUREDETAILS._serialized_start=708
-  _FEATUREDETAILS._serialized_end=814
-  _PRIMARYKEYDETAILS._serialized_start=816
-  _PRIMARYKEYDETAILS._serialized_end=898
-  _TIMESTAMPKEYDETAILS._serialized_start=900
-  _TIMESTAMPKEYDETAILS._serialized_end=984
-  _ONLINEFEATURETABLE._serialized_start=987
-  _ONLINEFEATURETABLE._serialized_end=1341
-  _FEATURETABLESFORSERVING._serialized_start=1343
-  _FEATURETABLESFORSERVING._serialized_end=1431
-  _MYSQLMETADATA._serialized_start=1433
-  _MYSQLMETADATA._serialized_end=1476
-  _SQLSERVERMETADATA._serialized_start=1478
-  _SQLSERVERMETADATA._serialized_end=1525
-  _DYNAMODBMETADATA._serialized_start=1527
-  _DYNAMODBMETADATA._serialized_end=1593
-  _COSMOSDBMETADATA._serialized_start=1595
-  _COSMOSDBMETADATA._serialized_end=1670
-  _ONLINESTORE._serialized_start=1673
-  _ONLINESTORE._serialized_end=2226
-  _ONLINESTOREDETAILED._serialized_start=2229
-  _ONLINESTOREDETAILED._serialized_end=2836
-  _FEATURETABLESFORSAGEMAKERSERVING._serialized_start=2838
-  _FEATURETABLESFORSAGEMAKERSERVING._serialized_end=2954
-  _ONLINEFEATURETABLEFORSAGEMAKERSERVING._serialized_start=2957
-  _ONLINEFEATURETABLEFORSAGEMAKERSERVING._serialized_end=3339
-  _ONLINESTOREFORSAGEMAKERSERVING._serialized_start=3342
-  _ONLINESTOREFORSAGEMAKERSERVING._serialized_end=3532
-  _FEATUREFUNCTIONPARAMETERINFO._serialized_start=3535
-  _FEATUREFUNCTIONPARAMETERINFO._serialized_end=3666
-  _FEATUREFUNCTIONFORSERVING._serialized_start=3669
-  _FEATUREFUNCTIONFORSERVING._serialized_end=3888
-  _FEATUREFUNCTIONSFORSERVING._serialized_start=3890
-  _FEATUREFUNCTIONSFORSERVING._serialized_end=3989
+  _ONLINESTOREFORSERVING._serialized_end=614
+  _MYSQLCONF._serialized_start=616
+  _MYSQLCONF._serialized_end=655
+  _SQLSERVERCONF._serialized_start=657
+  _SQLSERVERCONF._serialized_end=700
+  _DYNAMODBCONF._serialized_start=702
+  _DYNAMODBCONF._serialized_end=732
+  _COSMOSDBCONF._serialized_start=734
+  _COSMOSDBCONF._serialized_end=769
+  _BRICKSTORECONF._serialized_start=771
+  _BRICKSTORECONF._serialized_end=815
+  _FEATUREDETAILS._serialized_start=817
+  _FEATUREDETAILS._serialized_end=923
+  _PRIMARYKEYDETAILS._serialized_start=925
+  _PRIMARYKEYDETAILS._serialized_end=1007
+  _TIMESTAMPKEYDETAILS._serialized_start=1009
+  _TIMESTAMPKEYDETAILS._serialized_end=1093
+  _ONLINEFEATURETABLE._serialized_start=1096
+  _ONLINEFEATURETABLE._serialized_end=1450
+  _FEATURETABLESFORSERVING._serialized_start=1452
+  _FEATURETABLESFORSERVING._serialized_end=1540
+  _MYSQLMETADATA._serialized_start=1542
+  _MYSQLMETADATA._serialized_end=1585
+  _SQLSERVERMETADATA._serialized_start=1587
+  _SQLSERVERMETADATA._serialized_end=1634
+  _DYNAMODBMETADATA._serialized_start=1636
+  _DYNAMODBMETADATA._serialized_end=1702
+  _COSMOSDBMETADATA._serialized_start=1704
+  _COSMOSDBMETADATA._serialized_end=1779
+  _ONLINESTORE._serialized_start=1782
+  _ONLINESTORE._serialized_end=2335
+  _ONLINESTOREDETAILED._serialized_start=2338
+  _ONLINESTOREDETAILED._serialized_end=2945
+  _FEATURETABLESFORSAGEMAKERSERVING._serialized_start=2947
+  _FEATURETABLESFORSAGEMAKERSERVING._serialized_end=3063
+  _ONLINEFEATURETABLEFORSAGEMAKERSERVING._serialized_start=3066
+  _ONLINEFEATURETABLEFORSAGEMAKERSERVING._serialized_end=3448
+  _ONLINESTOREFORSAGEMAKERSERVING._serialized_start=3451
+  _ONLINESTOREFORSAGEMAKERSERVING._serialized_end=3641
+  _FEATUREFUNCTIONPARAMETERINFO._serialized_start=3644
+  _FEATUREFUNCTIONPARAMETERINFO._serialized_end=3775
+  _FEATUREFUNCTIONFORSERVING._serialized_start=3778
+  _FEATUREFUNCTIONFORSERVING._serialized_end=3997
+  _FEATUREFUNCTIONSFORSERVING._serialized_start=3999
+  _FEATUREFUNCTIONSFORSERVING._serialized_end=4098
 # @@protoc_insertion_point(module_scope)
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/converter_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/converter_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_type_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/cosmosdb_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/data_type_details_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/data_type_details_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_type_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/dynamodb_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/feature_spec_test_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/feature_spec_test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from databricks.feature_store.entities.column_info import ColumnInfo
 from databricks.feature_store.entities.feature_column_info import FeatureColumnInfo
 from databricks.feature_store.entities.feature_spec import FeatureSpec
 from databricks.feature_store.entities.feature_table_info import FeatureTableInfo
 from databricks.feature_store.entities.function_info import FunctionInfo
 from databricks.feature_store.entities.on_demand_column_info import OnDemandColumnInfo
 
+# TODO (ML-30526): Move this file to the tests module.
+
 TEST_WORKSPACE_ID = 123
 
 
 def get_test_table_infos_from_column_infos(column_infos: List[ColumnInfo]):
     table_infos = []
     unique_table_names = set(
         [
@@ -33,16 +35,15 @@
             column_info.info.udf_name
             for column_info in column_infos
             if isinstance(column_info, ColumnInfo)
             and isinstance(column_info.info, OnDemandColumnInfo)
         ]
     )
     for udf_name in unique_udf_names:
-        md5 = udf_name + "_md5"
-        function_infos.append(FunctionInfo(udf_name=udf_name, md5=md5))
+        function_infos.append(FunctionInfo(udf_name=udf_name))
     return function_infos
 
 
 def create_test_feature_spec(
     column_infos: List[ColumnInfo],
     table_infos: List[FeatureTableInfo] = None,
     function_infos: List[FunctionInfo] = None,
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/metrics_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/pandas_type_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/pandas_type_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,45 +141,45 @@
         return int(value)
 
     @staticmethod
     @return_if_none
     @return_if_nan
     def to_pandas(value: Union[int, Decimal]) -> np.int16:
         # TODO (ML-20967): We currently return an np.int16 with best effort if there are no undefined values.
-        #  However, if a np.nan is provided, we will return np.nan which is a np.float instead.
+        #  However, if a np.nan is provided, we will return np.nan which is a float instead.
         return np.int16(value)
 
 
 # Integer
 class PandasIntTypeConverter(PandasStatelessConverter):
     @staticmethod
     def to_online_store(value: np.int32) -> int:
         return int(value)
 
     @staticmethod
     @return_if_none
     @return_if_nan
     def to_pandas(value: Union[int, Decimal]) -> np.int32:
         # TODO (ML-20967): We currently return an np.int32 with best effort if there are no undefined values.
-        #  However, if a np.nan is provided, we will return np.nan which is a np.float instead.
+        #  However, if a np.nan is provided, we will return np.nan which is a float instead.
         return np.int32(value)
 
 
 # Long
 class PandasLongTypeConverter(PandasStatelessConverter):
     @staticmethod
     def to_online_store(value: np.int64) -> int:
         return int(value)
 
     @staticmethod
     @return_if_none
     @return_if_nan
     def to_pandas(value: Union[int, Decimal]) -> np.int64:
         # TODO (ML-20967): We currently return an np.int64 with best effort if there are no undefined values.
-        #  However, if a np.nan is provided, we will return np.nan which is a np.float instead.
+        #  However, if a np.nan is provided, we will return np.nan which is a float instead.
         return np.int64(value)
 
 
 # String
 class PandasStringTypeConverter(PandasStatelessConverter):
     @staticmethod
     def to_online_store(value: str) -> str:
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/serving_test_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/serving_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/sql_type_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/sql_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/uc_utils.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/uc_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,120 @@
 import copy
 import re
-from typing import List, Set
+from typing import Set
 
 from databricks.feature_store.entities.feature_spec import FeatureSpec
 
-SINGLE_LEVEL_NAMESPACE_TABLE_REGEX = r"^[\w_]+$"
-TWO_LEVEL_NAMESPACE_TABLE_REGEX = r"^[\w_]+(\.[\w_]+)$"
-THREE_LEVEL_NAMESPACE_TABLE_REGEX = r"^[\w_]+(\.[\w_]+){2}$"
+SINGLE_LEVEL_NAMESPACE_REGEX = r"^[\w_]+$"
+TWO_LEVEL_NAMESPACE_REGEX = r"^[\w_]+(\.[\w_]+)$"
+THREE_LEVEL_NAMESPACE_REGEX = r"^[\w_]+(\.[\w_]+){2}$"
 
 HIVE_METASTORE_NAME = "hive_metastore"
 # these two catalog names both points to the workspace local default HMS (hive metastore).
 LOCAL_METASTORE_NAMES = [HIVE_METASTORE_NAME, "spark_catalog"]
 # samples catalog is managed by databricks for hosting public dataset like NYC taxi dataset.
 # it is neither a UC nor local metastore catalog, accessing samples catalog using feature store client is not allowed.
 SAMPLES_CATALOG_NAME = "samples"
 
 
-# Get full table name in the form of <catalog_name>.<database_name>.<table_name>
+# Get full table name in the form of <catalog_name>.<schema_name>.<table_name>
 # given user specified table name, current catalog and schema.
 def get_full_table_name(
     table_name: str,
     current_catalog: str,
     current_schema: str,
 ) -> str:
+    _check_qualified_table_names({table_name})
+    return _get_full_name_for_entity(
+        name=table_name,
+        current_catalog=current_catalog,
+        current_schema=current_schema,
+        entity_type="table",
+    )
+
+
+# Get full UDF name in the form of <catalog_name>.<schema_name>.<udf_name>
+# given user specified UDF name, current catalog and schema.
+def get_full_udf_name(
+    udf_name: str,
+    current_catalog: str,
+    current_schema: str,
+) -> str:
+    _check_qualified_udf_names({udf_name})
+    return _get_full_name_for_entity(
+        name=udf_name,
+        current_catalog=current_catalog,
+        current_schema=current_schema,
+        entity_type="UDF",
+    )
+
+
+def _get_full_name_for_entity(
+    name: str,
+    current_catalog: str,
+    current_schema: str,
+    entity_type: str,
+) -> str:
     if not _is_single_level_name(current_catalog) or not _is_single_level_name(
         current_schema
     ):
         raise ValueError(
             f"Invalid catalog '{current_catalog}' or "
-            f"schema '{current_schema}' name for table '{table_name}'."
+            f"schema '{current_schema}' name for {entity_type} '{name}'."
         )
-    _check_qualified_names({table_name})
-    if _is_single_level_name(table_name):
-        full_table_name = f"{current_catalog}.{current_schema}.{table_name}"
-    elif _is_two_level_name(table_name):
-        full_table_name = f"{current_catalog}.{table_name}"
-    elif _is_three_level_name(table_name):
-        full_table_name = table_name
+    if _is_single_level_name(name):
+        full_name = f"{current_catalog}.{current_schema}.{name}"
+    elif _is_two_level_name(name):
+        full_name = f"{current_catalog}.{name}"
+    elif _is_three_level_name(name):
+        full_name = name
     else:
-        raise _invalid_table_names_error({table_name})
-    catalog, schema, table = full_table_name.split(".")
+        raise _invalid_names_error({name}, entity_type)
+
+    catalog, schema, name = full_name.split(".")
     if catalog == SAMPLES_CATALOG_NAME:
         raise ValueError(
             "'samples' catalog cannot be accessed using feature store client."
         )
     if catalog in LOCAL_METASTORE_NAMES:
-        return f"{HIVE_METASTORE_NAME}.{schema}.{table}"
-    return full_table_name
+        return f"{HIVE_METASTORE_NAME}.{schema}.{name}"
+    return full_name
 
 
 # Local metastore tables in feature_spec.yaml are all stored in 2L.
 # Standardize table names to be all in 3L to avoid erroneously reading data from UC tables.
 def get_feature_spec_with_full_table_names(feature_spec: FeatureSpec) -> FeatureSpec:
     column_info_table_names = [
         column_info.table_name for column_info in feature_spec.feature_column_infos
     ]
     table_info_table_names = [
         table_info.table_name for table_info in feature_spec.table_infos
     ]
-    _check_qualified_names(set(column_info_table_names))
-    _check_qualified_names(set(table_info_table_names))
+    _check_qualified_table_names(set(column_info_table_names))
+    _check_qualified_table_names(set(table_info_table_names))
     invalid_table_names = list(
         filter(_is_single_level_name, column_info_table_names)
     ) + list(filter(_is_single_level_name, table_info_table_names))
     if len(invalid_table_names) > 0:
-        raise _invalid_table_names_error(set(invalid_table_names))
+        raise _invalid_names_error(set(invalid_table_names), "table")
     standardized_feature_spec = copy.deepcopy(feature_spec)
     for column_info in standardized_feature_spec.feature_column_infos:
         if _is_two_level_name(column_info.table_name):
             column_info._table_name = f"{HIVE_METASTORE_NAME}.{column_info.table_name}"
     for table_info in standardized_feature_spec.table_infos:
         if _is_two_level_name(table_info.table_name):
             table_info._table_name = f"{HIVE_METASTORE_NAME}.{table_info.table_name}"
     return standardized_feature_spec
 
 
 # Reformat 3L table name for tables in local metastore to 2L. This is used when interacting with catalog client
 # and serializing workspace local feature spec for scoring.
 def reformat_full_table_name(full_table_name: str) -> str:
     if not _is_three_level_name(full_table_name):
-        raise _invalid_table_names_error({full_table_name})
+        raise _invalid_names_error({full_table_name}, "table")
     catalog, schema, table = full_table_name.split(".")
     if catalog in LOCAL_METASTORE_NAMES:
         return f"{schema}.{table}"
     return full_table_name
 
 
 # Reformat table names in feature_spec with reformat_full_table_name
@@ -92,94 +123,107 @@
 ) -> FeatureSpec:
     column_info_table_names = [
         column_info.table_name for column_info in feature_spec.feature_column_infos
     ]
     table_info_table_names = [
         table_info.table_name for table_info in feature_spec.table_infos
     ]
-    _check_qualified_names(set(column_info_table_names))
-    _check_qualified_names(set(table_info_table_names))
+    _check_qualified_table_names(set(column_info_table_names))
+    _check_qualified_table_names(set(table_info_table_names))
     invalid_table_names = list(
         filter(lambda name: not _is_three_level_name(name), column_info_table_names)
     ) + list(
         filter(lambda name: not _is_three_level_name(name), table_info_table_names)
     )
     if len(invalid_table_names) > 0:
-        raise _invalid_table_names_error(set(invalid_table_names))
+        raise _invalid_names_error(set(invalid_table_names), "table")
     standardized_feature_spec = copy.deepcopy(feature_spec)
     for column_info in standardized_feature_spec.feature_column_infos:
         column_info._table_name = reformat_full_table_name(column_info.table_name)
     for table_info in standardized_feature_spec.table_infos:
         table_info._table_name = reformat_full_table_name(table_info.table_name)
     return standardized_feature_spec
 
 
-def _invalid_table_names_error(invalid_table_names: Set[str]) -> ValueError:
+def _invalid_names_error(invalid_names: Set[str], entity_type: str) -> ValueError:
     return ValueError(
-        f"Invalid table name{'s' if len(invalid_table_names) > 1 else ''} '{', '.join(invalid_table_names)}'."
+        f"Invalid {entity_type} name{'s' if len(invalid_names) > 1 else ''} '{', '.join(invalid_names)}'."
     )
 
 
-def _is_qualified_table_name(feature_table_name) -> bool:
-    return isinstance(feature_table_name, str) and (
-        _is_single_level_name(feature_table_name)
-        or _is_two_level_name(feature_table_name)
-        or _is_three_level_name(feature_table_name)
+def _is_qualified_entity_name(name) -> bool:
+    return isinstance(name, str) and (
+        _is_single_level_name(name)
+        or _is_two_level_name(name)
+        or _is_three_level_name(name)
     )
 
 
 def _is_single_level_name(name) -> bool:
     return (
         isinstance(name, str)
-        and re.match(SINGLE_LEVEL_NAMESPACE_TABLE_REGEX, name) is not None
+        and re.match(SINGLE_LEVEL_NAMESPACE_REGEX, name) is not None
     )
 
 
 def _is_two_level_name(name) -> bool:
     return (
-        isinstance(name, str)
-        and re.match(TWO_LEVEL_NAMESPACE_TABLE_REGEX, name) is not None
+        isinstance(name, str) and re.match(TWO_LEVEL_NAMESPACE_REGEX, name) is not None
     )
 
 
 def _is_three_level_name(name) -> bool:
     return (
         isinstance(name, str)
-        and re.match(THREE_LEVEL_NAMESPACE_TABLE_REGEX, name) is not None
+        and re.match(THREE_LEVEL_NAMESPACE_REGEX, name) is not None
     )
 
 
 def tagging_for_uc_tables_error(full_table_name):
     return ValueError(
         f"Cannot set or delete tags for table {full_table_name}. "
         f"Tagging for Feature Tables in Unity Catalog is not yet supported."
     )
 
 
-# check if table is in UC
-def is_uc_table(full_table_name) -> bool:
-    catalog_name, schema_name, table_name = full_table_name.split(".")
+# check if entity is in UC and not in samples catalog
+def is_uc_entity(full_entity_name) -> bool:
+    catalog_name, schema_name, table_name = full_entity_name.split(".")
     return (
-        not is_default_hms_table(full_table_name)
+        not is_default_hms_table(full_entity_name)
         and catalog_name != SAMPLES_CATALOG_NAME
     )
 
 
 def is_default_hms_table(full_table_name) -> bool:
     catalog_name, schema_name, table_name = full_table_name.split(".")
     return (
         catalog_name in LOCAL_METASTORE_NAMES and catalog_name != SAMPLES_CATALOG_NAME
     )
 
 
+# check if UDF names are in the correct format - 1L, 2L or 3L
+def _check_qualified_udf_names(udf_names: Set[str]):
+    unqualified_udf_names = [
+        udf_name for udf_name in udf_names if not _is_qualified_entity_name(udf_name)
+    ]
+    if len(unqualified_udf_names) > 0:
+        raise ValueError(
+            f"UDF name{'s' if len(unqualified_udf_names) > 1 else ''} "
+            f"'{', '.join(map(str, unqualified_udf_names))}' must have the form "
+            f"<catalog_name>.<schema_name>.<udf_name>, <schema_name>.<udf_name>, "
+            f"or <udf_name> and only contain alphabet characters, numbers and _."
+        )
+
+
 # check if table names are in the correct format - 1L, 2L or 3L
-def _check_qualified_names(feature_table_names: Set[str]):
+def _check_qualified_table_names(feature_table_names: Set[str]):
     unqualified_table_names = list(
         filter(
-            lambda table_name: not _is_qualified_table_name(table_name),
+            lambda table_name: not _is_qualified_entity_name(table_name),
             feature_table_names,
         )
     )
     if len(unqualified_table_names) > 0:
         raise ValueError(
             f"Feature table name{'s' if len(unqualified_table_names) > 1 else ''} "
             f"'{', '.join(map(str, unqualified_table_names))}' must have the form "
@@ -190,28 +234,35 @@
 
 # For APIs like create_training_set and score_batch, all tables must all be in
 # UC catalog (shareable cross-workspaces) or default HMS (intended to only be used in the current workspace)
 # check if all tables are either in UC or default HMS.
 def _verify_all_tables_are_either_in_uc_or_in_hms(
     table_names: Set[str], current_catalog: str, current_schema: str
 ):
+    full_table_names = [
+        get_full_table_name(table_name, current_catalog, current_schema)
+        for table_name in table_names
+    ]
     is_valid = all(
-        map(
-            lambda table_name: is_uc_table(
-                get_full_table_name(table_name, current_catalog, current_schema)
-            ),
-            table_names,
-        )
+        [is_uc_entity(full_table_name) for full_table_name in full_table_names]
     ) or all(
-        map(
-            lambda table_name: is_default_hms_table(
-                get_full_table_name(table_name, current_catalog, current_schema)
-            ),
-            table_names,
-        )
+        [is_default_hms_table(full_table_name) for full_table_name in full_table_names]
     )
     if not is_valid:
         raise ValueError(
             f"Feature table names '{', '.join(table_names)}' "
             f"must all be in UC or the local default hive metastore. "
             f"Mixing feature tables from two different storage locations is not allowed."
         )
+
+
+# For APIs like create_training_set with FeatureFunctions, only UC UDFs are supported.
+def _verify_all_udfs_in_uc(
+    udf_names: Set[str], current_catalog: str, current_schema: str
+):
+    full_udf_names = [
+        get_full_udf_name(udf_name, current_catalog, current_schema)
+        for udf_name in udf_names
+    ]
+    is_valid = all([is_uc_entity(full_udf_name) for full_udf_name in full_udf_names])
+    if not is_valid:
+        raise ValueError(f"UDFs must all be in Unity Catalog.")
```

### Comparing `databricks-feature-lookup-0.4.1/databricks/feature_store/utils/utils_common.py` & `databricks-feature-lookup-0.5.0/databricks/feature_store/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/databricks_feature_lookup.egg-info/PKG-INFO` & `databricks-feature-lookup-0.5.0/databricks_feature_lookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.4.1
+Version: 0.5.0
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.4.1/setup.py` & `databricks-feature-lookup-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.4.1/tests/test_mlflow_model.py` & `databricks-feature-lookup-0.5.0/tests/test_mlflow_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 To run this test:
   pytest tests/test_mlflow_model.py
 """
 
 import io
 import os
 import sys
+from datetime import datetime
 from typing import List, Tuple
 from unittest.mock import ANY, MagicMock, patch
 
 import mlflow
 import numpy as np
 import pandas as pd
 import pytest
 
 from databricks.feature_store import mlflow_model
 from databricks.feature_store.entities.cloud import Cloud
 from databricks.feature_store.entities.column_info import ColumnInfo
 from databricks.feature_store.entities.data_type import DataType
 from databricks.feature_store.entities.feature_column_info import FeatureColumnInfo
+from databricks.feature_store.entities.feature_functions_for_serving import (
+    FeatureFunctionForServing,
+    FeatureFunctionParameterInfo,
+    FeatureFunctionsForServing,
+)
 from databricks.feature_store.entities.feature_table_info import FeatureTableInfo
 from databricks.feature_store.entities.feature_tables_for_serving import (
     FeatureTablesForSageMakerServing,
     FeatureTablesForServing,
 )
+from databricks.feature_store.entities.on_demand_column_info import OnDemandColumnInfo
 from databricks.feature_store.entities.online_feature_table import (
     FeatureDetails,
     OnlineFeatureTable,
     PrimaryKeyDetails,
 )
 from databricks.feature_store.entities.online_store_for_serving import (
     DynamoDbConf,
@@ -655,14 +662,19 @@
 @pytest.fixture(scope="function")
 def feature_spec_basic(ci_for_feature1, feature_table_info1):
     return create_test_feature_spec(
         column_infos=[ci_for_feature1], table_infos=[feature_table_info1]
     )
 
 
+@pytest.fixture(scope="function")
+def feature_spec_no_features(ci_for_source_data1):
+    return create_test_feature_spec(column_infos=[ci_for_source_data1], table_infos=[])
+
+
 @pytest.fixture(scope="module")
 def feature_spec_basic_default_metastore(
     ci_for_feature1_3_level_default_hive_metastore,
     feature_table_info1_3_level_default_hive_metastore,
 ):
     return create_test_feature_spec(
         column_infos=[ci_for_feature1_3_level_default_hive_metastore],
@@ -767,15 +779,15 @@
     fixtures defined above. It may remain unused in a test case.
     """
     feature_spec_load.return_value = feature_spec_advanced
     feature_tables_for_serving_load.return_value = feature_tables_for_serving_advanced
 
 
 @pytest.fixture(scope="function")
-def lookup_client_basic(online_feature_table1, online_feature_table2):
+def lookup_client_basic():
     with patch("databricks.feature_store.mlflow_model.OnlineLookupClient") as mock:
         yield mock.return_value
         return
 
 
 @pytest.fixture(scope="function")
 def lookup_client_advanced(online_feature_table1, online_feature_table2):
@@ -881,14 +893,18 @@
                 )
 
         mock.side_effect = mock_constructor
         yield (lookup_client1, lookup_client2)
         return
 
 
+def enable_feature_function_evaluation(self):
+    return True
+
+
 ##### Tests
 
 ## Tests: _load_pyfunc succeeds
 
 
 @pytest.mark.parametrize(
     "feature_spec_yaml", ["feature_spec_basic", "feature_spec_basic_default_metastore"]
@@ -1092,14 +1108,29 @@
     assert list(actual_ft_to_lookup_client.keys()) == ["test.ft1", "test.ft2"]
 
     feature_tables_for_serving_load.assert_called_once_with(path="/tmp/abc")
     pyfunc_model_load.assert_called_once_with(f"{MODEL_URI}/raw_model")
     feature_spec_load.assert_called_once_with(MODEL_URI)
 
 
+def test_load_no_features(
+    feature_spec_load,
+    feature_spec_no_features,
+    feature_tables_for_serving_load,
+    sum_features_model,
+):
+    feature_spec_load.return_value = feature_spec_no_features
+    feature_tables_for_serving_load.return_value = FeatureTablesForServing(
+        online_feature_tables=[]
+    )
+    loaded_model = mlflow_model._load_pyfunc(MODEL_URI)
+    assert loaded_model.feature_spec == feature_spec_no_features
+    assert loaded_model.raw_model == sum_features_model
+
+
 ## Tests: test batch lookup behavior
 # TODO: eventually this should be replaced with more end-to-end behavior once batching implemented rather than calling "private" method
 
 # if all feature tables are dynamo db, should be eligible for batch feature lookup
 @patch.dict(
     os.environ,
     {
@@ -1627,39 +1658,52 @@
     lookup_client_batch.batch_lookup_features.return_value = batch_lookup_values
     prediction = fs_model.predict(input_df)
 
     assert prediction.attrs[OVERRIDEN_FEATURE_COUNT] == overridden_feature_count
     assert list(prediction) == prediction_result
 
 
+@pytest.mark.parametrize(
+    "ff_enabled", [True, False]
+)  # <-- # Model initialization and prediction
+# on non-FF packaged models should work regardless of whether FEATURE_FUNCTION_EVALUATION_ENABLED.
 def test_predict_advanced(
     advanced_setup,
     lookup_client_advanced,
+    ff_enabled,
 ):
-    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
-    df = pd.DataFrame({"user_id": [123], "product_id": [555], "session_duration": [77]})
-    lookup_client1, lookup_client2 = lookup_client_advanced
-    lookup_client1.lookup_features.return_value = pd.DataFrame({"age": [55]})
-    lookup_client2.lookup_features.return_value = pd.DataFrame(
-        {"num_purchases": [3], "rating": [4.2]}
-    )
-    prediction = fs_model.predict(df)
-
-    lookup_client1.lookup_features.assert_called_once_with(ANY, ["age"], metrics=ANY)
-    pd.testing.assert_frame_equal(
-        lookup_client1.lookup_features.call_args[0][0], pd.DataFrame({"pk": [123]})
-    )
-
-    lookup_client2.lookup_features.assert_called_once_with(
-        ANY, ["num_purchases", "rating"], metrics=ANY
-    )
-    pd.testing.assert_frame_equal(
-        lookup_client2.lookup_features.call_args[0][0], pd.DataFrame({"pk": [555]})
-    )
-    assert prediction == [55 + 3 + 4.2 + 77]
+    with patch(
+        "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+        lambda self: ff_enabled,
+    ):
+        fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+        df = pd.DataFrame(
+            {"user_id": [123], "product_id": [555], "session_duration": [77]}
+        )
+        lookup_client1, lookup_client2 = lookup_client_advanced
+        lookup_client1.lookup_features.return_value = pd.DataFrame({"age": [55]})
+        lookup_client2.lookup_features.return_value = pd.DataFrame(
+            {"num_purchases": [3], "rating": [4.2]}
+        )
+        prediction = fs_model.predict(df)
+
+        lookup_client1.lookup_features.assert_called_once_with(
+            ANY, ["age"], metrics=ANY
+        )
+        pd.testing.assert_frame_equal(
+            lookup_client1.lookup_features.call_args[0][0], pd.DataFrame({"pk": [123]})
+        )
+
+        lookup_client2.lookup_features.assert_called_once_with(
+            ANY, ["num_purchases", "rating"], metrics=ANY
+        )
+        pd.testing.assert_frame_equal(
+            lookup_client2.lookup_features.call_args[0][0], pd.DataFrame({"pk": [555]})
+        )
+        assert prediction == [55 + 3 + 4.2 + 77]
 
 
 def test_predict_multiple_rows(basic_setup, lookup_client_basic):
     fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
     df = pd.DataFrame({"user_id": [123, 456]})
     lookup_client_basic.lookup_features.return_value = pd.DataFrame({"age": [55, 32]})
     prediction = fs_model.predict(df)
@@ -1747,15 +1791,14 @@
     np.testing.assert_array_equal(prediction, [55 + 4.2 + 15 + 7, 66 + 3.1 + 22 + 10])
 
 
 def test_predict_override_advanced(
     advanced_setup,
     lookup_client_advanced,
 ):
-
     fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
     df = pd.DataFrame(
         {
             "user_id": [123, 456],
             "product_id": [555, 666],
             "age": [np.nan, 47],  # <-- override "age" for only some rows
             "num_purchases": [
@@ -1810,14 +1853,32 @@
     )
     pd.testing.assert_frame_equal(
         lookup_client_basic.lookup_features.call_args[0][0], pd.DataFrame({"pk": [123]})
     )
     assert prediction == [55]
 
 
+def test_predict_no_features(
+    feature_spec_load,
+    feature_spec_no_features,
+    feature_tables_for_serving_load,
+    sum_features_model,
+):
+    feature_spec_load.return_value = feature_spec_no_features
+    feature_tables_for_serving_load.return_value = FeatureTablesForServing(
+        online_feature_tables=[]
+    )
+
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+
+    df = pd.DataFrame({"session_duration": [500]})
+    prediction = fs_model.predict(df)
+    assert prediction == [500]
+
+
 ## Tests: predict fails
 
 
 def test_predict_missing_source_data_column_info(
     advanced_setup, lookup_client_advanced
 ):
     fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
@@ -1891,7 +1952,667 @@
     # 2 rows in input
     df = pd.DataFrame({"user_id": [123, 456]})
     # lookup_client only returns 1 row
     lookup_client_basic.lookup_features.return_value = pd.DataFrame({"age": [55]})
     with pytest.raises(Exception) as e:
         fs_model.predict(df)
     assert "Expected 2 rows to be looked up" in str(e)
+
+
+##### Feature Function Integration Tests
+# TODO(ML-30606): Migrate to separate file
+
+
+@pytest.fixture(scope="module")
+def feature_function_for_serving_2x():
+    input_param = FeatureFunctionParameterInfo(
+        type_text="integer",
+        type_json="""{\"name\":\"x\",\"type\":\"integer\",\"nullable\":true,\"metadata\":{}}""",
+        name="x",
+        type_name=DataType.INTEGER,
+    )
+    return FeatureFunctionForServing(
+        full_name="cat.sch.times_two",
+        input_params=[input_param],
+        data_type=DataType.INTEGER,
+        full_data_type="INTEGER",
+        routine_definition="\n\nreturn 2*x",
+    )
+
+
+@pytest.fixture(scope="module")
+def feature_function_for_serving_plus_1():
+    input_param = FeatureFunctionParameterInfo(
+        type_text="integer",
+        type_json="""{\"name\":\"x\",\"type\":\"integer\",\"nullable\":true,\"metadata\":{}}""",
+        name="x",
+        type_name=DataType.INTEGER,
+    )
+    return FeatureFunctionForServing(
+        full_name="cat.sch.plus_1",
+        input_params=[input_param],
+        data_type=DataType.INTEGER,
+        full_data_type="INTEGER",
+        routine_definition="\n\nreturn x+1",
+    )
+
+
+@pytest.fixture(scope="module")
+def feature_functions_for_serving_basic(feature_function_for_serving_2x):
+    return FeatureFunctionsForServing(ff_for_serving=[feature_function_for_serving_2x])
+
+
+@pytest.fixture(scope="function")
+def feature_functions_for_serving_load():
+    with patch(
+        "databricks.feature_store.entities.feature_functions_for_serving.FeatureFunctionsForServing.load"
+    ) as mock:
+        yield mock
+        return
+
+
+@pytest.fixture(scope="function")
+def is_file():
+    with patch("os.path.isfile") as mock:
+        yield mock
+        return
+
+
+@pytest.fixture(scope="function")
+def odci_age_2x():
+    return ColumnInfo(
+        info=OnDemandColumnInfo(
+            udf_name="cat.sch.times_two",
+            input_bindings={"x": "age"},
+            output_name="age_times_2_output",
+        ),
+        include=True,
+    )
+
+
+@pytest.fixture(scope="function")
+def odci_age_plus_1():
+    return ColumnInfo(
+        info=OnDemandColumnInfo(
+            udf_name="cat.sch.plus_1",
+            input_bindings={"x": "age"},
+            output_name="age_plus_1_output",
+        ),
+        include=True,
+    )
+
+
+@pytest.fixture(scope="module")
+def ci_for_feature_age():
+    return ColumnInfo(
+        info=FeatureColumnInfo(
+            table_name="test.ft1",
+            feature_name="age",
+            lookup_key=["user_id"],
+            output_name="age",
+        ),
+        include=False,
+    )
+
+
+@pytest.fixture(scope="function")
+def feature_spec_with_odci_fci_excluded(
+    ci_for_feature1, feature_table_info1, odci_age_2x, ci_for_feature_age
+):
+    return create_test_feature_spec(
+        column_infos=[odci_age_2x, ci_for_feature_age],
+        table_infos=[feature_table_info1],
+    )
+
+
+@pytest.fixture(scope="function")
+def on_demand_setup(
+    feature_spec_load,
+    feature_spec_with_odci_fci_excluded,
+    feature_tables_for_serving_load,
+    feature_tables_for_serving_basic,
+    is_file,
+):
+    """
+    This fixture can be passed to a test function to patch FeatureSpec.load and
+    FeatureTablesForServing.load to return the basic feature_spec and feature_tables_for_serving
+    fixtures defined above. It may remain unused in a test case.
+    """
+    feature_spec_load.return_value = feature_spec_with_odci_fci_excluded
+    feature_tables_for_serving_load.return_value = feature_tables_for_serving_basic
+    is_file.side_effect = lambda path: path == os.path.join(
+        MODEL_URI, "_databricks_internal/feature_functions_for_serving.dat"
+    )
+
+
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+def test_predict_with_on_demand_basic(
+    on_demand_setup,
+    lookup_client_basic,
+    feature_functions_for_serving_basic,
+    feature_functions_for_serving_load,
+):
+    """
+    This test validates a simple codepath where a single feature is looked up in order to compute
+    a Feature Function.
+    """
+    feature_functions_for_serving_load.return_value = (
+        feature_functions_for_serving_basic
+    )
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    df = pd.DataFrame({"user_id": [123, 456]})
+    lookup_client_basic.lookup_features.return_value = pd.DataFrame({"age": [55, 32]})
+    prediction = fs_model.predict(df)
+
+    lookup_client_basic.lookup_features.assert_called_once_with(
+        ANY, ["age"], metrics=ANY
+    )
+    pd.testing.assert_frame_equal(
+        lookup_client_basic.lookup_features.call_args[0][0],
+        pd.DataFrame({"pk": [123, 456]}),
+    )
+    assert list(prediction) == [55 * 2, 32 * 2]  # Feature Function multiplies age by 2
+
+
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+def test_predict_no_materialized_features(
+    feature_spec_load,
+    odci_age_2x_age2,
+    ci_for_age2_source,
+    is_file,
+    feature_functions_for_serving_basic,
+    feature_functions_for_serving_load,
+    feature_tables_for_serving_load,
+):
+    """
+    This test validates a simple codepath where a single feature is looked up in order to compute
+    a Feature Function.
+    """
+    feature_spec_load.return_value = create_test_feature_spec(
+        column_infos=[odci_age_2x_age2, ci_for_age2_source]
+    )
+    is_file.side_effect = lambda path: path == os.path.join(
+        MODEL_URI, "_databricks_internal/feature_functions_for_serving.dat"
+    )
+    feature_functions_for_serving_load.return_value = (
+        feature_functions_for_serving_basic
+    )
+    feature_tables_for_serving_load.return_value = FeatureTablesForServing(
+        online_feature_tables=[]
+    )
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    df = pd.DataFrame({"age2": [3, 33]})
+    prediction = fs_model.predict(df)
+
+    assert list(prediction) == [3 * 2, 33 * 2]  # Feature Function multiplies age2 by 2
+
+
+# Override the FeatureColumnInfo passed as input to an on-demand function
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+def test_predict_with_on_demand_override_inputs(
+    on_demand_setup,
+    lookup_client_basic,
+    feature_functions_for_serving_basic,
+    feature_functions_for_serving_load,
+):
+    feature_functions_for_serving_load.return_value = (
+        feature_functions_for_serving_basic
+    )
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    df = pd.DataFrame({"user_id": [123, 456], "age": [100, 101]})
+    prediction = fs_model.predict(df)
+
+    assert list(prediction) == [(100 * 2), (101 * 2)]
+
+
+# Override the output of the Feature Function
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+def test_predict_override_on_demand(
+    on_demand_setup,
+    lookup_client_basic,
+    feature_functions_for_serving_basic,
+    feature_functions_for_serving_load,
+):
+    feature_functions_for_serving_load.return_value = (
+        feature_functions_for_serving_basic
+    )
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    df = pd.DataFrame({"user_id": [123, 456], "age_times_2_output": [100, 200]})
+    # TODO(ML-30619): Skipping lookup is not yet implemented.
+    lookup_client_basic.lookup_features.return_value = pd.DataFrame({"age": [55, 32]})
+    prediction = fs_model.predict(df)
+    assert list(prediction) == [100, 200]
+
+
+# Override the Feature Function output in one of two rows.
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+def test_predict_partial_override_on_demand(
+    on_demand_setup,
+    lookup_client_basic,
+    feature_functions_for_serving_basic,
+    feature_functions_for_serving_load,
+):
+    feature_functions_for_serving_load.return_value = (
+        feature_functions_for_serving_basic
+    )
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    df = pd.DataFrame(
+        {
+            "user_id": [123, 456],
+            "age_times_2_output": [
+                100,
+                np.nan,
+            ],  # <-- override "age_times_2_output" for only some rows
+        }
+    )
+    # Skipping lookup is not yet implemented
+    lookup_client_basic.lookup_features.return_value = pd.DataFrame({"age": [55, 32]})
+    prediction = fs_model.predict(df)
+    assert list(prediction) == [100, 32 * 2]
+
+
+@pytest.fixture(scope="module")
+def feature_function_for_serving_float2str():
+    input_param = FeatureFunctionParameterInfo(
+        type_text="float",
+        type_json="""{\"name\":\"x\",\"type\":\"integer\",\"nullable\":true,\"metadata\":{}}""",
+        name="x",
+        type_name=DataType.STRING,
+    )
+    return FeatureFunctionForServing(
+        full_name="cat.sch2.float_to_string",
+        input_params=[input_param],
+        data_type=DataType.STRING,
+        full_data_type="STRING",
+        routine_definition="\n\nreturn x",
+    )
+
+
+@pytest.fixture(scope="module")
+def feature_function_for_serving_date():
+    return FeatureFunctionForServing(
+        full_name="cat.sch.timestamp",
+        input_params=[],
+        data_type=DataType.TIMESTAMP,
+        full_data_type="TIMESTAMP",
+        routine_definition="\nfrom datetime import datetime\nreturn datetime(year=2000, month=1, day=1)\n",
+    )
+
+
+@pytest.fixture(scope="module")
+def feature_functions_for_serving_advanced(
+    feature_function_for_serving_2x,
+    feature_function_for_serving_float2str,
+    feature_function_for_serving_date,
+    feature_function_for_serving_plus_1,
+):
+    return FeatureFunctionsForServing(
+        ff_for_serving=[
+            feature_function_for_serving_2x,
+            feature_function_for_serving_float2str,
+            feature_function_for_serving_date,
+            feature_function_for_serving_plus_1,
+        ]
+    )
+
+
+@pytest.fixture(scope="module")
+def ci_for_the_float_feature():
+    return ColumnInfo(
+        info=FeatureColumnInfo(
+            table_name="test.ft2",
+            feature_name="the_float",
+            lookup_key=["user_id"],
+            output_name="the_float",
+        ),
+        include=True,
+    )
+
+
+@pytest.fixture(scope="module")
+def ci_for_age2_source():
+    return ColumnInfo(
+        info=SourceDataColumnInfo(
+            name="age2",
+        ),
+        include=False,
+    )
+
+
+@pytest.fixture(scope="function")
+def odci2_float2str():
+    return ColumnInfo(
+        info=OnDemandColumnInfo(
+            udf_name="cat.sch2.float_to_string",
+            input_bindings={"x": "the_float"},
+            output_name="float_to_string_output",
+        ),
+        include=True,
+    )
+
+
+@pytest.fixture(scope="function")
+def odci_date():
+    return ColumnInfo(
+        info=OnDemandColumnInfo(
+            udf_name="cat.sch.timestamp",
+            input_bindings={},
+            output_name="date_output",
+        ),
+        include=True,
+    )
+
+
+@pytest.fixture(scope="function")
+def odci_age_2x_age2():
+    return ColumnInfo(
+        info=OnDemandColumnInfo(
+            udf_name="cat.sch.times_two",
+            input_bindings={"x": "age2"},
+            output_name="age2_times_2_output",
+        ),
+        include=True,
+    )
+
+
+@pytest.fixture(scope="function")
+def advanced_feature_spec_with_odci(
+    ci_for_feature_age,
+    ci_for_the_float_feature,
+    ci_for_age2_source,
+    odci_age_2x,
+    odci2_float2str,
+    odci_date,
+    odci_age_2x_age2,
+    odci_age_plus_1,
+):
+    return create_test_feature_spec(
+        column_infos=[
+            ci_for_feature_age,
+            ci_for_the_float_feature,
+            ci_for_age2_source,
+            odci_age_2x,
+            odci2_float2str,
+            odci_date,
+            odci_age_2x_age2,
+            odci_age_plus_1,
+        ]
+    )
+
+
+@pytest.fixture(scope="function")
+def advanced_on_demand_setup(
+    feature_spec_load,
+    advanced_feature_spec_with_odci,
+    feature_tables_for_serving_load,
+    feature_tables_for_serving_advanced,
+    is_file,
+):
+    """
+    This fixture can be passed to a test function to patch FeatureSpec.load and
+    FeatureTablesForServing.load to return the basic feature_spec and feature_tables_for_serving
+    fixtures defined above. It may remain unused in a test case.
+    """
+    feature_spec_load.return_value = advanced_feature_spec_with_odci
+    feature_tables_for_serving_load.return_value = feature_tables_for_serving_advanced
+    is_file.side_effect = lambda path: path == os.path.join(
+        MODEL_URI, "_databricks_internal/feature_functions_for_serving.dat"
+    )
+
+
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+def test_predict_with_on_demand_advanced(
+    advanced_on_demand_setup,
+    lookup_client_advanced,
+    feature_functions_for_serving_advanced,
+    feature_functions_for_serving_load,
+):
+    """
+    This advanced test case validates the following:
+    - Feature that is used only as input to Feature Function ("age")
+    - Excluded source data that is only used as an input to FeatureFunctions ("age2")
+    - Feature Function without input ("cat.sch.timestamp")
+    - Feature Function DateType output ("date_output"). This is intended as a safety-check that non-
+      basic output types are handled correctly.
+    - Call the same UDF on two different columns ("age_times_2_output", "age2_times_2_output")
+    - Partially override a Feature Function output ("date_output")
+    - Partially override a Feature Function input ("age")
+    """
+    feature_functions_for_serving_load.return_value = (
+        feature_functions_for_serving_advanced
+    )
+    fs_model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    raw_model = MagicMock()
+    fs_model.raw_model = raw_model
+
+    # Partially override date_output
+    df = pd.DataFrame(
+        {
+            "user_id": [123, 456],
+            "age": [99, np.nan],
+            "age2": [33, 44],
+            "date_output": [np.nan, datetime(year=2020, month=2, day=1)],
+        }
+    )
+    lookup_client1, lookup_client2 = lookup_client_advanced
+    lookup_client1.lookup_features.return_value = pd.DataFrame({"age": [55, 32]})
+    lookup_client2.lookup_features.return_value = pd.DataFrame(
+        {"the_float": [4.2, 2.1]}
+    )
+    prediction = fs_model.predict(df)
+
+    lookup_client1.lookup_features.assert_called_once_with(ANY, ["age"], metrics=ANY)
+    pd.testing.assert_frame_equal(
+        lookup_client1.lookup_features.call_args[0][0],
+        pd.DataFrame({"pk": [123, 456]}),
+    )
+
+    lookup_client2.lookup_features.assert_called_once_with(
+        ANY, ["the_float"], metrics=ANY
+    )
+    pd.testing.assert_frame_equal(
+        lookup_client2.lookup_features.call_args[0][0],
+        pd.DataFrame({"pk": [123, 456]}),
+    )
+
+    expected_model_input_df = pd.DataFrame(
+        {
+            "the_float": [4.2, 2.1],
+            "age_times_2_output": pd.Series([99 * 2, 32 * 2], dtype="int32"),
+            "float_to_string_output": ["4.2", "2.1"],
+            "date_output": [
+                datetime(year=2000, month=1, day=1),
+                datetime(year=2020, month=2, day=1),
+            ],
+            "age2_times_2_output": pd.Series([33 * 2, 44 * 2], dtype="int32"),
+            "age_plus_1_output": pd.Series([99 + 1, 32 + 1], dtype="int32"),
+        }
+    )
+    actual = raw_model.predict.call_args[0][0]
+    pd.testing.assert_frame_equal(actual, expected_model_input_df)
+
+
+##### Feature Function Unit Tests
+# These unit tests mock out unrelated parts of _FeatureStoreModelWrapper and imports
+# TODO(ML-30606): Migrate to separate file
+
+
+@pytest.mark.parametrize("ff_enabled", [True, False])
+@patch.multiple(
+    mlflow_model._FeatureStoreModelWrapper,
+    _load_feature_tables_for_serving=MagicMock(),
+    _create_batch_lookup_client=MagicMock(),
+    _create_lookup_clients=MagicMock(),
+    _has_feature_functions=lambda x, y: True,
+)
+@patch("databricks.feature_store.entities.feature_spec.FeatureSpec.load", MagicMock())
+@patch("databricks.feature_store.mlflow_model.FeatureFunctionExecutor")
+@patch("databricks.feature_store.mlflow_model.FeatureFunctionsForServing")
+def test_feature_functions_initialization(
+    ffs_for_serving_cls, ff_executor_cls, ff_enabled
+):
+    ffs_for_serving_cls.load = MagicMock()
+    ffs_for_serving = MagicMock()
+    ffs_for_serving_cls.load.return_value = ffs_for_serving
+    with patch(
+        "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+        lambda self: ff_enabled,
+    ):
+        model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+        if ff_enabled:
+            expected_path = os.path.join(MODEL_URI, "_databricks_internal/")
+            ffs_for_serving_cls.load.assert_called_once_with(expected_path)
+            ff_executor_cls.assert_called_once_with(
+                ffs_for_serving, model.feature_spec.on_demand_column_infos
+            )
+        else:
+            assert ffs_for_serving_cls.load.call_count == 0
+            assert ff_executor_cls.call_count == 0
+
+
+@pytest.fixture(scope="function")
+def feature_spec_with_odci(ci_for_feature1, feature_table_info1, odci_age_2x):
+    return create_test_feature_spec(
+        column_infos=[
+            odci_age_2x,
+            ColumnInfo(
+                info=FeatureColumnInfo(
+                    table_name="test.ft1",
+                    feature_name="age",
+                    lookup_key=["user_id"],
+                    output_name="age",
+                ),
+                include=True,
+            ),
+            ColumnInfo(
+                SourceDataColumnInfo(name="user_id"),
+                include=True,
+            ),
+        ],
+        table_infos=[feature_table_info1],
+    )
+
+
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._is_lookup_client_feature_function_evaluation_enabled",
+    enable_feature_function_evaluation,
+)
+@patch.multiple(
+    mlflow_model._FeatureStoreModelWrapper,
+    __init__=lambda x, y: None,
+    _validate_input=MagicMock(),
+)
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._augment_with_materialized_features"
+)
+def test_predict_ff_executor_reorders_input(augment_fn, feature_spec_with_odci):
+    model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    model.has_feature_functions = True
+    model.feature_function_executor = MagicMock()
+    model.feature_spec = feature_spec_with_odci
+    raw_model = MagicMock()
+    model.raw_model = raw_model
+
+    raw_df = pd.DataFrame({"user_id": [123]})
+    df_with_materialized_features = pd.DataFrame({"user_id": [123], "age": [55]})
+    df_with_on_demand_features = pd.DataFrame({"age_times_2_output": [3.14]})
+
+    model.feature_function_executor.execute_feature_functions.return_value = (
+        df_with_on_demand_features
+    )
+    augment_fn.return_value = df_with_materialized_features
+
+    model.predict(raw_df)
+
+    # FeatureFunctionExecutor is called with expected args
+    model.feature_function_executor.execute_feature_functions.assert_called_once_with(
+        df_with_materialized_features
+    )
+    # Model.predict is called with expected DataFrame containing *reordered* on-demand features,
+    # materialized features, and source data.
+    expected_model_input_df = pd.DataFrame(
+        {"age_times_2_output": [3.14], "age": [55], "user_id": [123]}
+    )
+    actual = raw_model.predict.call_args[0][0]
+    pd.testing.assert_frame_equal(actual, expected_model_input_df)
+
+
+@pytest.fixture(scope="function")
+def feature_spec_with_excluded_columns(ci_for_feature1, feature_table_info1):
+    included_feat_col_info = ColumnInfo(
+        info=FeatureColumnInfo(
+            table_name="test.ft1",
+            feature_name="age",
+            lookup_key=["user_id"],
+            output_name="included_feature",
+        ),
+        include=True,
+    )
+    excluded_feat_col_info = ColumnInfo(
+        info=FeatureColumnInfo(
+            table_name="test.ft1",
+            feature_name="age",
+            lookup_key=["user_id"],
+            output_name="excluded_feature",
+        ),
+        include=False,
+    )
+    excluded_source_col_info = ColumnInfo(
+        SourceDataColumnInfo(name="user_id"), include=False
+    )
+    return create_test_feature_spec(
+        column_infos=[
+            included_feat_col_info,
+            excluded_feat_col_info,
+            excluded_source_col_info,
+        ]
+    )
+
+
+@patch.multiple(
+    mlflow_model._FeatureStoreModelWrapper,
+    __init__=lambda x, y: None,
+    _validate_input=MagicMock(),
+)
+@patch(
+    "databricks.feature_store.mlflow_model._FeatureStoreModelWrapper._augment_with_materialized_features"
+)
+def test_predict_excludes_columns(augment_fn, feature_spec_with_excluded_columns):
+    model = mlflow_model._FeatureStoreModelWrapper(MODEL_URI)
+    model.has_feature_functions = False
+    model.feature_spec = feature_spec_with_excluded_columns
+    raw_model = MagicMock()
+    model.raw_model = raw_model
+    raw_df = pd.DataFrame({"user_id": [123]})
+    augmented_df = pd.DataFrame(
+        {
+            "user_id": [123],
+            "included_feature": ["I'm included"],
+            "excluded_feature": ["I'm excluded"],
+        }
+    )
+
+    augment_fn.return_value = augmented_df
+    model.predict(raw_df)
+
+    actual = raw_model.predict.call_args[0][0]
+    pd.testing.assert_frame_equal(
+        actual, pd.DataFrame({"included_feature": ["I'm included"]})
+    )
```

### Comparing `databricks-feature-lookup-0.4.1/tests/test_online_lookup_client.py` & `databricks-feature-lookup-0.5.0/tests/test_online_lookup_client.py`

 * *Files identical despite different names*

