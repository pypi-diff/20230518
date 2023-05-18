# Comparing `tmp/ml-management-0.0.31.tar.gz` & `tmp/ml-management-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.31.tar", last modified: Thu May  4 11:23:59 2023, max compression
+gzip compressed data, was "ml-management-0.0.32.tar", last modified: Thu May 18 13:07:10 2023, max compression
```

## Comparing `ml-management-0.0.31.tar` & `ml-management-0.0.32.tar`

### file list

```diff
@@ -1,61 +1,73 @@
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-05-02 14:30:21.000000 ml-management-0.0.31/MANIFEST.in
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/dataset/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      191 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      330 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/dataset/datamodel.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1298 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/dataset.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/dataset/dummy_dataset/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/dataset/dummy_dataset/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      560 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/dummy_dataset/dummy_dataset.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/dataset/s3_dataset/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/dataset/s3_dataset/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10399 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/s3_dataset/s3dataset.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/executor_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/executor_template/default_executors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4592 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      401 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/mlmanagement/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      581 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    11676 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9511 2023-05-04 09:36:23.000000 ml-management-0.0.31/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      163 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5001 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      261 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/models/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/models/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/models/patterns/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4365 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/registry/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/registry/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2566 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/registry/exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/tests/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/tests/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9508 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/tests/test_s3_dataset.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-05-04 11:23:59.537529 ml-management-0.0.31/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-05-02 14:30:21.000000 ml-management-0.0.31/README.md
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-05-04 11:23:57.000000 ml-management-0.0.31/VERSION
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ml_management.egg-info/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1938 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      142 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/requires.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-05-04 11:23:59.537529 ml-management-0.0.31/setup.cfg
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1030 2023-05-04 08:40:01.000000 ml-management-0.0.31/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.197035 ml-management-0.0.32/
+-rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-04-17 13:42:26.000000 ml-management-0.0.32/MANIFEST.in
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.32/ML_management/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      120 2023-05-18 07:29:32.000000 ml-management-0.0.32/ML_management/collectors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1092 2023-05-17 12:25:48.000000 ml-management-0.0.32/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      456 2023-05-18 06:45:39.000000 ml-management-0.0.32/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      509 2023-05-18 07:27:29.000000 ml-management-0.0.32/ML_management/collectors/collectors.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/dummy/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      463 2023-05-17 13:22:23.000000 ml-management-0.0.32/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/s3/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10557 2023-05-17 13:22:23.000000 ml-management-0.0.32/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)   331440 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3167 2023-05-18 08:42:14.000000 ml-management-0.0.32/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/dataset_loader_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2407 2023-05-17 10:16:44.000000 ml-management-0.0.32/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-18 07:11:26.000000 ml-management-0.0.32/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/executor_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4566 2023-05-17 10:16:44.000000 ml-management-0.0.32/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      402 2023-05-18 07:11:58.000000 ml-management-0.0.32/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/mlmanagement/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      581 2023-04-26 06:58:05.000000 ml-management-0.0.32/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-05-11 13:44:22.000000 ml-management-0.0.32/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-05-11 13:44:22.000000 ml-management-0.0.32/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    11676 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10262 2023-05-17 08:18:52.000000 ml-management-0.0.32/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      201 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      316 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/models/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.32/ML_management/models/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/models/patterns/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4202 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/registry/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.32/ML_management/registry/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/registry/exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-05-15 06:26:40.000000 ml-management-0.0.32/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/tests/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.32/ML_management/tests/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-04-17 13:42:26.000000 ml-management-0.0.32/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9298 2023-05-16 14:18:14.000000 ml-management-0.0.32/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/uploader_data/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1582 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-18 13:07:10.197035 ml-management-0.0.32/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)       56 2022-11-02 13:55:55.000000 ml-management-0.0.32/README.md
+-rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-05-18 13:07:02.000000 ml-management-0.0.32/VERSION
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.197035 ml-management-0.0.32/ml_management.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2449 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)      142 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-18 13:07:10.197035 ml-management-0.0.32/setup.cfg
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1030 2023-05-15 06:26:38.000000 ml-management-0.0.32/setup.py
```

### Comparing `ml-management-0.0.31/ML_management/dataset/dataset.py` & `ml-management-0.0.32/ML_management/collectors/collector_pattern.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-"""Abstract class of Dataset for Job."""
+"""Abstract class of Collector for Job."""
 from abc import ABC, abstractmethod
 
 # That's copied from server, excluding splitters
 
 
-class Dataset(ABC):
-    """Abstract class of Dataset for Job."""
+class CollectorPattern(ABC):
+    """Abstract class of Collector for Job."""
 
     @abstractmethod
     def set_data(self, *args, **kwargs):
         """Set suitable data."""
         raise NotImplementedError
 
+    @staticmethod
     @abstractmethod
-    def get_json_schema(self):
+    def get_json_schema():
         """
         Every dataset should define json schema for its set_data parameters.
 
         https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.1.1
 
         The value of keyword "type" MUST be either a string or an array.
         If it is an array, elements of the array MUST be strings and MUST be unique.
 
         String values MUST be one of the six primitive types ("null", "boolean", "object", "array", "number", or "string"),
         or "integer" which matches any number with a zero fractional part.
 
         Parameters are optional by default. Requiered parameters are specified as array by key "required".
         """
         raise NotImplementedError
-
-    @staticmethod
-    @abstractmethod
-    def get_data_flavour():
-        """Get data flavour for this Dataset."""
-        # better leave it staticmethod for now, not to instatiate Datasets in Job.
-        raise NotImplementedError
```

### Comparing `ml-management-0.0.31/ML_management/dataset/s3_dataset/s3dataset.py` & `ml-management-0.0.32/ML_management/collectors/s3/s3collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""S3 Dataset for downloading files and folders."""
+"""S3 Collector for downloading files and folders."""
 import os
 import posixpath
 from typing import List, Optional, Union
 
 from boto3 import client
 from botocore.exceptions import ClientError
-from ML_management.dataset.datamodel import DatasetFlavour
-from ML_management.dataset.dataset import Dataset
+from ML_management.collectors.collector_pattern import CollectorPattern
 
 
 class S3FolderNotFound(Exception):
     """Define Version Not Found Exception."""
 
     def __init__(self, path: str, bucket: str):
         self.path = path
@@ -46,23 +45,24 @@
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (S3ObjectNotFound, (self.path, self.bucket))
 
 
-class S3Dataset(Dataset):
-    """Dataloader for S3 paths using boto3 library."""
+class S3Collector(CollectorPattern):
+    """Collector for S3 paths using boto3 library."""
 
     def __init__(self) -> None:
         self.default_url = os.environ.get("MLFLOW_S3_ENDPOINT_URL", "http://localhost:9000")
         self.default_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID", "minioadmin")
         self.default_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY", "minioadmin")
 
-    def get_json_schema(self):
+    @staticmethod
+    def get_json_schema():
         """Return json schema."""
         return {
             "type": "object",
             "properties": {
                 "local_path": {"type": "string"},
                 "bucket": {"type": "string"},
                 "remote_paths": {"type": "array", "items": {"type": "string"}},
@@ -77,15 +77,16 @@
                     ]
                 },
                 "endpoint_url": {"type": "string"},
                 "aws_access_key_id": {"type": "string"},
                 "aws_secret_access_key": {"type": "string"},
                 "aws_session_token": {"type": "string"},
             },
-            "required": ["remote_paths"],
+            "required": ["bucket"],
+            "additionalProperties": False,
         }
 
     def _download_file(self, bucket: str, service_client, remote_file_path: str, local_path: str):
         dirpath = posixpath.dirname(remote_file_path)
         local_dir_path = os.path.join(local_path, dirpath)
         local_file_path = os.path.join(local_path, remote_file_path)
         if not os.path.exists(local_dir_path):
@@ -133,16 +134,16 @@
             else:
                 raise err
 
     def set_data(
         self,
         *,
         local_path: str = "/s3_data/",
-        bucket: str = "mlflow-artifacts",  # TODO do we pass bucket or not? is it always possible to parse?
-        remote_paths: List[str],
+        bucket: str,  # TODO do we pass bucket or not? is it always possible to parse?
+        remote_paths: Optional[List[str]] = None,
         service_name: str = "s3",
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
         verify: Optional[Union[bool, str]] = None,
         endpoint_url: Optional[str] = None,
         aws_access_key_id: Optional[str] = None,
@@ -223,21 +224,20 @@
             use_ssl=use_ssl,
             verify=verify,
             endpoint_url=endpoint_url if endpoint_url else self.default_url,
             aws_access_key_id=aws_access_key_id if aws_access_key_id else self.default_access_key_id,
             aws_secret_access_key=aws_secret_access_key if aws_secret_access_key else self.default_secret_access_key,
             aws_session_token=aws_session_token,
         )
-        for path in remote_paths:
-            if path.endswith("/"):
-                # it is a folder
-                # list all files in a folder in one go and download them all!
-                self._download_folder(bucket, service_client, path, local_path)
-            else:
-                # it is a file
-                self._download_file(bucket, service_client, path, local_path)
+        if remote_paths is not None:
+            for path in remote_paths:
+                if path.endswith("/"):
+                    # it is a folder
+                    # list all files in a folder in one go and download them all!
+                    self._download_folder(bucket, service_client, path, local_path)
+                else:
+                    # it is a file
+                    self._download_file(bucket, service_client, path, local_path)
+        else:
+            for key in service_client.list_objects(Bucket=bucket)["Contents"]:
+                self._download_file(bucket, service_client, key["Key"], local_path)
         return local_path
-
-    @staticmethod
-    def get_data_flavour():
-        """Return flavour."""
-        return DatasetFlavour.S3
```

### Comparing `ml-management-0.0.31/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.32/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.32/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.32/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.32/ML_management/executor_template/executor_pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,20 @@
         """
         self.executor_name = executor_name
         self.desired_model_methods = desired_model_methods
         self.executor_upload_model_mode = executor_upload_model_mode
 
         # That parameters will be set automatically in job before the 'execute' func would be executed.
         self.model = None
-        self.data_path = None
+        self.dataset = None
         self.model_methods_parameters: dict = {}
         self.model_methods_schema: dict = {}
         """
         :param self.model: python model class
-        :param self.data_path: the path or object for dataset
+        :param self.dataset: object for dataset
         :param self.model_methods_parameters: the dict of parameters for each desired_model_methods.
             One could use it in execute() function like that:
                 def execute(self):
                     self.model.train_function(**self.model_methods_parameters[ModelMethodName.train_function])
             In that case method 'execute' calls train_function method of the model with corresponding parameters for that method
             See examples in default_executors folder.
         :param model_methods_schema: the dict of schema parameters for each desired_model_methods.
@@ -44,15 +44,15 @@
     @abstractmethod
     def execute(self, **executor_params):
         """
         Do execution step.
 
         Parameter self.model with the desired model will be set automatically in the job before 'execute' execution.
         To get data_path use self.data_path parameter, which also will be set in the job.
-        'executor_methods_params' are executor parameters. One have to define it yourself as ordinary kwargs with type annotation.
+        'executor_methods_params' are executor parameters. One has to define it as ordinary kwargs with type annotation.
         Also, you could use self.model_methods_parameters for call desired model method with right params.
         return param: artifacts: A dictionary containing ``<name, artifact_uri>`` entries.
                       For example, consider the following ``artifacts`` dictionary::
 
                         {
                             "my_file": "s3://my-bucket/path/to/my/file",
                             "my_file2": "/home/username/path/to/my/file"
```

### Comparing `ml-management-0.0.31/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.32/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.32/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.32/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.32/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.32/ML_management/mlmanagement/mlmanager.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 
 import cloudpickle
 import requests
 from ML_management.mlmanagement import utils
 from ML_management.mlmanagement.jsonschema_inference import infer_jsonschema
 from ML_management.mlmanagement.model_type import ModelType
 from ML_management.mlmanagement.server_mlmanager_exceptions import InvalidExperimentName, ModelTypeIsNotFound
-from ML_management.mlmanagement.utils import EXPERIMENT_NAME_FOR_EXECUTOR, active_run_stack, is_server, server_ml_api
+from ML_management.mlmanagement.utils import (
+    EXPERIMENT_NAME_FOR_DATASET_LOADER,
+    EXPERIMENT_NAME_FOR_EXECUTOR,
+    active_run_stack,
+    is_server,
+    server_ml_api,
+)
 from mlflow.exceptions import MlflowException, RestException
 from requests_toolbelt import MultipartEncoder
 
 import mlflow
 
 
 def create_kwargs(frame, is_it_class_function=False):
@@ -62,39 +68,45 @@
     kwargs_for_save_model = kwargs.copy()
     for delete_arg in delete_args_for_save_model_func:
         del kwargs_for_save_model[delete_arg]
 
     python_model = kwargs_for_save_model["python_model"]
 
     # import some modules here because of circular import
+    from ML_management.dataset_loader_template.dataset_loader_pattern import DatasetLoaderPattern
+    from ML_management.dataset_loader_template.dataset_loader_pattern_to_methods_map import dataset_loader_pattern_to_methods
     from ML_management.executor_template.executor_pattern import JobExecutorPattern
     from ML_management.executor_template.executor_pattern_to_methods_map import executor_pattern_to_methods
     from ML_management.models.model_type_to_methods_map import model_pattern_to_methods
     from ML_management.models.patterns.model_pattern import Model
 
     with TemporaryDirectory() as temp_dir:
         model_folder = "model"
         path_for_model_folder = os.path.join(temp_dir, model_folder)
         zip_file_folder = "zip_file"
         path_for_zip_file = os.path.join(temp_dir, zip_file_folder)
         if python_model is not None:
             if isinstance(python_model, Model):
                 kwargs["model_type"] = ModelType.MODEL
                 model_to_methods = model_pattern_to_methods
-                if utils.active_experiment_name == EXPERIMENT_NAME_FOR_EXECUTOR:
-                    raise InvalidExperimentName(ModelType.MODEL.value, EXPERIMENT_NAME_FOR_EXECUTOR)
+                if utils.active_experiment_name in [EXPERIMENT_NAME_FOR_EXECUTOR, EXPERIMENT_NAME_FOR_DATASET_LOADER]:
+                    raise InvalidExperimentName(ModelType.MODEL.value, utils.active_experiment_name)
             elif isinstance(python_model, JobExecutorPattern):
                 kwargs["model_type"] = ModelType.EXECUTOR
                 model_to_methods = executor_pattern_to_methods
                 if utils.active_experiment_name != EXPERIMENT_NAME_FOR_EXECUTOR:
                     raise InvalidExperimentName(ModelType.EXECUTOR.value, utils.active_experiment_name)
                 # collect all needed model's methods
                 kwargs["model_method_names"] = python_model.desired_model_methods
                 kwargs["executor_upload_model_mode"] = python_model.executor_upload_model_mode
-
+            elif isinstance(python_model, DatasetLoaderPattern):
+                kwargs["model_type"] = ModelType.DATASET_LOADER
+                model_to_methods = dataset_loader_pattern_to_methods
+                if utils.active_experiment_name != EXPERIMENT_NAME_FOR_DATASET_LOADER:
+                    raise InvalidExperimentName(kwargs["model_type"].value, utils.active_experiment_name)
             else:
                 raise ModelTypeIsNotFound()
 
             # now we need to infer schemas for methods.
             methods_schema = {}
             for (model_type, methods_name_to_schema_map) in model_to_methods.items():
                 if isinstance(python_model, model_type):
@@ -110,16 +122,16 @@
                 del kwargs[delete_arg]
             kwargs["loader_module"] = mlflow.pyfunc.model.__name__
             model_filename = shutil.make_archive(path_for_zip_file, "zip", path_for_model_folder)
 
         elif kwargs["loader_module"] is not None:
             # now one could log only ModelType.MODEL type by 'loader_module' parameter.
             kwargs["model_type"] = ModelType.MODEL
-            if utils.active_experiment_name == EXPERIMENT_NAME_FOR_EXECUTOR:
-                raise InvalidExperimentName(ModelType.MODEL.value, EXPERIMENT_NAME_FOR_EXECUTOR)
+            if utils.active_experiment_name in [EXPERIMENT_NAME_FOR_EXECUTOR, EXPERIMENT_NAME_FOR_DATASET_LOADER]:
+                raise InvalidExperimentName(ModelType.MODEL.value, utils.active_experiment_name)
             # 'model_methods_schema' not defined
             kwargs["model_methods_schema"] = json.dumps({})
 
             if not os.path.isdir(kwargs["data_path"]):
                 raise Exception("Directory {0} doesn't exist".format(kwargs["data_path"]))
             model_filename = shutil.make_archive(path_for_zip_file, "zip", kwargs["data_path"])
         else:
```

### Comparing `ml-management-0.0.31/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.32/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.32/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.32/ML_management/models/patterns/model_pattern.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import mlflow
 
 
 class Model(mlflow.pyfunc.PythonModel, ABC):
     """Abstract class for model that Job will use."""
 
     def __init__(self):
-        """Initialize data path."""
-        self.data_path = None
+        """Initialize dataset."""
+        self.dataset = None
 
     @abstractmethod
     def predict_function(self, **kwargs):
         """Every model should make predictions."""
         raise NotImplementedError
 
     def upload_model(
@@ -80,12 +80,7 @@
                     extra_pip_requirements=extra_pip_requirements,
                     conda_env=conda_env,
                 )
         except Exception as err:
             raise err
         finally:
             utils.active_experiment_name = old_experiment_name
-
-    @abstractmethod
-    def get_data_flavour(self):
-        """Every model is required to store one of the data flavour."""
-        raise NotImplementedError
```

### Comparing `ml-management-0.0.31/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.32/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/registry/exceptions.py` & `ml-management-0.0.32/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/registry/registry_manager.py` & `ml-management-0.0.32/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.32/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.31/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.32/ML_management/tests/test_s3_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import shutil
 import unittest
 from unittest.mock import Mock, patch
 
 import boto3
-import ML_management.dataset.s3_dataset.s3dataset
+import ML_management.collectors.s3.s3collector
 from botocore.exceptions import ClientError
-from ML_management.dataset.s3_dataset.s3dataset import S3BucketNotFound, S3FolderNotFound, S3ObjectNotFound
+from ML_management.collectors import COLLECTORS
+from ML_management.collectors.s3.s3collector import S3BucketNotFound, S3FolderNotFound, S3ObjectNotFound
 
 
 def mock_client_download_successful(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     def mock_download_file(Bucket, Key, Filename, ExtraArgs=None, Callback=None, Config=None):
         files_content_map = {
@@ -111,20 +112,20 @@
     test-data:
         sample_data/1.txt ("one\n"),
         sample_data/2.txt ("two\n"),
         sample_data/sample_folder/3.txt ("three\n")
     """
 
     @patch(
-        "ML_management.dataset.s3_dataset.s3dataset.client",
+        "ML_management.collectors.s3.s3collector.client",
         new=mock_client_download_successful,
     )
     def test_download_files(self):
-        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
-        assert mock_client_download_successful is ML_management.dataset.s3_dataset.s3dataset.client
+        s3_dataset = COLLECTORS["s3"]()
+        assert mock_client_download_successful is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
         local_path = s3_dataset.set_data(
             local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
             bucket="test-data",
             remote_paths=[
                 "sample_data/1.txt",
@@ -145,20 +146,20 @@
         with open(os.path.join(local_path, "sample_data/sample_folder/3.txt"), "r") as f:
             text_one = f.read()
             self.assertEqual(text_one, "three\n")
 
         shutil.rmtree(os.path.join(local_path, "sample_data/"))
 
     @patch(
-        "ML_management.dataset.s3_dataset.s3dataset.client",
+        "ML_management.collectors.s3.s3collector.client",
         new=mock_client_download_folder_successful,
     )
     def test_download_folder(self):
-        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
-        assert mock_client_download_folder_successful is ML_management.dataset.s3_dataset.s3dataset.client
+        s3_dataset = COLLECTORS["s3"]()
+        assert mock_client_download_folder_successful is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
         local_path = s3_dataset.set_data(
             local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
             bucket="test-data",
             remote_paths=["sample_data/"],
             endpoint_url=endpoint_url,
@@ -175,77 +176,77 @@
         with open(os.path.join(local_path, "sample_data/sample_folder/3.txt"), "r") as f:
             text_one = f.read()
             self.assertEqual(text_one, "three\n")
 
         shutil.rmtree(os.path.join(local_path, "sample_data/"))
 
     @patch(
-        "ML_management.dataset.s3_dataset.s3dataset.client",
+        "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_object,
     )
     def test_download_bad_object(self):
-        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
-        assert mock_client_bad_object is ML_management.dataset.s3_dataset.s3dataset.client
+        s3_dataset = COLLECTORS["s3"]()
+        assert mock_client_bad_object is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3ObjectNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="test-data",
                 remote_paths=["sample_data/nosuchfile.txt"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
             )
 
     @patch(
-        "ML_management.dataset.s3_dataset.s3dataset.client",
+        "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_folder,
     )
     def test_download_bad_folder(self):
-        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
-        assert mock_client_bad_folder is ML_management.dataset.s3_dataset.s3dataset.client
+        s3_dataset = COLLECTORS["s3"]()
+        assert mock_client_bad_folder is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3FolderNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="test-data",
                 remote_paths=["sample_data/nosuchfolder/"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
             )
 
     @patch(
-        "ML_management.dataset.s3_dataset.s3dataset.client",
+        "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_bucket_folder,
     )
     def test_download_bad_bucket_folder(self):
-        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
-        assert mock_client_bad_bucket_folder is ML_management.dataset.s3_dataset.s3dataset.client
+        s3_dataset = COLLECTORS["s3"]()
+        assert mock_client_bad_bucket_folder is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3BucketNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="nosuchbucket",
                 remote_paths=["sample_data/"],
                 endpoint_url=endpoint_url,
                 aws_access_key_id="some_mock_key",
                 aws_secret_access_key="some_mock_key",
             )
 
     @patch(
-        "ML_management.dataset.s3_dataset.s3dataset.client",
+        "ML_management.collectors.s3.s3collector.client",
         new=mock_client_bad_bucket_object,
     )
     def test_download_bad_bucket_object(self):
-        s3_dataset = ML_management.dataset.s3_dataset.s3dataset.S3Dataset()
-        assert mock_client_bad_bucket_object is ML_management.dataset.s3_dataset.s3dataset.client
+        s3_dataset = COLLECTORS["s3"]()
+        assert mock_client_bad_bucket_object is ML_management.collectors.s3.s3collector.client
         endpoint_url = "some_mock_url"
 
         with self.assertRaises(S3BucketNotFound):
             s3_dataset.set_data(
                 local_path=os.path.join(os.path.dirname(__file__), "downloaded_data/"),
                 bucket="nosuchbucket",
                 remote_paths=["sample_data/1.txt"],
```

### Comparing `ml-management-0.0.31/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.32/ml_management.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 MANIFEST.in
 README.md
 VERSION
 setup.py
 ML_management/__init__.py
-ML_management/dataset/__init__.py
-ML_management/dataset/datamodel.py
-ML_management/dataset/dataset.py
-ML_management/dataset/dummy_dataset/__init__.py
-ML_management/dataset/dummy_dataset/dummy_dataset.py
-ML_management/dataset/s3_dataset/__init__.py
-ML_management/dataset/s3_dataset/s3dataset.py
+ML_management/collectors/__init__.py
+ML_management/collectors/collector_pattern.py
+ML_management/collectors/collector_pattern_to_methods_map.py
+ML_management/collectors/collectors.py
+ML_management/collectors/dummy/__init__.py
+ML_management/collectors/dummy/dummy_collector.py
+ML_management/collectors/s3/__init__.py
+ML_management/collectors/s3/s3collector.py
+ML_management/collectors/topic_markers/__init__.py
+ML_management/collectors/topic_markers/api_schema.py
+ML_management/collectors/topic_markers/topic_markers_collector.py
+ML_management/dataset_loader_template/__init__.py
+ML_management/dataset_loader_template/dataset_loader_pattern.py
+ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
 ML_management/executor_template/__init__.py
 ML_management/executor_template/executor_pattern.py
 ML_management/executor_template/executor_pattern_to_methods_map.py
 ML_management/executor_template/upload_model_mode.py
 ML_management/executor_template/default_executors/__init__.py
 ML_management/executor_template/default_executors/finetune_executor.py
 ML_management/executor_template/default_executors/test_executor.py
@@ -35,12 +42,14 @@
 ML_management/models/patterns/trainable_model.py
 ML_management/registry/__init__.py
 ML_management/registry/exceptions.py
 ML_management/registry/registry_manager.py
 ML_management/tests/__init__.py
 ML_management/tests/test_jsonschema_inference.py
 ML_management/tests/test_s3_dataset.py
+ML_management/uploader_data/__init__.py
+ML_management/uploader_data/s3_uploader.py
 ml_management.egg-info/PKG-INFO
 ml_management.egg-info/SOURCES.txt
 ml_management.egg-info/dependency_links.txt
 ml_management.egg-info/requires.txt
 ml_management.egg-info/top_level.txt
```

### Comparing `ml-management-0.0.31/setup.py` & `ml-management-0.0.32/setup.py`

 * *Files identical despite different names*

