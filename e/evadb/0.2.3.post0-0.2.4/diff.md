# Comparing `tmp/evadb-0.2.3.post0.tar.gz` & `tmp/evadb-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.2.3.post0.tar", last modified: Sat May 13 22:06:47 2023, max compression
+gzip compressed data, was "evadb-0.2.4.tar", last modified: Thu May 18 03:49:40 2023, max compression
```

## Comparing `evadb-0.2.3.post0.tar` & `evadb-0.2.4.tar`

### file list

```diff
@@ -1,461 +1,467 @@
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/LICENSE.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16204 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/PKG-INFO
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13569 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/README.md
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.559629 evadb-0.2.3.post0/eva/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.559629 evadb-0.2.3.post0/eva/binder/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/binder/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/binder/binder_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12812 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/binder/statement_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8000 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/binder/statement_binder_context.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.559629 evadb-0.2.3.post0/eva/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    18073 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/catalog/catalog_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3076 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/catalog/catalog_type.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6946 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/catalog/catalog_utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.563629 evadb-0.2.3.post0/eva/catalog/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-05-07 23:58:31.000000 evadb-0.2.3.post0/eva/catalog/models/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/association_models.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/catalog/models/base_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/column_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3274 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/index_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/table_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_io_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/schema_utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.563629 evadb-0.2.3.post0/eva/catalog/services/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/catalog/services/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/base_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/column_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2887 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/index_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/table_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3119 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/catalog/sql_config.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.563629 evadb-0.2.3.post0/eva/configuration/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/configuration/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4200 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/configuration/bootstrap_environment.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4146 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/configuration/configuration_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/configuration/constants.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      882 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/constants.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      787 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/eva.yml
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1553 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/eva_cmd_client.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2399 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/eva_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/abstract_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2214 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/executor/apply_and_merge_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1530 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/create_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5728 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/executor/create_index_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/create_mat_view_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7642 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/create_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/delete_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2557 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/drop_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/drop_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3013 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/execution_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3091 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/executor/executor_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1523 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/explain_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3507 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/faiss_index_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/function_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/groupby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/hash_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/insert_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/join_build_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/lateral_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/limit_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/load_csv_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6065 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/eva/executor/load_multimedia_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/nested_loop_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/orderby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8071 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/plan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/pp_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/predicate_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/project_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/rename_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/sample_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/seq_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/show_info_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/storage_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/executor/union_executor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3521 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/executor/exchange_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/executor/ray_stage.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/optimizer/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/rules.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.567629 evadb-0.2.3.post0/eva/experimental/ray/planner/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/experimental/ray/planner/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/experimental/ray/planner/exchange_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/expression/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/expression/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5469 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/expression/abstract_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/expression/aggregation_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/expression/arithmetic_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/expression/comparison_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/constant_value_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10440 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/expression/expression_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10171 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/function_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/logical_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/expression/tuple_value_expression.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/catalog/frame_info.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/catalog/properties.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1961 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/models/server/response.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/models/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/models/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14837 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/models/storage/batch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3260 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/cost_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/group.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/group_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/memo.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    35842 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/operators.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3838 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_task_stack.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12579 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_tasks.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10874 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/optimizer/optimizer_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5897 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/optimizer/plan_generator.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/optimizer/property.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.571629 evadb-0.2.3.post0/eva/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1016 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/optimizer/rules/pattern.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    43623 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/rules/rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7221 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/rules/rules_base.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7743 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/rules/rules_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13132 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/optimizer/statement_to_opr_convertor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.575630 evadb-0.2.3.post0/eva/parser/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/alias.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2672 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_index_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_mat_view_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/create_udf_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/delete_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/drop_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/drop_udf_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19477 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/eva.lark
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.575630 evadb-0.2.3.post0/eva/parser/evaql/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    65109 2022-12-14 06:32:03.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_lexer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)   408798 2022-12-14 06:32:04.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    44890 2022-12-14 06:32:04.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_parserListener.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    26541 2022-12-14 06:32:04.000000 evadb-0.2.3.post0/eva/parser/evaql/evaql_parserVisitor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/explain_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/insert_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_parser.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.579630 evadb-0.2.3.post0/eva/parser/lark_visitor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2161 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10502 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_expressions.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6231 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_functions.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2143 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1112 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/load_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/rename_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/select_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/show_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/parser/statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/parser/table_ref.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1679 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/parser/types.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/plan_nodes/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/abstract_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2401 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_index_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/create_udf_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/delete_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/drop_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/drop_udf_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/explain_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2355 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/faiss_index_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/function_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/groupby_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/insert_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/limit_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/load_data_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/orderby_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/pp_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/predicate_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/project_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/rename_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/sample_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/show_info_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/storage_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/plan_nodes/union_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/readers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/readers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/readers/abstract_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2651 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/readers/csv_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5986 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/readers/decord_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/readers/image/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/readers/image/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1067 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/readers/image/opencv_image_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/eva/server/command_handler.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/server/db_api.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3276 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/server/interpreter.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2866 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/server/server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6132 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/eva/storage/abstract_media_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2385 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/storage/abstract_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/storage/image_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8881 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/storage/sqlite_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/storage/storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2496 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/storage/video_storage_engine.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/third_party/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/third_party/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.583630 evadb-0.2.3.post0/eva/third_party/huggingface/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-05-13 20:09:04.000000 evadb-0.2.3.post0/eva/third_party/huggingface/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/third_party/huggingface/binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6403 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/third_party/huggingface/create.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2615 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/third_party/huggingface/model.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/abstract/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/udfs/abstract/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/abstract/abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3945 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/asl_action_recognition.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3218 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/chatgpt.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/decorators/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2185 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/decorators.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2754 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3375 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1437 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/udfs/decorators/utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/emotion_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/face_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5998 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/feature_extractor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/gpu_compatible.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/udfs/ndarray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/udfs/ndarray/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/udfs/ndarray/crop.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/udfs/ndarray/similarity.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-05-03 20:30:47.000000 evadb-0.2.3.post0/eva/udfs/ocr_extractor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7165 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/eva/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3858 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/udfs/yolo_object_detector.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/eva/utils/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/eva/utils/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/errors.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6969 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/eva/utils/generic_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1956 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/eva/utils/kv_cache.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/logging_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/s3_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/eva/utils/stats.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      717 2023-05-13 22:04:38.000000 evadb-0.2.3.post0/eva/version.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.587630 evadb-0.2.3.post0/evadb.egg-info/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16204 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/PKG-INFO
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13509 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/entry_points.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1121 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/requires.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-05-13 22:06:47.000000 evadb-0.2.3.post0/evadb.egg-info/top_level.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/pyproject.toml
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/setup.cfg
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4049 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/setup.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/benchmark_tests/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/benchmark_tests/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1176 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/benchmark_tests/conftest.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6639 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/binder/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/binder/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/binder/test_binder_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14016 2023-05-04 00:59:50.000000 evadb-0.2.3.post0/test/binder/test_statement_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7961 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/binder/test_statement_binder_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1796 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/binder/test_statement_binder_python37.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/catalog/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/models/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/models/test_models.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.591630 evadb-0.2.3.post0/test/catalog/services/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/services/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_column_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4745 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/catalog/services/test_index_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_table_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_udf_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_udf_cost_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/services/test_udf_io_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6808 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/catalog/test_catalog_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/catalog/test_column_type.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/catalog/test_sqlalchemy.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.595630 evadb-0.2.3.post0/test/configuration/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/configuration/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/configuration/test_bootstrap_environment.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/configuration/test_configuration_manager.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.595630 evadb-0.2.3.post0/test/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_abstract_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_create_mat_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3987 2023-05-03 23:43:07.000000 evadb-0.2.3.post0/test/executor/test_create_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_execution_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/test_executor_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_limit_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_orderby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10986 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_plan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/test_pp_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_sample_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/executor/utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/expression/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/expression/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_abstract_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_aggregation.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_arithmetic.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_comparison.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/expression/test_expression_tree.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/expression/test_expression_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/expression/test_function_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/expression/test_logical.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/integration_tests/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/integration_tests/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3585 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4522 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_chatgpt.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7645 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5158 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2358 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4086 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13961 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3806 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2983 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_like.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    20623 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5227 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2658 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10182 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10755 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_pytorch.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9958 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/integration_tests/test_reuse.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    30781 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_select_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3277 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12287 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/integration_tests/test_similarity.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/integration_tests/test_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1573 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/markers.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/models/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.599630 evadb-0.2.3.post0/test/models/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/models/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/models/storage/test_batch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11829 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/test/optimizer/rules/test_rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_cost_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_group.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_memo.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13335 2023-05-13 21:57:00.000000 evadb-0.2.3.post0/test/optimizer/test_statement_to_opr_convertor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/parser/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/parser/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36047 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/parser/test_parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7781 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/parser/test_parser_statements.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/plan_nodes/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/plan_nodes/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/readers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/readers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/readers/test_csv_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8104 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/readers/test_decord_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_command_handler.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_db_api.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_interpreter.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/server/test_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4113 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/storage/test_video_storage.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1801 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/test_eva_cmd_client.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/test_eva_imports.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1810 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/test_eva_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/udfs/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.603631 evadb-0.2.3.post0/test/udfs/decorators/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7430 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2134 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/test/udfs/ndarray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/ndarray/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/udfs/ndarray/test_open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4412 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/test/udfs/test_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/test_emotion_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/udfs/test_facenet_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2768 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17437 2023-05-13 22:04:13.000000 evadb-0.2.3.post0/test/util.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/test/utils/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/test/utils/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-05-13 21:27:51.000000 evadb-0.2.3.post0/test/utils/test_generic_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-04-29 19:10:28.000000 evadb-0.2.3.post0/test/utils/test_timer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2199 2023-05-13 21:57:10.000000 evadb-0.2.3.post0/test/utils/test_xdist.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-13 22:06:47.607631 evadb-0.2.3.post0/third_party/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.3.post0/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.467877 evadb-0.2.4/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-05-18 00:46:12.000000 evadb-0.2.4/LICENSE.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16362 2023-05-18 03:49:40.467877 evadb-0.2.4/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13729 2023-05-18 02:58:13.000000 evadb-0.2.4/README.md
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7778 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12413 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7997 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/statement_binder_context.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    18120 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3022 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/catalog_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7200 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/catalog_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/association_models.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4671 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/base_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5266 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/column_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3393 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/index_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/table_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/schema_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/base_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2899 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3119 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/sql_config.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.427875 evadb-0.2.4/eva/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4298 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4146 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/configuration_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1403 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      882 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      787 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/eva.yml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1997 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2692 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2140 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/apply_and_merge_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1530 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5191 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_mat_view_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7642 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2557 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/drop_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3017 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3958 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1522 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/function_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/groupby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/hash_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/join_build_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/lateral_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/load_csv_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6038 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/load_multimedia_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/nested_loop_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8075 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/predicate_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/project_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/storage_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/union_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3916 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/vector_index_scan_executor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3522 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/executor/exchange_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/executor/ray_stage.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/optimizer/rules/rules.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/planner/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/planner/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/planner/exchange_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5559 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/aggregation_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/arithmetic_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/comparison_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/constant_value_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10433 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10172 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/logical_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/tuple_value_expression.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/catalog/frame_info.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/catalog/properties.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1961 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/server/response.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14841 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/storage/batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.435876 evadb-0.2.4/eva/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3259 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/group_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    37333 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/operators.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3837 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12582 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_tasks.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10874 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5897 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/plan_generator.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/property.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.435876 evadb-0.2.4/eva/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1019 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/rules/pattern.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    45651 2023-05-18 02:58:13.000000 evadb-0.2.4/eva/optimizer/rules/rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7336 2023-05-18 02:58:13.000000 evadb-0.2.4/eva/optimizer/rules/rules_base.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7842 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/rules/rules_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13590 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/statement_to_opr_converter.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.435876 evadb-0.2.4/eva/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/alias.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2740 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_index_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_mat_view_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/drop_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19597 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/eva.lark
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/insert_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_parser.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.439875 evadb-0.2.4/eva/parser/lark_visitor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2161 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10670 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6231 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_functions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2143 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1112 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/show_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/table_ref.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1738 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/types.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/abstract_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2469 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_index_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/delete_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/drop_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/drop_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/explain_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/groupby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/insert_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/limit_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/load_data_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/orderby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/pp_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/predicate_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/project_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/rename_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/sample_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/show_info_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/storage_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1421 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/union_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2720 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/vector_index_scan_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/abstract_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2648 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5987 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/readers/image/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/image/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1067 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/image/opencv_image_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3252 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2954 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6133 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2383 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/abstract_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/image_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8972 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2496 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/video_storage_engine.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/third_party/huggingface/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      612 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6403 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/create.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2615 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/model.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/third_party/vector_stores/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      607 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3227 2023-05-18 02:58:13.000000 evadb-0.2.4/eva/third_party/vector_stores/faiss.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2960 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/qdrant.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1376 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1594 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/abstract/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2442 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3945 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3914 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/tracker_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/asl_action_recognition.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3219 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/chatgpt.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2188 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2755 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3376 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2067 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/face_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5999 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/feature_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/gpu_compatible.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ocr_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2899 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/sift_feature_extractor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/trackers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      636 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/trackers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2367 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/trackers/nor_fair.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7609 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3859 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/yolo_object_detector.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/eva/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/errors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7254 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1956 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/kv_cache.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/logging_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1388 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/math_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/s3_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/stats.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      711 2023-05-18 03:01:42.000000 evadb-0.2.4/eva/version.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/evadb.egg-info/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16362 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13679 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1240 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/requires.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/top_level.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-05-18 00:46:12.000000 evadb-0.2.4/pyproject.toml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-05-18 03:49:40.467877 evadb-0.2.4/setup.cfg
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4396 2023-05-18 00:46:12.000000 evadb-0.2.4/setup.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/benchmark_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/benchmark_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1176 2023-05-18 00:46:12.000000 evadb-0.2.4/test/benchmark_tests/conftest.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6639 2023-05-18 00:46:12.000000 evadb-0.2.4/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/test_binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13099 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/test_statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7962 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/test_statement_binder_context.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/models/test_models.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4794 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6808 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/test_column_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/test_sqlalchemy.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-05-18 00:46:12.000000 evadb-0.2.4/test/configuration/test_bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-18 00:46:12.000000 evadb-0.2.4/test/configuration/test_configuration_manager.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_create_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3989 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10983 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_aggregation.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_arithmetic.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_comparison.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_expression_tree.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_logical.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/integration_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3585 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4522 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_chatgpt.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6167 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5158 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2358 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4086 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13961 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3806 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2983 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_like.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    20622 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5377 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2658 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10646 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11709 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10469 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_reuse.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    30781 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3277 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14709 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1574 2023-05-18 00:46:12.000000 evadb-0.2.4/test/markers.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/storage/test_batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11993 2023-05-18 02:58:13.000000 evadb-0.2.4/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13564 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_statement_to_opr_converter.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36070 2023-05-18 00:46:12.000000 evadb-0.2.4/test/parser/test_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7783 2023-05-18 00:46:12.000000 evadb-0.2.4/test/parser/test_parser_statements.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-05-18 00:46:12.000000 evadb-0.2.4/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-05-18 00:46:12.000000 evadb-0.2.4/test/readers/test_csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8104 2023-05-18 00:46:12.000000 evadb-0.2.4/test/readers/test_decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4113 2023-05-18 00:46:12.000000 evadb-0.2.4/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-05-18 00:46:12.000000 evadb-0.2.4/test/storage/test_video_storage.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3309 2023-05-18 00:46:12.000000 evadb-0.2.4/test/test_eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-05-18 00:46:12.000000 evadb-0.2.4/test/test_eva_imports.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1825 2023-05-18 00:46:12.000000 evadb-0.2.4/test/test_eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7429 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4412 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2768 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17438 2023-05-18 00:46:12.000000 evadb-0.2.4/test/util.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/test_generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/test_timer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2199 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/test_xdist.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.467877 evadb-0.2.4/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.4/third_party/__init__.py
```

### Comparing `evadb-0.2.3.post0/LICENSE.txt` & `evadb-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/PKG-INFO` & `evadb-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.3.post0
+Version: 0.2.4
 Summary: EVA AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
 Download-URL: https://github.com/georgia-tech-db/eva
 Description: <div >
@@ -27,15 +27,15 @@
                 <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
                 <a href="https://github.com/orgs/georgia-tech-db/projects/3">
                     <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
                 </a>
                 <a href="https://pepy.tech/project/evadb">
                   <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
                 </a>
-                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
+                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
         </div>
         
         <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
         
         EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
         
         ## Quick Links
@@ -63,25 +63,25 @@
         
         ## Demo
         
         Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
         
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
-        
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
          * ð® <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
          * ð® <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
         
         ## Documentation
         
         * [Detailed Documentation](https://evadb.readthedocs.io/)
-          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
+          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/aidb.html">Video Database Systems</a>.
           - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
           - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
         * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
         * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
         * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
         * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
         
@@ -191,15 +191,15 @@
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
         
         ### ð® [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
         
-        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
+        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
         
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
         
         ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.3.post0 Summary: EVA AI-
-Relational Database System Home-page: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group Author-email: arulraj@gatech.edu License:
-Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/eva
-Description:
+Metadata-Version: 2.1 Name: evadb Version: 0.2.4 Summary: EVA AI-Relational
+Database System Home-page: https://github.com/georgia-tech-db/eva Author:
+Georgia Tech Database Group Author-email: arulraj@gatech.edu License: Apache
+License 2.0 Download-URL: https://github.com/georgia-tech-db/eva Description:
 [EVA]
 # EVA AI-Relational Database System
 [Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
 [Downloads] [Python Versions]
 **** EVA is a database system for building simpler and faster AI-powered
 applications. ****
 EVA is designed for supporting database applications that operate on both
@@ -31,26 +30,27 @@
 user-defined functions - Ã°ÂÂÂ¦ Built-in caching to eliminate redundant model
 invocations across queries - Ã¢ÂÂ¨Ã¯Â¸Â First-class support for PyTorch and
 HuggingFace models - Ã°ÂÂÂ Installable via pip and fully implemented in
 Python ## Demo Here are some illustrative EVA-backed applications (all of them
 are Jupyter notebooks that can be opened in Google Colab): * Ã°ÂÂÂ® Using
 ChatGPT_to_ask_questions_based_on_videos * Ã°ÂÂÂ® Analysing_traffic_flow_at
 an_intersection * Ã°ÂÂÂ® Examining_the_emotion_palette_of_actors_in_a_movie *
-Ã°ÂÂÂ® Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image
-Segmentation_using_Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates *
-Ã°ÂÂÂ® Analysing_toxicity_of_social_media_memes ## Documentation * [Detailed
-Documentation](https://evadb.readthedocs.io/) - If you are wondering why you
-might need an AI-relational database system, start with the page on Video
-Database_Systems. - The Getting_Started page shows how you can use EVA for
-different AI pipelines, and how you can easily extend EVA by defining an user-
-defined function that wraps around your custom deep learning model. - The User
-Guides section contains Jupyter Notebooks that demonstrate how to use various
-features of EVA. Each notebook includes a link to Google Colab to run the code.
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
-emotion-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
+Ã°ÂÂÂ® Image_Similarity_Search_on_Reddit_[FAISS_+_Qdrant] * Ã°ÂÂÂ®
+Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image_Segmentation_using
+Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates * Ã°ÂÂÂ® Analysing
+toxicity_of_social_media_memes ## Documentation * [Detailed Documentation]
+(https://evadb.readthedocs.io/) - If you are wondering why you might need an
+AI-relational database system, start with the page on Video_Database_Systems. -
+The Getting_Started page shows how you can use EVA for different AI pipelines,
+and how you can easily extend EVA by defining an user-defined function that
+wraps around your custom deep learning model. - The User_Guides section
+contains Jupyter Notebooks that demonstrate how to use various features of EVA.
+Each notebook includes a link to Google Colab to run the code. * [Tutorials]
+(https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
 shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
 (https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
 github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 ## Quick Start - Install EVA using the pip package manager. EVA supports Python
 versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
 EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
 notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
@@ -101,15 +101,15 @@
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [MNIST Digit
 Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
 mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
 ----------|--------------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ®
 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/
-tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication
+tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification
 Models) | Source Video | Query Result | |---------------|--------------| |
 [Source Video] |[Query Result] | ### Ã°ÂÂÂ® [License Plate Recognition]
 (https://github.com/georgia-tech-db/eva-application-template) (Plate Detection
 + OCR Extraction Models) | Query Result | |--------------| [Query Result] | ###
 Ã°ÂÂÂ® [Meme Toxicity Classification](https://github.com/georgia-tech-db/
 toxicity-classification) (OCR Extraction + Toxicity Classification Models) |
 Query Result | |--------------| [Query Result] | ## Community and Support
```

### Comparing `evadb-0.2.3.post0/README.md` & `evadb-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://github.com/orgs/georgia-tech-db/projects/3">
             <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
         </a>
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
         </a>
-        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
+        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
 </div>
 
 <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
 EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
 
 ## Quick Links
@@ -54,25 +54,25 @@
 
 ## Demo
 
 Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
 
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
-
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
  * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
  * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
 
 ## Documentation
 
 * [Detailed Documentation](https://evadb.readthedocs.io/)
-  - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
+  - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/aidb.html">Video Database Systems</a>.
   - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
   - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
 * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 
@@ -182,15 +182,15 @@
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
 ### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
 
-### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
+### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
 
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
 
 ### 🔮 [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
```

#### html2text {}

```diff
@@ -25,43 +25,44 @@
 support for your custom deep learning models through user-defined functions -
 ð¦ Built-in caching to eliminate redundant model invocations across queries -
 â¨ï¸ First-class support for PyTorch and HuggingFace models - ð
 Installable via pip and fully implemented in Python ## Demo Here are some
 illustrative EVA-backed applications (all of them are Jupyter notebooks that
 can be opened in Google Colab): * ð® Using_ChatGPT_to_ask_questions_based_on
 videos * ð® Analysing_traffic_flow_at_an_intersection * ð® Examining_the
-emotion_palette_of_actors_in_a_movie * ð® Classifying_images_based_on_their
-content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
-plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
-[Detailed Documentation](https://evadb.readthedocs.io/) - If you are wondering
-why you might need an AI-relational database system, start with the page on
-Video_Database_Systems. - The Getting_Started page shows how you can use EVA
-for different AI pipelines, and how you can easily extend EVA by defining an
-user-defined function that wraps around your custom deep learning model. - The
-User_Guides section contains Jupyter Notebooks that demonstrate how to use
-various features of EVA. Each notebook includes a link to Google Colab to run
-the code. * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/
-tutorials/03-emotion-analysis.ipynb) * [Join us on Slack!](https://
-join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) *
-[Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3) *
-[Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
-analysis.ipynb) ## Quick Start - Install EVA using the pip package manager. EVA
-supports Python versions >= 3.7: ```shell pip install evadb ``` - To launch and
-connect to an EVA server in a Jupyter notebook, check out this [illustrative
-emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/
-tutorials/03-emotion-analysis.ipynb): ```shell cursor = connect_to_server() ```
-- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/
-ua_detrac.mp4) for illustration): ```mysql LOAD VIDEO "data/ua_detrac/
-ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You can now run queries over
-the loaded video: ```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ```
-- Search for frames in the video that contain a car: ```mysql SELECT id, data
-FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| - Search for frames in the video that contain a pedestrian and a car:
-```mysql SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
+emotion_palette_of_actors_in_a_movie * ð® Image_Similarity_Search_on_Reddit_
+[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their_content * ð® Image
+Segmentation_using_Hugging_Face * ð® Recognizing_license_plates * ð®
+Analysing_toxicity_of_social_media_memes ## Documentation * [Detailed
+Documentation](https://evadb.readthedocs.io/) - If you are wondering why you
+might need an AI-relational database system, start with the page on Video
+Database_Systems. - The Getting_Started page shows how you can use EVA for
+different AI pipelines, and how you can easily extend EVA by defining an user-
+defined function that wraps around your custom deep learning model. - The User
+Guides section contains Jupyter Notebooks that demonstrate how to use various
+features of EVA. Each notebook includes a link to Google Colab to run the code.
+* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
+(https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
+github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+## Quick Start - Install EVA using the pip package manager. EVA supports Python
+versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
+EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
+notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a
+video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
+for illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
+TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
+```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
+frames in the video that contain a car: ```mysql SELECT id, data FROM
+TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
+Result | |---------------|--------------| |[Source Video] |[Query Result] | -
+Search for frames in the video that contain a pedestrian and a car: ```mysql
+SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
 (data).labels; ``` - Search for frames with more than three cars: ```mysql
 SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') >
 3; ``` - **Use your custom deep learning model in queries** with a user-defined
 function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
 'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
 useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
 id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
@@ -95,34 +96,35 @@
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
 Classification Model) | Source Video | Query Result | |---------------|--------
 ------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
-analysis.html) (Face Detection + Emotion Classfication Models) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-
-application-template) (Plate Detection + OCR Extraction Models) | Query Result
-| |--------------| [Query Result] | ### ð® [Meme Toxicity Classification]
-(https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction +
-Toxicity Classification Models) | Query Result | |--------------| [Query
-Result] | ## Community and Support ð If you have general questions about
-EVA, want to say hello or just follow along, we'd like to invite you to join
-our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-
-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg). [EVA_Slack_Channel] If you run into any
-problems or issues, please create a Github issue and we'll try our best to
-help. Don't see a feature in the list? Search our issue tracker if someone has
-already requested it and add a comment to it explaining your use-case, or open
-a new issue if not. We prioritize our roadmap based on user feedback, so we'd
-love to hear from you. ## Contributing [![PyPI Version](https://img.shields.io/
-pypi/v/evadb.svg)](https://pypi.org/project/evadb) [![CI Status](https://
-circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/
-georgia-tech-db/eva) [![Documentation Status](https://readthedocs.org/projects/
-evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
-index.html) EVA is the beneficiary of many [contributors](https://github.com/
-georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are
-appreciated. To file a bug or to request a feature, please use GitHub_issues.
-Pull_requests are welcome. For more information, see our [contribution guide]
-(https://evadb.readthedocs.io/en/stable/source/contribute/index.html). ##
-License Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
+analysis.html) (Face Detection + Emotion Classification Models) | Source Video
+| Query Result | |---------------|--------------| |[Source Video] |[Query
+Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
+db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
+Result | |--------------| [Query Result] | ### ð® [Meme Toxicity
+Classification](https://github.com/georgia-tech-db/toxicity-classification)
+(OCR Extraction + Toxicity Classification Models) | Query Result | |-----------
+---| [Query Result] | ## Community and Support ð If you have general
+questions about EVA, want to say hello or just follow along, we'd like to
+invite you to join our [Slack Community](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg). [EVA_Slack_Channel] If you
+run into any problems or issues, please create a Github issue and we'll try our
+best to help. Don't see a feature in the list? Search our issue tracker if
+someone has already requested it and add a comment to it explaining your use-
+case, or open a new issue if not. We prioritize our roadmap based on user
+feedback, so we'd love to hear from you. ## Contributing [![PyPI Version]
+(https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [!
+[CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https:/
+/circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
+readthedocs.org/projects/evadb/badge/?version=stable)](https://
+evadb.readthedocs.io/en/stable/index.html) EVA is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EVA are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE).
```

### Comparing `evadb-0.2.3.post0/eva/__init__.py` & `evadb-0.2.4/eva/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/binder/__init__.py` & `evadb-0.2.4/eva/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/binder/statement_binder.py` & `evadb-0.2.4/eva/binder/statement_binder.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,62 +8,48 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import sys
+from functools import singledispatchmethod
 from pathlib import Path
 
 from eva.binder.binder_utils import (
     BinderError,
     bind_table_info,
     check_column_name_is_string,
     check_groupby_pattern,
     check_table_object_is_video,
     extend_star,
+    handle_bind_extract_object_function,
     resolve_alias_table_value_expression,
 )
 from eva.binder.statement_binder_context import StatementBinderContext
 from eva.catalog.catalog_manager import CatalogManager
-from eva.catalog.catalog_type import IndexType, NdArrayType, TableType, VideoColumnName
+from eva.catalog.catalog_type import NdArrayType, TableType, VideoColumnName
 from eva.catalog.catalog_utils import get_metadata_properties
 from eva.configuration.constants import EVA_DEFAULT_DIR
 from eva.expression.abstract_expression import AbstractExpression, ExpressionType
 from eva.expression.function_expression import FunctionExpression
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.create_index_statement import CreateIndexStatement
 from eva.parser.create_mat_view_statement import CreateMaterializedViewStatement
 from eva.parser.delete_statement import DeleteTableStatement
 from eva.parser.explain_statement import ExplainStatement
 from eva.parser.rename_statement import RenameTableStatement
 from eva.parser.select_statement import SelectStatement
 from eva.parser.statement import AbstractStatement
 from eva.parser.table_ref import TableRef
+from eva.parser.types import UDFType
 from eva.third_party.huggingface.binder import assign_hf_udf
 from eva.utils.generic_utils import get_file_checksum, load_udf_class_from_file
 from eva.utils.logging_manager import logger
 
-if sys.version_info >= (3, 8):
-    from functools import singledispatchmethod
-else:
-    # https://stackoverflow.com/questions/24601722/how-can-i-use-functools-singledispatch-with-instance-methods
-    from functools import singledispatch, update_wrapper
-
-    def singledispatchmethod(func):
-        dispatcher = singledispatch(func)
-
-        def wrapper(*args, **kw):
-            return dispatcher.dispatch(args[1].__class__)(*args, **kw)
-
-        wrapper.register = dispatcher.register
-        update_wrapper(wrapper, func)
-        return wrapper
-
 
 class StatementBinder:
     def __init__(self, binder_context: StatementBinderContext):
         self._binder_context = binder_context
         self._catalog = CatalogManager()
 
     @singledispatchmethod
@@ -91,18 +77,14 @@
 
         # TODO: create index currently only supports single numpy column.
         assert len(node.col_list) == 1, "Index cannot be created on more than 1 column"
 
         # TODO: create index currently only works on TableInfo, but will extend later.
         assert node.table_ref.is_table_atom(), "Index can only be created on Tableinfo"
 
-        assert IndexType.is_faiss_index_type(
-            node.index_type
-        ), "Index type {} is not supported.".format(node.index_type)
-
         if not node.udf_func:
             # Feature table type needs to be float32 numpy array.
             col_def = node.col_list[0]
             table_ref_obj = node.table_ref.table.table_obj
             col = [col for col in table_ref_obj.columns if col.name == col_def.name][0]
             assert (
                 col.array_type == NdArrayType.FLOAT32
@@ -230,14 +212,18 @@
         if node.col_name == VideoColumnName.data:
             self._binder_context.enable_video_retrieval()
         node.col_alias = "{}.{}".format(table_alias, node.col_name.lower())
         node.col_object = col_obj
 
     @bind.register(FunctionExpression)
     def _bind_func_expr(self, node: FunctionExpression):
+        # handle the special case of "extract_object"
+        if node.name.upper() == str(UDFType.EXTRACT_OBJECT):
+            handle_bind_extract_object_function(node, self)
+            return
         # bind all the children
         for child in node.children:
             self.bind(child)
 
         udf_obj = self._catalog.get_udf_catalog_entry_by_name(node.name)
         if udf_obj is None:
             err_msg = (
@@ -249,15 +235,15 @@
 
         if udf_obj.type == "HuggingFace":
             node.function = assign_hf_udf(udf_obj)
 
         else:
             if udf_obj.type == "ultralytics":
                 # manually set the impl_path for yolo udfs we only handle object
-                # detection for now, hopefully this can be generelized
+                # detection for now, hopefully this can be generalized
                 udf_obj.impl_file_path = (
                     Path(f"{EVA_DEFAULT_DIR}/udfs/yolo_object_detector.py")
                     .absolute()
                     .as_posix()
                 )
 
             # Verify the consistency of the UDF. If the checksum of the UDF does not
```

### Comparing `evadb-0.2.3.post0/eva/binder/statement_binder_context.py` & `evadb-0.2.4/eva/binder/statement_binder_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             Union[TupleValueExpression, FunctionExpression, UdfIOCatalogEntry]
         ],
     ):
         """
         Add a alias -> derived table column mapping
         Arguments:
             alias (str): name of alias
-            target_list: list of Tuplevalue Expression or FunctionExpression or UdfIOCatalogEntry
+            target_list: list of TupleValueExpression or FunctionExpression or UdfIOCatalogEntry
         """
         self._check_duplicate_alias(alias)
         col_alias_map = {}
         for expr in target_list:
             if isinstance(expr, FunctionExpression):
                 for obj in expr.output_objs:
                     col_alias_map[obj.name] = obj
@@ -104,44 +104,44 @@
 
     def get_binded_column(
         self, col_name: str, alias: str = None
     ) -> Tuple[str, CatalogColumnType]:
         """
         Find the binded column object
         Arguments:
-            col_name (str): columna name
+            col_name (str): column name
             alias (str): alias name
 
         Returns:
             A tuple of alias and column object
         """
 
         def raise_error():
             err_msg = f"Found invalid column {col_name}"
             logger.error(err_msg)
             raise BinderError(err_msg)
 
         if not alias:
             alias, col_obj = self._search_all_alias_maps(col_name)
         else:
-            # serach in all alias maps
+            # search in all alias maps
             col_obj = self._check_table_alias_map(alias, col_name)
             if not col_obj:
                 col_obj = self._check_derived_table_alias_map(alias, col_name)
 
         if col_obj:
             return alias, col_obj
 
         raise_error()
 
     def _check_table_alias_map(self, alias, col_name) -> ColumnCatalogEntry:
         """
         Find the column object in table alias map
         Arguments:
-            col_name (str): columna name
+            col_name (str): column name
             alias (str): alias name
 
         Returns:
             column object
         """
         table_obj = self._table_alias_map.get(alias, None)
         if table_obj:
```

### Comparing `evadb-0.2.3.post0/eva/catalog/__init__.py` & `evadb-0.2.4/eva/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/catalog_manager.py` & `evadb-0.2.4/eva/catalog/catalog_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import shutil
 from pathlib import Path
 from typing import List
 
-from eva.catalog.catalog_type import ColumnType, IndexType, TableType, VideoColumnName
+from eva.catalog.catalog_type import (
+    ColumnType,
+    TableType,
+    VectorStoreType,
+    VideoColumnName,
+)
 from eva.catalog.catalog_utils import (
     cleanup_storage,
     construct_udf_cache_catalog_entry,
     get_image_table_column_definitions,
     get_video_table_column_definitions,
     xform_column_definitions_to_catalog_entries,
 )
@@ -303,20 +308,20 @@
 
     """ Index related services. """
 
     def insert_index_catalog_entry(
         self,
         name: str,
         save_file_path: str,
-        index_type: IndexType,
+        vector_store_type: VectorStoreType,
         feat_column: ColumnCatalogEntry,
         udf_signature: str,
     ) -> IndexCatalogEntry:
         index_catalog_entry = self._index_service.insert_entry(
-            name, save_file_path, index_type, feat_column, udf_signature
+            name, save_file_path, vector_store_type, feat_column, udf_signature
         )
         return index_catalog_entry
 
     def get_index_catalog_entry_by_name(self, name: str) -> IndexCatalogEntry:
         return self._index_service.get_entry_by_name(name)
 
     def get_index_catalog_entry_by_column_and_udf_signature(
```

### Comparing `evadb-0.2.3.post0/eva/catalog/catalog_type.py` & `evadb-0.2.4/eva/catalog/catalog_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,20 +88,17 @@
             np_type = np.dtype(object)
         else:
             raise ValueError("Can not auto convert %s to numpy type" % t)
 
         return np_type
 
 
-class IndexType(EVAEnum):
-    HNSW  # noqa: F821
-
-    @classmethod
-    def is_faiss_index_type(cls, t):
-        return t in [cls.HNSW]
+class VectorStoreType(EVAEnum):
+    FAISS  # noqa: F821
+    QDRANT  # noqa: F821
 
 
 class VideoColumnName(EVAEnum):
     name  # noqa: F821
     id  # noqa: F821
     data  # noqa: F821
     seconds  # noqa: F821
```

### Comparing `evadb-0.2.3.post0/eva/catalog/catalog_utils.py` & `evadb-0.2.4/eva/catalog/catalog_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,27 @@
 from eva.catalog.models.udf_catalog import UdfCatalogEntry
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.expression.function_expression import FunctionExpression
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.create_statement import ColConstraintInfo, ColumnDefinition
 from eva.utils.generic_utils import get_str_hash, remove_directory_contents
 
+CATALOG_TABLES = [
+    "column_catalog",
+    "table_catalog",
+    "depend_column_and_udf_cache",
+    "udf_cache",
+    "udf_catalog",
+    "depend_udf_and_udf_cache",
+    "index_catalog",
+    "udfio_catalog",
+    "udf_cost_catalog",
+    "udf_metadata_catalog",
+]
+
 
 def is_video_table(table: TableCatalogEntry):
     return table.table_type == TableType.VIDEO_DATA
 
 
 def is_string_col(col: ColumnCatalogEntry):
     return col.type == ColumnType.TEXT or col.array_type == NdArrayType.STR
@@ -130,16 +143,15 @@
 ) -> UdfCacheCatalogEntry:
     """Constructs a udf cache catalog entry from a given function expression.
     It is assumed that the function expression has already been bound using the binder.
     The catalog entry is populated with dependent udfs and columns by traversing the
     expression tree. The cache name is represented by the signature of the function
     expression.
     Args:
-        func_expr (FunctionExpression): the function expression with which the cache is
-        assoicated
+        func_expr (FunctionExpression): the function expression with which the cache is associated
     Returns:
         UdfCacheCatalogEntry: the udf cache catalog entry
     """
     udf_depends = []
     col_depends = []
     for expr in func_expr.find_all(FunctionExpression):
         udf_depends.append(expr.udf_obj.row_id)
```

### Comparing `evadb-0.2.3.post0/eva/catalog/models/__init__.py` & `evadb-0.2.4/eva/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/models/association_models.py` & `evadb-0.2.4/eva/catalog/models/association_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from sqlalchemy import Column, ForeignKey, Table, UniqueConstraint
 
 from eva.catalog.models.base_model import BaseModel
 
-# dependency table to maintain a many-to-many relationship between udf_catalog and udf_cache_catalog. This is important to ensure that any changes to udf are propogated to udf_cache. For example, deletion of a udf should also clear the associated caches.
+# dependency table to maintain a many-to-many relationship between udf_catalog and udf_cache_catalog. This is important to ensure that any changes to udf are propagated to udf_cache. For example, deletion of a udf should also clear the associated caches.
 
 depend_udf_and_udf_cache = Table(
     "depend_udf_and_udf_cache",
     BaseModel.metadata,
     Column("_udf_id", ForeignKey("udf_catalog._row_id")),
     Column("_udf_cache_id", ForeignKey("udf_cache._row_id")),
     UniqueConstraint("_udf_id", "_udf_cache_id"),
```

### Comparing `evadb-0.2.3.post0/eva/catalog/models/base_model.py` & `evadb-0.2.4/eva/catalog/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 class CustomModel:
     """This overrides the default `_declarative_constructor` constructor.
 
     It skips the attributes that are not present for the model, thus if a
     dict is passed with some unknown attributes for the model on creation,
-    it won't complain for `unkwnown field`s.
+    it won't complain for `unknown field`s.
     Declares and int `_row_id` field for all tables
     """
 
     query = db_session.query_property()
     _row_id = Column("_row_id", Integer, primary_key=True)
 
     def __init__(self, **kwargs):
```

### Comparing `evadb-0.2.3.post0/eva/catalog/models/column_catalog.py` & `evadb-0.2.4/eva/catalog/models/column_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from eva.catalog.catalog_type import ColumnType, Dimension, NdArrayType
 from eva.catalog.models.association_models import depend_column_and_udf_cache
 from eva.catalog.models.base_model import BaseModel
 
 
 class ColumnCatalog(BaseModel):
     """The `ColumnCatalog` catalog stores information about the columns of the table.
-    It maintinas the following information for each column
+    It maintains the following information for each column
     `_row_id:` an autogenerated identifier
     `_name: ` name of the column
     `_type:` the type of the column, refer `ColumnType`
     `_is_nullable:` which indicates whether the column is nullable
     `_array_type:` the type of array, as specified in `NdArrayType` (or `None` if the column is a primitive type)
     `_array_dimensions:` the dimensions of the array (if `_array_type` is not `None`)
     `_table_id:` the `_row_id` of the `TableCatalog` entry to which the column belongs
@@ -62,14 +62,19 @@
     _dep_caches = relationship(
         "UdfCacheCatalog",
         secondary=depend_column_and_udf_cache,
         back_populates="_col_depends",
         cascade="all, delete",
     )
 
+    # Column that index is built on.
+    _index_column = relationship(
+        "IndexCatalog", back_populates="_feat_column", cascade="all, delete"
+    )
+
     def __init__(
         self,
         name: str,
         type: ColumnType,
         is_nullable: bool = False,
         array_type: NdArrayType = None,
         array_dimensions: Tuple[int] = (),
@@ -84,15 +89,15 @@
 
     @property
     def array_dimensions(self):
         return literal_eval(self._array_dimensions)
 
     @array_dimensions.setter
     def array_dimensions(self, value: Tuple[int]):
-        # This tranformation converts the ANYDIM enum to
+        # This transformation converts the ANYDIM enum to
         # None which is expected by petastorm.
         # Before adding data, petastorm verifies _is_compliant_shape
         # and any unknown dimension is expected to be None
         # https://petastorm.readthedocs.io/en/latest/_modules/petastorm/codecs.html#DataframeColumnCodec.encode
         dimensions = []
         for dim in value:
             if dim == Dimension.ANYDIM:
```

### Comparing `evadb-0.2.3.post0/eva/catalog/models/index_catalog.py` & `evadb-0.2.4/eva/catalog/models/index_catalog.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,45 +14,50 @@
 # limitations under the License.
 from dataclasses import dataclass
 
 from sqlalchemy import Column, ForeignKey, Integer, String
 from sqlalchemy.orm import relationship
 from sqlalchemy.types import Enum
 
-from eva.catalog.catalog_type import IndexType
+from eva.catalog.catalog_type import VectorStoreType
 from eva.catalog.models.base_model import BaseModel
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
 
 
 class IndexCatalog(BaseModel):
     """The `IndexCatalogEntry` catalog stores information about all the indexes in the system.
     `_row_id:` an autogenerated unique identifier.
     `_name:` the name of the index.
     `_save_file_path:` the path to the index file on disk
-    `_type:` the type of the index (refer to `IndexType`)
+    `_type:` the type of the index (refer to `VectorStoreType`)
     `_feat_column_id:` the `_row_id` of the `ColumnCatalog` entry for the column on which the index is built.
     `_udf_signature:` if the index is created by running udf expression on input column, this will store
                       the udf signature of the used udf. Otherwise, this field is None.
     """
 
     __tablename__ = "index_catalog"
 
     _name = Column("name", String(100), unique=True)
     _save_file_path = Column("save_file_path", String(128))
-    _type = Column("type", Enum(IndexType), default=Enum)
-    _feat_column_id = Column("column_id", Integer, ForeignKey("column_catalog._row_id"))
+    _type = Column("type", Enum(VectorStoreType), default=Enum)
+    _feat_column_id = Column(
+        "column_id", Integer, ForeignKey("column_catalog._row_id", ondelete="CASCADE")
+    )
     _udf_signature = Column("udf", String, default=None)
 
-    _feat_column = relationship("ColumnCatalog")
+    _feat_column = relationship(
+        "ColumnCatalog",
+        back_populates="_index_column",
+    )
 
     def __init__(
         self,
         name: str,
         save_file_path: str,
-        type: IndexType,
+        type: VectorStoreType,
         feat_column_id: int = None,
         udf_signature: str = None,
     ):
         self._name = name
         self._save_file_path = save_file_path
         self._type = type
         self._feat_column_id = feat_column_id
@@ -75,12 +80,12 @@
 class IndexCatalogEntry:
     """Dataclass representing an entry in the IndexCatalogEntry.
     This is done to ensure we don't expose the sqlalchemy dependencies beyond catalog service. Further, sqlalchemy does not allow sharing of objects across threads.
     """
 
     name: str
     save_file_path: str
-    type: IndexType
+    type: VectorStoreType
     row_id: int = None
     feat_column_id: int = None
     udf_signature: str = None
     feat_column: ColumnCatalogEntry = None
```

### Comparing `evadb-0.2.3.post0/eva/catalog/models/table_catalog.py` & `evadb-0.2.4/eva/catalog/models/table_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/models/udf_cache_catalog.py` & `evadb-0.2.4/eva/catalog/models/udf_cache_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/models/udf_catalog.py` & `evadb-0.2.4/eva/catalog/models/udf_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/models/udf_cost_catalog.py` & `evadb-0.2.4/eva/catalog/models/udf_cost_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/models/udf_io_catalog.py` & `evadb-0.2.4/eva/catalog/models/udf_io_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.4/eva/catalog/models/udf_metadata_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/schema_utils.py` & `evadb-0.2.4/eva/catalog/schema_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/__init__.py` & `evadb-0.2.4/eva/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/base_service.py` & `evadb-0.2.4/eva/catalog/services/base_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/column_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/index_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/index_catalog_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
 from sqlalchemy.orm.exc import NoResultFound
 
-from eva.catalog.catalog_type import IndexType
+from eva.catalog.catalog_type import VectorStoreType
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
 from eva.catalog.models.index_catalog import IndexCatalog, IndexCatalogEntry
 from eva.catalog.services.base_service import BaseService
 from eva.utils.logging_manager import logger
 
 
 class IndexCatalogService(BaseService):
     def __init__(self):
         super().__init__(IndexCatalog)
 
     def insert_entry(
         self,
         name: str,
         save_file_path: str,
-        type: IndexType,
+        type: VectorStoreType,
         feat_column: ColumnCatalogEntry,
         udf_signature: str,
     ) -> IndexCatalogEntry:
         index_entry = IndexCatalog(
             name, save_file_path, type, feat_column.row_id, udf_signature
         )
         index_entry = index_entry.save()
```

### Comparing `evadb-0.2.3.post0/eva/catalog/services/table_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/udf_cache_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/udf_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.4/eva/catalog/services/udf_metadata_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/catalog/sql_config.py` & `evadb-0.2.4/eva/catalog/sql_config.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/configuration/__init__.py` & `evadb-0.2.4/eva/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/configuration/bootstrap_environment.py` & `evadb-0.2.4/eva/configuration/bootstrap_environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     default_install_dir = eva_installation_dir
     dataset_location = EVA_DEFAULT_DIR / EVA_DATASET_DIR
     index_dir = eva_config_dir / INDEX_DIR
     cache_dir = eva_config_dir / CACHE_DIR
     s3_dir = eva_config_dir / S3_DOWNLOAD_DIR
     tmp_dir = eva_config_dir / TMP_DIR
 
+    if not dataset_location.exists():
+        dataset_location.mkdir(parents=True, exist_ok=True)
     if not eva_config_dir.exists():
         eva_config_dir.mkdir(parents=True, exist_ok=True)
     if not index_dir.exists():
         index_dir.mkdir(parents=True, exist_ok=True)
     if not cache_dir.exists():
         cache_dir.mkdir(parents=True, exist_ok=True)
     if not s3_dir.exists():
```

### Comparing `evadb-0.2.3.post0/eva/configuration/configuration_manager.py` & `evadb-0.2.4/eva/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/configuration/constants.py` & `evadb-0.2.4/eva/configuration/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import eva
 from eva.version import VERSION
 
 EVA_INSTALLATION_DIR = Path(eva.__file__).parent
 EVA_ROOT_DIR = Path(eva.__file__).parent.parent
 # Using eva version to govern the EVA_DEFAULT_DIR
 # This means we won't support backward compatibility as each version will maintain its own copy of database.
-# Ideally, if the new release is not breaking backward compatibilty, we can keep using the same copy.
+# Ideally, if the new release is not breaking backward compatibility, we can keep using the same copy.
 # We can revisit it later
 EVA_DEFAULT_DIR = Path.home() / ".eva" / str(VERSION)
 EVA_DATASET_DIR = "eva_datasets"
 EVA_CONFIG_FILE = "eva.yml"
 UDF_DIR = "udfs"
 CATALOG_DIR = "catalog"
 INDEX_DIR = "index"
```

### Comparing `evadb-0.2.3.post0/eva/constants.py` & `evadb-0.2.4/eva/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/eva.yml` & `evadb-0.2.4/eva/eva.yml`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,14 @@
 00000240: 636f 7264 5374 6f72 6167 6545 6e67 696e  cordStorageEngin
 00000250: 6522 0a20 2069 6d61 6765 5f65 6e67 696e  e".  image_engin
 00000260: 653a 2022 6576 612e 7374 6f72 6167 652e  e: "eva.storage.
 00000270: 696d 6167 655f 7374 6f72 6167 655f 656e  image_storage_en
 00000280: 6769 6e65 2e49 6d61 6765 5374 6f72 6167  gine.ImageStorag
 00000290: 6545 6e67 696e 6522 0a73 6572 7665 723a  eEngine".server:
 000002a0: 0a20 2068 6f73 743a 2022 302e 302e 302e  .  host: "0.0.0.
-000002b0: 3022 0a20 2070 6f72 743a 2035 3433 320a  0".  port: 5432.
+000002b0: 3022 0a20 2070 6f72 743a 2038 3830 330a  0".  port: 8803.
 000002c0: 2020 736f 636b 6574 5f74 696d 656f 7574    socket_timeout
 000002d0: 3a20 3630 0a0a 6578 7065 7269 6d65 6e74  : 60..experiment
 000002e0: 616c 3a0a 2020 7261 793a 2046 616c 7365  al:.  ray: False
 000002f0: 0a0a 7468 6972 645f 7061 7274 793a 0a20  ..third_party:. 
 00000300: 206f 7065 6e61 695f 6170 695f 6b65 793a   openai_api_key:
 00000310: 2022 22                                   ""
```

### Comparing `evadb-0.2.3.post0/eva/eva_cmd_client.py` & `evadb-0.2.4/eva/eva_cmd_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import argparse
 import asyncio
 import sys
 from os.path import abspath, dirname, join
 
 from eva.utils.logging_manager import logger
 
 """
@@ -25,33 +26,50 @@
 EVA_CODE_DIR = abspath(join(THIS_DIR, ".."))
 sys.path.append(EVA_CODE_DIR)
 
 from eva.configuration.configuration_manager import ConfigurationManager  # noqa: E402
 from eva.server.interpreter import start_cmd_client  # noqa: E402
 
 
-async def eva_client():
+async def eva_client(host: str, port: int):
     """
-    Start the eva system
+    Start the eva client
     """
 
-    # Get the hostname and port information from the configuration file
-    config = ConfigurationManager()
-    host = config.get_value("server", "host")
-    port = config.get_value("server", "port")
-
     # Launch client
     try:
         await start_cmd_client(host, port)
     except KeyboardInterrupt:
         pass
     except Exception as e:
         logger.critical(e)
         raise e
 
 
 def main():
-    asyncio.run(eva_client())
+    parser = argparse.ArgumentParser(description="EVA Client")
+
+    parser.add_argument(
+        "--host",
+        help="Specify the host address of the server you want to connect to.",
+    )
+
+    parser.add_argument(
+        "--port",
+        help="Specify the port number of the server you want to connect to.",
+    )
+
+    ## PARSE ARGS
+    args, unknown = parser.parse_known_args()
+
+    host = (
+        args.host if args.host else ConfigurationManager().get_value("server", "host")
+    )
+
+    port = (
+        args.port if args.port else ConfigurationManager().get_value("server", "port")
+    )
+    asyncio.run(eva_client(host, port))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evadb-0.2.3.post0/eva/eva_server.py` & `evadb-0.2.4/eva/eva_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,23 +28,16 @@
 sys.path.append(EVA_CODE_DIR)
 
 from eva.configuration.configuration_manager import ConfigurationManager  # noqa: E402
 from eva.server.server import EvaServer  # noqa: E402
 from eva.udfs.udf_bootstrap_queries import init_builtin_udfs  # noqa: E402
 
 
-async def start_eva_server():
-    """
-    Start the eva server
-    """
-    # Get the hostname and port information from the configuration file
-    config = ConfigurationManager()
-    host = config.get_value("server", "host")
-    port = config.get_value("server", "port")
-
+async def start_eva_server(host: str, port: int):
+    """Start the eva server"""
     eva_server = EvaServer()
 
     await eva_server.start_eva_server(host, port)
 
 
 def stop_server():
     """
@@ -57,14 +50,24 @@
     return 0
 
 
 def main():
     parser = argparse.ArgumentParser(description="EVA Server")
 
     parser.add_argument(
+        "--host",
+        help="Specify the host address on which the server will start.",
+    )
+
+    parser.add_argument(
+        "--port",
+        help="Specify the port number on which the server will start.",
+    )
+
+    parser.add_argument(
         "--start",
         help="start server",
         action="store_true",
         default=True,
     )
 
     parser.add_argument(
@@ -77,18 +80,26 @@
     ## PARSE ARGS
     args, unknown = parser.parse_known_args()
 
     # Stop server
     if args.stop:
         return stop_server()
 
+    host = (
+        args.host if args.host else ConfigurationManager().get_value("server", "host")
+    )
+
+    port = (
+        args.port if args.port else ConfigurationManager().get_value("server", "port")
+    )
+
     # Start server
     if args.start:
         mode = ConfigurationManager().get_value("core", "mode")
         init_builtin_udfs(mode=mode)
 
-        asyncio.run(start_eva_server())
+        asyncio.run(start_eva_server(host=host, port=int(port)))
 
 
 if __name__ == "__main__":
     # execute only if run as the entry point into the program
     main()
```

### Comparing `evadb-0.2.3.post0/eva/executor/__init__.py` & `evadb-0.2.4/eva/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/abstract_executor.py` & `evadb-0.2.4/eva/executor/abstract_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __init__(self, node: AbstractPlan):
         self._node = node
         self._children = []
 
     def append_child(self, child: AbstractExecutor):
         """
-        appends a child exector node
+        appends a child executor node
 
         Arguments:
             child {AbstractExecutor} -- child node
         """
         self._children.append(child)
 
     @property
@@ -59,13 +59,13 @@
         return self._node
 
     @abstractmethod
     def exec(self, *args, **kwargs) -> Iterable[Batch]:
         """
         This method is implemented by every executor.
         Contains logic for that executor;
-        For retrival based executor : It fetchs frame batches from
+        For retrieval based executor : It fetches frame batches from
         child nodes and emits it to parent node.
         """
 
     def __call__(self, *args, **kwargs) -> Generator[Batch, None, None]:
         yield from self.exec(*args, **kwargs)
```

### Comparing `evadb-0.2.3.post0/eva/executor/apply_and_merge_executor.py` & `evadb-0.2.4/eva/executor/seq_scan_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,44 +11,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
 from eva.executor.abstract_executor import AbstractExecutor
+from eva.executor.executor_utils import apply_predicate, apply_project
 from eva.models.storage.batch import Batch
-from eva.plan_nodes.apply_and_merge_plan import ApplyAndMergePlan
+from eva.plan_nodes.seq_scan_plan import SeqScanPlan
 
 
-class ApplyAndMergeExecutor(AbstractExecutor):
+class SequentialScanExecutor(AbstractExecutor):
     """
-    Apply the function expression to the input data, merge the output of the function
-    with the input data, and yield the result to the parent. The current implementation
-    assumes an inner join while merging. Therefore, if the function does not return any
-    output, the input rows are dropped.
+    Applies predicates to filter the frames which satisfy the condition
     Arguments:
-        node (AbstractPlan): ApplyAndMergePlan
+        node (AbstractPlan): The SequentialScanPlan
 
     """
 
-    def __init__(self, node: ApplyAndMergePlan):
+    def __init__(self, node: SeqScanPlan):
         super().__init__(node)
-        self.func_expr = node.func_expr
-        self.do_unnest = node.do_unnest
+        self.predicate = node.predicate
+        self.project_expr = node.columns
         self.alias = node.alias
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         for batch in child_executor.exec(**kwargs):
-            res = self.func_expr.evaluate(batch)
-            if not res.empty():
-                if self.do_unnest:
-                    res.unnest()
-
-                # Merge the results to the input.
-                # This assumes that the batch index is preserved by the function
-                # call. Since both the batch and the results are sorted, we could
-                # perform a sorted merge, though the typical small size of the
-                # batch and results should not significantly impact performance.
-                merged_batch = Batch.join(batch, res)
-                merged_batch.reset_index()
-                yield merged_batch
+            # apply alias to the batch
+            # id, data -> myvideo.id, myvideo.data
+            if self.alias:
+                batch.modify_column_alias(self.alias)
+
+            # We do the predicate first
+            batch = apply_predicate(batch, self.predicate)
+            # Then do project
+            batch = apply_project(batch, self.project_expr)
+
+            if not batch.empty():
+                yield batch
```

### Comparing `evadb-0.2.3.post0/eva/executor/create_executor.py` & `evadb-0.2.4/eva/executor/create_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/create_index_executor.py` & `evadb-0.2.4/eva/executor/create_index_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,137 +10,118 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 
-import faiss
-import numpy as np
 import pandas as pd
 
 from eva.catalog.catalog_manager import CatalogManager
-from eva.catalog.catalog_type import IndexType
 from eva.catalog.sql_config import IDENTIFIER_COLUMN
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.executor.abstract_executor import AbstractExecutor
-from eva.executor.executor_utils import ExecutorError
+from eva.executor.executor_utils import ExecutorError, handle_vector_store_params
 from eva.models.storage.batch import Batch
 from eva.plan_nodes.create_index_plan import CreateIndexPlan
 from eva.storage.storage_engine import StorageEngine
+from eva.third_party.vector_stores.types import FeaturePayload
+from eva.third_party.vector_stores.utils import VectorStoreFactory
 from eva.utils.logging_manager import logger
 
 
-def create_faiss_index(index_type: IndexType, input_dim: int):
-    # Refernce to Faiss documentation.
-    # IDMap: https://github.com/facebookresearch/faiss/wiki/Pre--and-post-processing#faiss-id-mapping
-    # Other index types: https://github.com/facebookresearch/faiss/wiki/The-index-factory
-
-    if index_type == IndexType.HNSW:
-        # HSNW is the actual index. Faiss also provides
-        # a secondary mapping (IDMap) to map from ID inside index to
-        # our given ID.
-        return faiss.IndexIDMap2(faiss.IndexHNSWFlat(input_dim, 32))
-
-
 class CreateIndexExecutor(AbstractExecutor):
     def __init__(self, node: CreateIndexPlan):
         super().__init__(node)
 
     def exec(self, *args, **kwargs):
         catalog_manager = CatalogManager()
         if catalog_manager.get_index_catalog_entry_by_name(self.node.name):
             msg = f"Index {self.node.name} already exists."
             logger.error(msg)
             raise ExecutorError(msg)
 
-        # Get the index type.
-        index_type = self.node.index_type
-
-        assert IndexType.is_faiss_index_type(
-            index_type
-        ), "Index type {} is not supported.".format(index_type)
-
-        if IndexType.is_faiss_index_type(index_type):
-            self._create_faiss_index()
+        self.index_path = self._get_index_save_path()
+        self.index = None
+        self._create_index()
 
         yield Batch(
             pd.DataFrame(
                 [f"Index {self.node.name} successfully added to the database."]
             )
         )
 
     def _get_index_save_path(self) -> Path:
         index_dir = Path(ConfigurationManager().get_value("storage", "index_dir"))
         if not index_dir.exists():
             index_dir.mkdir(parents=True, exist_ok=True)
         return str(
-            index_dir / Path("{}_{}.index".format(self.node.index_type, self.node.name))
+            index_dir
+            / Path("{}_{}.index".format(self.node.vector_store_type, self.node.name))
         )
 
-    def _create_faiss_index(self):
+    def _create_index(self):
         try:
-            catalog_manager = CatalogManager()
-
             # Get feature tables.
             feat_catalog_entry = self.node.table_ref.table.table_obj
 
             # Get feature column.
             feat_col_name = self.node.col_list[0].name
             feat_column = [
                 col for col in feat_catalog_entry.columns if col.name == feat_col_name
             ][0]
 
-            # Get udf function.
-            udf_func = self.node.udf_func
-
             # Add features to index.
             # TODO: batch size is hardcoded for now.
-            index = None
             input_dim = -1
             storage_engine = StorageEngine.factory(feat_catalog_entry)
-            for input_batch in storage_engine.read(feat_catalog_entry, 1):
-                if udf_func:
+            for input_batch in storage_engine.read(feat_catalog_entry):
+                if self.node.udf_func:
                     # Create index through UDF expression.
                     # UDF(input column) -> 2 dimension feature vector.
                     input_batch.modify_column_alias(feat_catalog_entry.name.lower())
                     feat_batch = self.node.udf_func.evaluate(input_batch)
                     feat_batch.drop_column_alias()
                     input_batch.drop_column_alias()
-                    feat = feat_batch.column_as_numpy_array("features")[0]
+                    feat = feat_batch.column_as_numpy_array("features")
                 else:
-                    # Create index on the feature table direclty.
+                    # Create index on the feature table directly.
                     # Pandas wraps numpy array as an object inside a numpy
                     # array. Use zero index to get the actual numpy array.
-                    feat = input_batch.column_as_numpy_array(feat_col_name)[0]
+                    feat = input_batch.column_as_numpy_array(feat_col_name)
+
+                row_id = input_batch.column_as_numpy_array(IDENTIFIER_COLUMN)
 
-                # Transform to 2-D.
-                feat = feat.reshape(1, -1)
+                for i in range(len(input_batch)):
+                    row_feat = feat[i].reshape(1, -1)
+                    if self.index is None:
+                        input_dim = row_feat.shape[1]
+                        self.index = VectorStoreFactory.init_vector_store(
+                            self.node.vector_store_type,
+                            self.node.name,
+                            **handle_vector_store_params(
+                                self.node.vector_store_type, self.index_path
+                            ),
+                        )
+                        self.index.create(input_dim)
 
-                if index is None:
-                    input_dim = feat.shape[-1]
-                    index = create_faiss_index(self.node.index_type, input_dim)
-
-                # Row ID for mapping back to the row.
-                row_id = input_batch.column_as_numpy_array(IDENTIFIER_COLUMN)[0]
-                index.add_with_ids(feat, np.array([row_id]))
+                    # Row ID for mapping back to the row.
+                    self.index.add([FeaturePayload(row_id[i], row_feat)])
 
             # Persist index.
-            faiss.write_index(index, self._get_index_save_path())
+            self.index.persist()
 
             # Save to catalog.
-            catalog_manager.insert_index_catalog_entry(
+            CatalogManager().insert_index_catalog_entry(
                 self.node.name,
-                self._get_index_save_path(),
-                self.node.index_type,
+                self.index_path,
+                self.node.vector_store_type,
                 feat_column,
-                udf_func.signature() if udf_func else None,
+                self.node.udf_func.signature() if self.node.udf_func else None,
             )
         except Exception as e:
-            # Roll back in reverse order.
-            # Delete on-disk index.
-            index_path = Path(self._get_index_save_path())
-            if index_path.exists():
-                index_path.unlink()
+            # Delete index.
+            if self.index:
+                self.index.delete()
 
             # Throw exception back to user.
             raise ExecutorError(str(e))
```

### Comparing `evadb-0.2.3.post0/eva/executor/create_mat_view_executor.py` & `evadb-0.2.4/eva/executor/create_mat_view_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/create_udf_executor.py` & `evadb-0.2.4/eva/executor/create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/delete_executor.py` & `evadb-0.2.4/eva/executor/delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/drop_executor.py` & `evadb-0.2.4/eva/executor/drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/drop_udf_executor.py` & `evadb-0.2.4/eva/executor/drop_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/execution_context.py` & `evadb-0.2.4/eva/executor/execution_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,27 @@
     @property
     def gpus(self):
         return self._gpus
 
     def _populate_gpu_from_config(self) -> List:
         # Populate GPU IDs from yaml config file.
         gpu_conf = self._config_manager.get_value("executor", "gpu_ids")
-        availble_gpus = [i for i in range(get_gpu_count())]
-        return list(set(availble_gpus) & set(gpu_conf))
+        available_gpus = [i for i in range(get_gpu_count())]
+        return list(set(available_gpus) & set(gpu_conf))
 
     def _populate_gpu_from_env(self) -> List:
         # Populate GPU IDs from env variable.
         gpu_conf = map(
             lambda x: x.strip(),
             os.environ.get("CUDA_VISIBLE_DEVICES", "").strip().split(","),
         )
         gpu_conf = list(filter(lambda x: x, gpu_conf))
         gpu_conf = [int(gpu_id) for gpu_id in gpu_conf]
-        availble_gpus = [i for i in range(get_gpu_count())]
-        return list(set(availble_gpus) & set(gpu_conf))
+        available_gpus = [i for i in range(get_gpu_count())]
+        return list(set(available_gpus) & set(gpu_conf))
 
     def _populate_gpu_ids(self) -> List:
         # Populate available GPU IDs from Torch library. Then, select subset of GPUs
         # from available GPUs based on user configuration.
         if not is_gpu_available():
             return []
         gpus = self._populate_gpu_from_config()
```

### Comparing `evadb-0.2.3.post0/eva/executor/executor_utils.py` & `evadb-0.2.4/eva/executor/executor_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import os
 from pathlib import Path
 from typing import Generator, List
 
 import cv2
 
 from eva.catalog.catalog_manager import CatalogManager
+from eva.catalog.catalog_type import VectorStoreType
 from eva.expression.abstract_expression import AbstractExpression
 from eva.models.storage.batch import Batch
 from eva.parser.table_ref import TableInfo
 from eva.parser.types import FileFormatType
 from eva.utils.logging_manager import logger
 
 
@@ -93,7 +94,31 @@
 def validate_media(file_path: Path, media_type: FileFormatType) -> bool:
     if media_type == FileFormatType.VIDEO:
         return validate_video(file_path)
     elif media_type == FileFormatType.IMAGE:
         return validate_image(file_path)
     else:
         raise ValueError(f"Unsupported Media type {str(media_type)}")
+
+
+def handle_vector_store_params(
+    vector_store_type: VectorStoreType, index_path: str
+) -> dict:
+    """Handle vector store parameters based on the vector store type and index path.
+
+    Args:
+        vector_store_type (VectorStoreType): The type of vector store.
+        index_path (str): The path to store the index.
+
+    Returns:
+        dict: Dictionary containing the appropriate vector store parameters.
+
+
+    Raises:
+        ValueError: If the vector store type in the node is not supported.
+    """
+    if vector_store_type == VectorStoreType.FAISS:
+        return {"index_path": index_path}
+    elif vector_store_type == VectorStoreType.QDRANT:
+        return {"index_db": str(Path(index_path).parent)}
+    else:
+        raise ValueError("Unsupported vector store type: {}".format(vector_store_type))
```

### Comparing `evadb-0.2.3.post0/eva/executor/explain_executor.py` & `evadb-0.2.4/eva/executor/explain_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class ExplainExecutor(AbstractExecutor):
     def __init__(self, node: ExplainPlan):
         super().__init__(node)
 
     def exec(self, *args, **kwargs):
         # Traverse optimized physical plan, which is commonly supported.
-        # Logical plan can be also printted by passing explainable_opr
+        # Logical plan can be also printed by passing explainable_opr
         # attribute of the node, but is not done for now.
         plan_str = self._exec(self._node.children[0], 0)
         yield Batch(pd.DataFrame([plan_str]))
 
     def _exec(self, node: AbstractPlan, depth: int):
         cur_str = " " * depth * 4 + "|__ " + str(node.__class__.__name__) + "\n"
         for child in node.children:
```

### Comparing `evadb-0.2.3.post0/eva/executor/faiss_index_scan_executor.py` & `evadb-0.2.4/eva/executor/vector_index_scan_executor.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,47 +10,55 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-import faiss
 import pandas as pd
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.sql_config import IDENTIFIER_COLUMN
 from eva.executor.abstract_executor import AbstractExecutor
+from eva.executor.executor_utils import handle_vector_store_params
 from eva.models.storage.batch import Batch
-from eva.plan_nodes.faiss_index_scan_plan import FaissIndexScanPlan
+from eva.plan_nodes.vector_index_scan_plan import VectorIndexScanPlan
+from eva.third_party.vector_stores.types import VectorIndexQuery
+from eva.third_party.vector_stores.utils import VectorStoreFactory
 
 
 # Helper function for getting row_id column alias.
 def get_row_id_column_alias(column_list):
     for column in column_list:
         alias, col_name = column.split(".")
         if col_name == IDENTIFIER_COLUMN:
             return alias
 
 
-class FaissIndexScanExecutor(AbstractExecutor):
-    def __init__(self, node: FaissIndexScanPlan):
+class VectorIndexScanExecutor(AbstractExecutor):
+    def __init__(self, node: VectorIndexScanPlan):
         super().__init__(node)
+
         self.index_name = node.index_name
         self.limit_count = node.limit_count
         self.search_query_expr = node.search_query_expr
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         catalog_manager = CatalogManager()
 
         # Fetch the index from disk.
         index_catalog_entry = catalog_manager.get_index_catalog_entry_by_name(
             self.index_name
         )
-        index = faiss.read_index(index_catalog_entry.save_file_path)
+        self.index_path = index_catalog_entry.save_file_path
+        self.index = VectorStoreFactory.init_vector_store(
+            self.node.vector_store_type,
+            self.index_name,
+            **handle_vector_store_params(self.node.vector_store_type, self.index_path)
+        )
 
         # Get the query feature vector. Create a dummy
         # batch to retreat a single file path.
         dummy_batch = Batch(
             frames=pd.DataFrame(
                 {"0": [0]},
             )
@@ -58,33 +66,33 @@
         search_batch = self.search_query_expr.evaluate(dummy_batch)
 
         # Scan index. The search batch comes from the Open call.
         feature_col_name = self.search_query_expr.output_objs[0].name
         search_batch.drop_column_alias()
         search_feat = search_batch.column_as_numpy_array(feature_col_name)[0]
         search_feat = search_feat.reshape(1, -1)
-        dis_np, row_id_np = index.search(search_feat, self.limit_count.value)
-
-        distance_list, row_id_list = [], []
-        for dis, row_id in zip(dis_np[0], row_id_np[0]):
-            distance_list.append(dis)
-            row_id_list.append(row_id)
+        index_result = self.index.query(
+            VectorIndexQuery(search_feat, self.limit_count.value)
+        )
+        # todo support queries over distance as well
+        # distance_list = index_result.similarities
+        row_id_np = index_result.ids
 
         # Load projected columns from disk and join with search results.
         row_id_col_name = None
         res_row_list = [None for _ in range(self.limit_count.value)]
         for batch in self.children[0].exec(**kwargs):
             column_list = batch.columns
             if not row_id_col_name:
                 row_id_alias = get_row_id_column_alias(column_list)
                 row_id_col_name = "{}.{}".format(row_id_alias, IDENTIFIER_COLUMN)
 
             # Nested join.
             for _, row in batch.frames.iterrows():
-                for idx, rid in enumerate(row_id_list):
+                for idx, rid in enumerate(row_id_np):
                     if rid == row[row_id_col_name]:
                         res_row = dict()
                         for col_name in column_list:
                             res_row[col_name] = row[col_name]
                         res_row_list[idx] = res_row
 
         yield Batch(pd.DataFrame(res_row_list))
```

### Comparing `evadb-0.2.3.post0/eva/executor/function_scan_executor.py` & `evadb-0.2.4/eva/executor/function_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/groupby_executor.py` & `evadb-0.2.4/eva/executor/groupby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/hash_join_executor.py` & `evadb-0.2.4/eva/executor/hash_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/insert_executor.py` & `evadb-0.2.4/eva/executor/insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/join_build_executor.py` & `evadb-0.2.4/eva/executor/join_build_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/lateral_join_executor.py` & `evadb-0.2.4/eva/executor/lateral_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/limit_executor.py` & `evadb-0.2.4/eva/executor/limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/load_csv_executor.py` & `evadb-0.2.4/eva/executor/load_csv_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/load_executor.py` & `evadb-0.2.4/eva/executor/load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/load_multimedia_executor.py` & `evadb-0.2.4/eva/executor/load_multimedia_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                     for path, is_valid in zip(video_files, valid_bitmap)
                     if not is_valid
                 ]
 
                 invalid_files_str = "\n".join(invalid_files)
                 err_msg = f"Load {self.media_type.name} failed due to invalid files: \n{invalid_files_str}"
                 logger.error(err_msg)
-                raise ValueError("Load failed due to invalid files")
+                raise ValueError(err_msg)
 
             # Get valid files.
             valid_files = [
                 str(path)
                 for path, is_valid in zip(video_files, valid_bitmap)
                 if is_valid
             ]
```

### Comparing `evadb-0.2.3.post0/eva/executor/nested_loop_join_executor.py` & `evadb-0.2.4/eva/executor/nested_loop_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/orderby_executor.py` & `evadb-0.2.4/eva/executor/orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/plan_executor.py` & `evadb-0.2.4/eva/executor/plan_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from eva.executor.create_mat_view_executor import CreateMaterializedViewExecutor
 from eva.executor.create_udf_executor import CreateUDFExecutor
 from eva.executor.delete_executor import DeleteExecutor
 from eva.executor.drop_executor import DropExecutor
 from eva.executor.drop_udf_executor import DropUDFExecutor
 from eva.executor.executor_utils import ExecutorError
 from eva.executor.explain_executor import ExplainExecutor
-from eva.executor.faiss_index_scan_executor import FaissIndexScanExecutor
 from eva.executor.function_scan_executor import FunctionScanExecutor
 from eva.executor.groupby_executor import GroupByExecutor
 from eva.executor.hash_join_executor import HashJoinExecutor
 from eva.executor.insert_executor import InsertExecutor
 from eva.executor.join_build_executor import BuildJoinExecutor
 from eva.executor.lateral_join_executor import LateralJoinExecutor
 from eva.executor.limit_executor import LimitExecutor
@@ -41,14 +40,15 @@
 from eva.executor.project_executor import ProjectExecutor
 from eva.executor.rename_executor import RenameExecutor
 from eva.executor.sample_executor import SampleExecutor
 from eva.executor.seq_scan_executor import SequentialScanExecutor
 from eva.executor.show_info_executor import ShowInfoExecutor
 from eva.executor.storage_executor import StorageExecutor
 from eva.executor.union_executor import UnionExecutor
+from eva.executor.vector_index_scan_executor import VectorIndexScanExecutor
 from eva.experimental.ray.executor.exchange_executor import ExchangeExecutor
 from eva.models.storage.batch import Batch
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.plan_nodes.types import PlanOprType
 from eva.utils.logging_manager import logger
 
 
@@ -137,16 +137,16 @@
             executor_node = ShowInfoExecutor(node=plan)
         elif plan_opr_type == PlanOprType.EXPLAIN:
             executor_node = ExplainExecutor(node=plan)
         elif plan_opr_type == PlanOprType.CREATE_INDEX:
             executor_node = CreateIndexExecutor(node=plan)
         elif plan_opr_type == PlanOprType.APPLY_AND_MERGE:
             executor_node = ApplyAndMergeExecutor(node=plan)
-        elif plan_opr_type == PlanOprType.FAISS_INDEX_SCAN:
-            executor_node = FaissIndexScanExecutor(node=plan)
+        elif plan_opr_type == PlanOprType.VECTOR_INDEX_SCAN:
+            executor_node = VectorIndexScanExecutor(node=plan)
         elif plan_opr_type == PlanOprType.DELETE:
             executor_node = DeleteExecutor(node=plan)
 
         # EXPLAIN does not need to build execution tree for its children
         if plan_opr_type != PlanOprType.EXPLAIN:
             # Build Executor Tree for children
             for children in plan.children:
@@ -156,15 +156,15 @@
 
     def _clean_execution_tree(self, tree_root: AbstractExecutor):
         """clean the execution tree from memory
 
         Arguments:
             tree_root {AbstractExecutor} -- root of execution tree to delete
         """
-        # ToDo
+        # Todo
         # clear all the nodes from the execution tree
 
     def execute_plan(self) -> Iterator[Batch]:
         """execute the plan tree"""
         try:
             execution_tree = self._build_execution_tree(self._plan)
             output = execution_tree.exec()
```

### Comparing `evadb-0.2.3.post0/eva/executor/pp_executor.py` & `evadb-0.2.4/eva/executor/pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/predicate_executor.py` & `evadb-0.2.4/eva/executor/predicate_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/project_executor.py` & `evadb-0.2.4/eva/executor/project_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/rename_executor.py` & `evadb-0.2.4/eva/executor/rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/sample_executor.py` & `evadb-0.2.4/eva/executor/sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/seq_scan_executor.py` & `evadb-0.2.4/eva/executor/union_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,41 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
 from eva.executor.abstract_executor import AbstractExecutor
-from eva.executor.executor_utils import apply_predicate, apply_project
 from eva.models.storage.batch import Batch
-from eva.plan_nodes.seq_scan_plan import SeqScanPlan
+from eva.plan_nodes.union_plan import UnionPlan
 
 
-class SequentialScanExecutor(AbstractExecutor):
+class UnionExecutor(AbstractExecutor):
     """
-    Applies predicates to filter the frames which satisfy the condition
+    Merge the seq scan queries
     Arguments:
-        node (AbstractPlan): The SequentialScanPlan
+        node (AbstractPlan): The UnionPlan
 
     """
 
-    def __init__(self, node: SeqScanPlan):
+    def __init__(self, node: UnionPlan):
         super().__init__(node)
-        self.predicate = node.predicate
-        self.project_expr = node.columns
-        self.alias = node.alias
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
-        child_executor = self.children[0]
-        for batch in child_executor.exec(**kwargs):
-            # apply alias to the batch
-            # id, data -> myvideo.id, myvideo.data
-            if self.alias:
-                batch.modify_column_alias(self.alias)
-
-            # We do the predicate first
-            batch = apply_predicate(batch, self.predicate)
-            # Then do project
-            batch = apply_project(batch, self.project_expr)
+        assert self.node.all is True, "Only UNION ALL is supported now."
 
-            if not batch.empty():
+        # We should have only two children
+        for child in self.children:
+            for batch in child.exec():
                 yield batch
```

### Comparing `evadb-0.2.3.post0/eva/executor/show_info_executor.py` & `evadb-0.2.4/eva/executor/show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/storage_executor.py` & `evadb-0.2.4/eva/executor/storage_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/executor/union_executor.py` & `evadb-0.2.4/eva/readers/image/opencv_image_reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,32 +8,23 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Iterator
+from typing import Dict, Iterator
 
-from eva.executor.abstract_executor import AbstractExecutor
-from eva.models.storage.batch import Batch
-from eva.plan_nodes.union_plan import UnionPlan
+import cv2
 
+from eva.readers.abstract_reader import AbstractReader
 
-class UnionExecutor(AbstractExecutor):
-    """
-    Merge the seq scan queries
-    Arguments:
-        node (AbstractPlan): The UnionPlan
 
-    """
+class CVImageReader(AbstractReader):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-    def __init__(self, node: UnionPlan):
-        super().__init__(node)
-
-    def exec(self, *args, **kwargs) -> Iterator[Batch]:
-        assert self.node.all is True, "Only UNION ALL is supported now."
-
-        # We should have only two children
-        for child in self.children:
-            for batch in child.exec():
-                yield batch
+    def _read(self) -> Iterator[Dict]:
+        im_bgr = cv2.imread(str(self.file_url))
+        im_rgb = cv2.cvtColor(im_bgr, cv2.COLOR_BGR2RGB)
+        assert im_rgb is not None, f"Failed to read image file {self.file_url}"
+        yield {"data": im_rgb}
```

### Comparing `evadb-0.2.3.post0/eva/experimental/__init__.py` & `evadb-0.2.4/eva/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/__init__.py` & `evadb-0.2.4/eva/experimental/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/executor/__init__.py` & `evadb-0.2.4/eva/experimental/ray/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/executor/exchange_executor.py` & `evadb-0.2.4/eva/experimental/ray/executor/exchange_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 class QueueReaderExecutor(AbstractExecutor):
     def __init__(self):
         super().__init__(None)
 
     def exec(self, **kwargs) -> Iterator[Batch]:
         assert (
             "input_queues" in kwargs
-        ), "Invalid ray exectuion stage. No input_queue found"
+        ), "Invalid Ray execution stage. No input_queue found"
         input_queues = kwargs["input_queues"]
-        assert len(input_queues) == 1, "Not support mulitple input queues yet"
+        assert len(input_queues) == 1, "Not support multiple input queues yet"
         iq = input_queues[0]
 
         while True:
             next_item = iq.get(block=True)
             if next_item is StageCompleteSignal:
                 iq.put(StageCompleteSignal)
                 break
@@ -65,15 +65,15 @@
         super().__init__(node)
 
     def exec(self, is_top=True) -> Iterator[Batch]:
         assert (
             len(self.children) == 1
         ), "Exchange executor does not support children != 1"
 
-        # Find the exchange exector below the tree
+        # Find the exchange executor below the tree
         curr_exec = self
         input_queues = []
         while len(curr_exec.children) > 0 and not isinstance(
             curr_exec.children[0], ExchangeExecutor
         ):
             curr_exec = curr_exec.children[0]
```

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/executor/ray_stage.py` & `evadb-0.2.4/eva/experimental/ray/executor/ray_stage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/optimizer/__init__.py` & `evadb-0.2.4/eva/experimental/ray/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/__init__.py` & `evadb-0.2.4/eva/experimental/ray/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/optimizer/rules/rules.py` & `evadb-0.2.4/eva/experimental/ray/optimizer/rules/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     def check(self, before: LogicalGet, context: OptimizerContext):
         return True
 
     def apply(self, before: LogicalGet, context: OptimizerContext):
         # Configure the batch_mem_size. It decides the number of rows
         # read in a batch from storage engine.
-        # ToDO: Experiment heuristics.
+        # Todo: Experiment heuristics.
         scan = SeqScanPlan(None, before.target_list, before.alias)
         lower = ExchangePlan(parallelism=1)
         lower.append_child(
             StoragePlan(
                 before.table_obj,
                 before.video,
                 predicate=before.predicate,
```

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/planner/__init__.py` & `evadb-0.2.4/eva/experimental/ray/planner/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/experimental/ray/planner/exchange_plan.py` & `evadb-0.2.4/eva/experimental/ray/planner/exchange_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/expression/__init__.py` & `evadb-0.2.4/eva/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/expression/abstract_expression.py` & `evadb-0.2.4/eva/expression/abstract_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         assert index >= 0 and index < len(self._children)
         return self._children[index]
 
     @property
     def children(self):
         return self._children
 
+    @children.setter
+    def children(self, children):
+        self._children = children
+
     def append_child(self, child):
         self._children.append(child)
 
     def get_children_count(self) -> int:
         return len(self._children)
 
     @property
@@ -176,20 +180,20 @@
         Returns:
             the generator object.
         """
         yield self
         for child in self.children:
             yield from child.dfs()
 
-    def find_all(self, expresison_type: Any):
-        """Returns a generator which visits all the nodes in expresison tree and yields one that matches the passed `expression_type`.
+    def find_all(self, expression_type: Any):
+        """Returns a generator which visits all the nodes in expression tree and yields one that matches the passed `expression_type`.
 
         Args:
-            expresison_type (Any): expression type to match with
+            expression_type (Any): expression type to match with
 
         Returns:
             the generator object.
         """
 
         for node in self.bfs():
-            if isinstance(node, expresison_type):
+            if isinstance(node, expression_type):
                 yield node
```

### Comparing `evadb-0.2.3.post0/eva/expression/aggregation_expression.py` & `evadb-0.2.4/eva/expression/aggregation_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/expression/arithmetic_expression.py` & `evadb-0.2.4/eva/expression/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/expression/comparison_expression.py` & `evadb-0.2.4/eva/expression/comparison_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/expression/constant_value_expression.py` & `evadb-0.2.4/eva/expression/constant_value_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from eva.catalog.catalog_type import ColumnType
 from eva.expression.abstract_expression import AbstractExpression, ExpressionType
 from eva.models.storage.batch import Batch
 
 
 class ConstantValueExpression(AbstractExpression):
-    # ToDo Implement generic value class
+    # Todo Implement generic value class
     # for now we don't assign any class to value
     # it can have types like string, int etc
     # return type not set, handle that based on value
     def __init__(self, value: Any, v_type: ColumnType = ColumnType.INTEGER):
         super().__init__(ExpressionType.CONSTANT_VALUE)
         self._value = value
         self._v_type = v_type
@@ -43,15 +43,15 @@
     def value(self):
         return self._value
 
     @property
     def v_type(self):
         return self._v_type
 
-    # ToDo implement other functionalities like maintaining hash
+    # Todo implement other functionalities like maintaining hash
     # comparing two objects of this class(==)
 
     def __eq__(self, other):
         is_subtree_equal = super().__eq__(other)
         if not isinstance(other, ConstantValueExpression):
             return False
         # if the value type is NDARRAY, we need to reduce the
```

### Comparing `evadb-0.2.3.post0/eva/expression/expression_utils.py` & `evadb-0.2.4/eva/expression/expression_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from eva.expression.logical_expression import LogicalExpression
 from eva.expression.tuple_value_expression import TupleValueExpression
 
 
 def to_conjunction_list(
     expression_tree: AbstractExpression,
 ) -> List[AbstractExpression]:
-    """Convert expression tree to list of conjuntives
+    """Convert expression tree to list of conjunctives
 
     Note: It does not normalize the expression tree before extracting the conjunctives.
 
     Args:
         expression_tree (AbstractExpression): expression tree to transform
 
     Returns:
@@ -49,15 +49,15 @@
 
     return expression_list
 
 
 def conjunction_list_to_expression_tree(
     expression_list: List[AbstractExpression],
 ) -> AbstractExpression:
-    """Convert expression list to expression tree using conjuction connector
+    """Convert expression list to expression tree using conjunction connector
 
     [a, b, c] -> AND( AND(a, b), c)
     Args:
         expression_list (List[AbstractExpression]): list of conjunctives
 
     Returns:
         AbstractExpression: expression tree
@@ -95,15 +95,15 @@
         RuntimeError: Invalid expression
 
     Example:
         extract_range_from_comparison_expr(id < 10, 0, inf): True, [(0,9)]
     """
 
     if not isinstance(expr, ComparisonExpression):
-        raise RuntimeError(f"Expected Comparision Expression, got {type(expr)}")
+        raise RuntimeError(f"Expected Comparison Expression, got {type(expr)}")
     left = expr.children[0]
     right = expr.children[1]
     expr_type = expr.etype
     val = None
     const_first = False
     if isinstance(left, TupleValueExpression) and isinstance(
         right, ConstantValueExpression
@@ -112,15 +112,15 @@
     elif isinstance(left, ConstantValueExpression) and isinstance(
         right, TupleValueExpression
     ):
         val = left.value
         const_first = True
     else:
         raise RuntimeError(
-            f"Only supports extracting range from Comparision Expression \
+            f"Only supports extracting range from Comparison Expression \
                 with two children TupleValueExpression and \
                 ConstantValueExpression, got {left} and {right}"
         )
 
     if const_first:
         if expr_type is ExpressionType.COMPARE_GREATER:
             expr_type = ExpressionType.COMPARE_LESSER
@@ -153,16 +153,15 @@
 def extract_range_list_from_predicate(
     predicate: AbstractExpression, lower_bound: int, upper_bound: int
 ) -> List:
     """The function converts the range predicate on the column in the
         `predicate` to a list of [(start_1, end_1), ... ] pairs.
 
         It assumes the predicate contains conditions on only one column.
-        It is the responsibilty of the caller that `predicate` does not contains
-        conditions on multiple columns.
+        It is the responsibility of the caller that `predicate` does not contains conditions on multiple columns.
 
     Args:
         predicate (AbstractExpression): Input predicate to extract
             valid ranges. The predicate should contain conditions on
             only one columns, else it raise error.
         lower_bound (int): lower bound of the comparison predicate
         upper_bound (int): upper bound of the comparison predicate
@@ -276,15 +275,15 @@
         only contains LogicalExpression, ComparisonExpression,
         TupleValueExpression or ConstantValueExpression
 
     Args:
         predicate (AbstractExpression): predicate expression to check
 
     Returns:
-        bool: True, if it is a simple predicate, lese False
+        bool: True, if it is a simple predicate, else False
     """
 
     def _has_simple_expressions(expr):
         simple = type(expr) in simple_expressions
         for child in expr.children:
             simple = simple and _has_simple_expressions(child)
         return simple
```

### Comparing `evadb-0.2.3.post0/eva/expression/function_expression.py` & `evadb-0.2.4/eva/expression/function_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from eva.utils.stats import UDFStats
 
 
 class FunctionExpression(AbstractExpression):
     """
     Consider FunctionExpression: ObjDetector -> (labels, boxes)
 
-    `output`: If the user wants only subset of ouputs. Eg,
-    ObjDetector.lables the parser with set output to 'labels'
+    `output`: If the user wants only subset of outputs. Eg,
+    ObjDetector.labels the parser with set output to 'labels'
 
     `output_objs`: It is populated by the binder. In case the
     output is None, the binder sets output_objs to list of all
     output columns of the FunctionExpression. Eg, ['labels',
     'boxes']. Otherwise, only the output columns.
 
     FunctionExpression also needs to prepend its alias to all the
```

### Comparing `evadb-0.2.3.post0/eva/expression/logical_expression.py` & `evadb-0.2.4/eva/expression/logical_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/expression/tuple_value_expression.py` & `evadb-0.2.4/eva/expression/tuple_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/__init__.py` & `evadb-0.2.4/eva/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/catalog/__init__.py` & `evadb-0.2.4/eva/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/catalog/frame_info.py` & `evadb-0.2.4/eva/models/catalog/frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/catalog/properties.py` & `evadb-0.2.4/eva/models/catalog/properties.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/server/__init__.py` & `evadb-0.2.4/eva/models/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/server/response.py` & `evadb-0.2.4/eva/models/server/response.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/storage/__init__.py` & `evadb-0.2.4/eva/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/models/storage/batch.py` & `evadb-0.2.4/eva/models/storage/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             return
         if by is None:
             by = self.columns[0]
         self._frames.sort_values(by=by, ignore_index=True, inplace=True)
 
     def sort_orderby(self, by, sort_type=None) -> None:
         """
-        in_place sort for orderby
+        in_place sort for order_by
 
         Args:
             by: list of column names
             sort_type: list of True/False if ASC for each column name in 'by'
                 i.e [True, False] means [ASC, DESC]
         """
 
@@ -235,25 +235,25 @@
 
     def project(self, cols: None) -> Batch:
         """
         Takes as input the column list, returns the projection.
         We do a copy for now.
         """
         cols = cols or []
-        verfied_cols = [c for c in cols if c in self._frames]
-        unknown_cols = list(set(cols) - set(verfied_cols))
+        verified_cols = [c for c in cols if c in self._frames]
+        unknown_cols = list(set(cols) - set(verified_cols))
         assert len(unknown_cols) == 0, unknown_cols
-        return Batch(self._frames[verfied_cols])
+        return Batch(self._frames[verified_cols])
 
     @classmethod
     def merge_column_wise(cls, batches: List[Batch], auto_renaming=False) -> Batch:
         """
         Merge list of batch frames column_wise and return a new batch frame
         Arguments:
-            batches: List[Batch]: lsit of batch objects to be merged
+            batches: List[Batch]: list of batch objects to be merged
             auto_renaming: if true rename column names if required
 
         Returns:
             Batch: Merged batch object
         """
         if not len(batches):
             return Batch()
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/__init__.py` & `evadb-0.2.4/eva/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/binder.py` & `evadb-0.2.4/eva/optimizer/binder.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
             if len(pattern.children) != len(expr.children):
                 return
 
             for child_grp, pattern_child in zip(expr.children, pattern.children):
                 child_binders.append(Binder._grp_binder(child_grp, pattern_child, memo))
         else:
-            # record the group id in a Dummy Opearator
+            # record the group id in a Dummy Operator
             curr_iterator = iter([Dummy(expr.group_id, expr.opr)])
 
         yield from itertools.product(curr_iterator, *child_binders)
 
     @staticmethod
     def build_opr_tree_from_pre_order_repr(pre_order_repr: tuple) -> Operator:
         opr_tree = pre_order_repr[0]
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/cost_model.py` & `evadb-0.2.4/eva/optimizer/cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/group.py` & `evadb-0.2.4/eva/optimizer/group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/group_expression.py` & `evadb-0.2.4/eva/optimizer/group_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/memo.py` & `evadb-0.2.4/eva/optimizer/memo.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         new_group_id = len(self._groups)
         aliases = self._get_table_aliases(expr)
         self._groups[new_group_id] = Group(new_group_id, aliases)
         self._insert_expr(expr, new_group_id)
 
     def _insert_expr(self, expr: GroupExpression, group_id: int):
         """
-        Insert a group expressoin into a particular group
+        Insert a group expression into a particular group
         """
         assert group_id < len(self.groups), "Group Id out of the bound"
 
         group = self.groups[group_id]
         group.add_expr(expr)
         self._group_exprs[hash(expr)] = expr
 
@@ -114,15 +114,15 @@
         Otherwise, inserts the expr into specified group.
         """
         # check duplicate expression
         duplicate_expr = self.find_duplicate_expr(expr)
         if duplicate_expr is not None:
             return duplicate_expr
 
-        # did not find a dulpicate expression
+        # did not find a duplicate expression
         expr.group_id = group_id
 
         if expr.group_id == UNDEFINED_GROUP_ID:
             self._create_new_group(expr)
         else:
             self._insert_expr(expr, group_id)
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/operators.py` & `evadb-0.2.4/eva/optimizer/operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import deque
 from enum import IntEnum, auto
 from pathlib import Path
 from typing import Any, List
 
-from eva.catalog.catalog_type import IndexType
+from eva.catalog.catalog_type import VectorStoreType
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
 from eva.catalog.models.table_catalog import TableCatalogEntry
 from eva.catalog.models.udf_io_catalog import UdfIOCatalogEntry
 from eva.catalog.models.udf_metadata_catalog import UdfMetadataCatalogEntry
 from eva.expression.abstract_expression import AbstractExpression
 from eva.expression.constant_value_expression import ConstantValueExpression
 from eva.expression.function_expression import FunctionExpression
@@ -58,20 +58,21 @@
     LOGICALFUNCTIONSCAN = auto()
     LOGICAL_CREATE_MATERIALIZED_VIEW = auto()
     LOGICAL_SHOW = auto()
     LOGICALDROPUDF = auto()
     LOGICALEXPLAIN = auto()
     LOGICALCREATEINDEX = auto()
     LOGICAL_APPLY_AND_MERGE = auto()
-    LOGICALFAISSINDEXSCAN = auto()
+    LOGICAL_EXTRACT_OBJECT = auto()
+    LOGICAL_VECTOR_INDEX_SCAN = auto()
     LOGICALDELIMITER = auto()
 
 
 class Operator:
-    """Base class for logital plan of operators
+    """Base class for logical plan of operators
     Arguments:
         op_type: {OperatorType} -- {the opr type held by this node}
         children: {List} -- {the list of operator children for this node}
     """
 
     def __init__(self, op_type: OperatorType, children=None):
         self._opr_type = op_type
@@ -914,14 +915,53 @@
             and self.alias == other.alias
         )
 
     def __hash__(self) -> int:
         return hash((super().__hash__(), self.func_expr, self.do_unnest, self.alias))
 
 
+class LogicalExtractObject(Operator):
+    def __init__(
+        self,
+        detector: FunctionExpression,
+        tracker: FunctionExpression,
+        alias: Alias,
+        do_unnest: bool = False,
+        children: List = None,
+    ):
+        super().__init__(OperatorType.LOGICAL_EXTRACT_OBJECT, children)
+        self.detector = detector
+        self.tracker = tracker
+        self.do_unnest = do_unnest
+        self.alias = alias
+
+    def __eq__(self, other):
+        is_subtree_equal = super().__eq__(other)
+        if not isinstance(other, LogicalExtractObject):
+            return False
+        return (
+            is_subtree_equal
+            and self.detector == other.detector
+            and self.tracker == other.tracker
+            and self.do_unnest == other.do_unnest
+            and self.alias == other.alias
+        )
+
+    def __hash__(self) -> int:
+        return hash(
+            (
+                super().__hash__(),
+                self.detector,
+                self.tracker,
+                self.do_unnest,
+                self.alias,
+            )
+        )
+
+
 class LogicalJoin(Operator):
     """
     Logical node for join operators
 
     Attributes:
         join_type: JoinType
             Join type provided by the user - Lateral, Inner, Outer
@@ -993,15 +1033,15 @@
                 self.right_keys,
                 tuple(self.join_project or []),
             )
         )
 
 
 class LogicalCreateMaterializedView(Operator):
-    """Logical node for create materiaziled view operations
+    """Logical node for create materialized view operations
     Arguments:
         view {TableRef}: [view table that is to be created]
         col_list{List[ColumnDefinition]} -- column names in the view
         if_not_exists {bool}: [whether to override if view exists]
     """
 
     def __init__(
@@ -1102,23 +1142,23 @@
 
 class LogicalCreateIndex(Operator):
     def __init__(
         self,
         name: str,
         table_ref: TableRef,
         col_list: List[ColumnDefinition],
-        index_type: IndexType,
+        vector_store_type: VectorStoreType,
         udf_func: FunctionExpression = None,
         children: List = None,
     ):
         super().__init__(OperatorType.LOGICALCREATEINDEX, children)
         self._name = name
         self._table_ref = table_ref
         self._col_list = col_list
-        self._index_type = index_type
+        self._vector_store_type = vector_store_type
         self._udf_func = udf_func
 
     @property
     def name(self):
         return self._name
 
     @property
@@ -1126,42 +1166,42 @@
         return self._table_ref
 
     @property
     def col_list(self):
         return self._col_list
 
     @property
-    def index_type(self):
-        return self._index_type
+    def vector_store_type(self):
+        return self._vector_store_type
 
     @property
     def udf_func(self):
         return self._udf_func
 
     def __eq__(self, other):
         is_subtree_equal = super().__eq__(other)
         if not isinstance(other, LogicalCreateIndex):
             return False
         return (
             is_subtree_equal
             and self.name == other.name
             and self.table_ref == other.table_ref
             and self.col_list == other.col_list
-            and self.index_type == other.index_type
+            and self.vector_store_type == other.vector_store_type
             and self.udf_func == other.udf_func
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 super().__hash__(),
                 self.name,
                 self.table_ref,
                 tuple(self.col_list),
-                self.index_type,
+                self.vector_store_type,
                 self.udf_func,
             )
         )
 
 
 class LogicalApplyAndMerge(Operator):
     """Evaluate the function expression on the input data and return the merged output.
@@ -1217,52 +1257,60 @@
                 self.do_unnest,
                 self.alias,
                 self._merge_type,
             )
         )
 
 
-class LogicalFaissIndexScan(Operator):
+class LogicalVectorIndexScan(Operator):
     def __init__(
         self,
         index_name: str,
+        vector_store_type: VectorStoreType,
         limit_count: ConstantValueExpression,
         search_query_expr: FunctionExpression,
         children: List = None,
     ):
-        super().__init__(OperatorType.LOGICALFAISSINDEXSCAN, children)
+        super().__init__(OperatorType.LOGICAL_VECTOR_INDEX_SCAN, children)
         self._index_name = index_name
+        self._vector_store_type = vector_store_type
         self._limit_count = limit_count
         self._search_query_expr = search_query_expr
 
     @property
     def index_name(self):
         return self._index_name
 
     @property
+    def vector_store_type(self):
+        return self._vector_store_type
+
+    @property
     def limit_count(self):
         return self._limit_count
 
     @property
     def search_query_expr(self):
         return self._search_query_expr
 
     def __eq__(self, other):
         is_subtree_equal = super().__eq__(other)
-        if not isinstance(other, LogicalFaissIndexScan):
+        if not isinstance(other, LogicalVectorIndexScan):
             return False
         return (
             is_subtree_equal
             and self.index_name == other.index_name
+            and self.vector_store_type == other.vector_store_type
             and self.limit_count == other.limit_count
             and self.search_query_expr == other.search_query_expr
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 super().__hash__(),
                 self.index_name,
+                self.vector_store_type,
                 self.limit_count,
                 self.search_query_expr,
             )
         )
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/optimizer_context.py` & `evadb-0.2.4/eva/optimizer/optimizer_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,12 +93,12 @@
         self.memo.erase_group(group_id)
         new_expr = self._xform_opr_to_group_expr(opr)
         new_expr = self.memo.add_group_expr(new_expr, group_id)
         return new_expr
 
     def add_opr_to_group(self, opr: Operator, group_id: int = UNDEFINED_GROUP_ID):
         """
-        Convert opertator to group_expression and add to the group
+        Convert operator to group_expression and add to the group
         """
         grp_expr = self._xform_opr_to_group_expr(opr)
         grp_expr = self.memo.add_group_expr(grp_expr, group_id)
         return grp_expr
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/optimizer_task_stack.py` & `evadb-0.2.4/eva/optimizer/optimizer_task_stack.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/optimizer_tasks.py` & `evadb-0.2.4/eva/optimizer/optimizer_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             for match in iter(binder):
                 if not rule.check(match, self.optimizer_context):
                     continue
                 after = rule.apply(match, self.optimizer_context)
                 plans = list(after)
                 assert (
                     len(plans) <= 1
-                ), "Rewrite rule cannot generate more than oen alternate plan."
+                ), "Rewrite rule cannot generate more than open alternate plan."
                 for plan in plans:
                     new_expr = self.optimizer_context.replace_expression(
                         plan, self.root_expr.group_id
                     )
                     self.optimizer_context.task_stack.push(
                         TopDownRewrite(new_expr, self.rule_set, self.optimizer_context)
                     )
@@ -150,20 +150,20 @@
                 logger.info(
                     "In BottomUp, Rule {} matched for {}".format(rule, self.root_expr)
                 )
                 after = rule.apply(match, self.optimizer_context)
                 plans = list(after)
                 assert (
                     len(plans) <= 1
-                ), "Rewrite rule cannot generate more than oen alternate plan."
+                ), "Rewrite rule cannot generate more than open alternate plan."
                 for plan in plans:
                     new_expr = self.optimizer_context.replace_expression(
                         plan, self.root_expr.group_id
                     )
-                    logger.info("After rewiting {}".format(self.root_expr))
+                    logger.info("After rewriting {}".format(self.root_expr))
                     self.optimizer_context.task_stack.push(
                         BottomUpRewrite(new_expr, self.rule_set, self.optimizer_context)
                     )
                     # The root has changed so we cannot apply more rules to the same
                     # root, hence return
                     return
             self.root_expr.mark_rule_explored(rule.rule_type)
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/optimizer_utils.py` & `evadb-0.2.4/eva/optimizer/optimizer_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.alias import Alias
 from eva.parser.create_statement import ColumnDefinition
 from eva.utils.kv_cache import DiskKVCache
 
 
 def column_definition_to_udf_io(col_list: List[ColumnDefinition], is_input: bool):
-    """Create the UdfIOCatalogEntry object fro each column definition provided
+    """Create the UdfIOCatalogEntry object for each column definition provided
 
     Arguments:
         col_list(List[ColumnDefinition]): parsed input/output definitions
         is_input(bool): true if input else false
     """
     if isinstance(col_list, ColumnDefinition):
         col_list = [col_list]
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/plan_generator.py` & `evadb-0.2.4/eva/optimizer/plan_generator.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/property.py` & `evadb-0.2.4/eva/optimizer/property.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/rules/__init__.py` & `evadb-0.2.4/eva/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/optimizer/rules/pattern.py` & `evadb-0.2.4/eva/optimizer/rules/pattern.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 from eva.optimizer.operators import OperatorType
 
 
 class Pattern:
     def __init__(self, opr_type: OperatorType):
         self._opr_type = opr_type
-        self._chilren = []
+        self._children = []
 
     def append_child(self, child: Pattern):
-        self._chilren.append(child)
+        self._children.append(child)
 
     @property
     def children(self):
-        return self._chilren
+        return self._children
 
     @property
     def opr_type(self):
         return self._opr_type
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/rules/rules.py` & `evadb-0.2.4/eva/optimizer/rules/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     LogicalCreateIndex,
     LogicalCreateMaterializedView,
     LogicalCreateUDF,
     LogicalDelete,
     LogicalDrop,
     LogicalDropUDF,
     LogicalExplain,
-    LogicalFaissIndexScan,
+    LogicalExtractObject,
     LogicalFilter,
     LogicalFunctionScan,
     LogicalGet,
     LogicalGroupBy,
     LogicalInsert,
     LogicalJoin,
     LogicalLimit,
@@ -73,36 +73,37 @@
     LogicalOrderBy,
     LogicalProject,
     LogicalQueryDerivedGet,
     LogicalRename,
     LogicalSample,
     LogicalShow,
     LogicalUnion,
+    LogicalVectorIndexScan,
     Operator,
     OperatorType,
 )
 from eva.plan_nodes.create_index_plan import CreateIndexPlan
 from eva.plan_nodes.create_plan import CreatePlan
 from eva.plan_nodes.create_udf_plan import CreateUDFPlan
 from eva.plan_nodes.delete_plan import DeletePlan
 from eva.plan_nodes.drop_plan import DropPlan
 from eva.plan_nodes.drop_udf_plan import DropUDFPlan
-from eva.plan_nodes.faiss_index_scan_plan import FaissIndexScanPlan
 from eva.plan_nodes.function_scan_plan import FunctionScanPlan
 from eva.plan_nodes.groupby_plan import GroupByPlan
 from eva.plan_nodes.hash_join_probe_plan import HashJoinProbePlan
 from eva.plan_nodes.insert_plan import InsertPlan
 from eva.plan_nodes.lateral_join_plan import LateralJoinPlan
 from eva.plan_nodes.limit_plan import LimitPlan
 from eva.plan_nodes.load_data_plan import LoadDataPlan
 from eva.plan_nodes.orderby_plan import OrderByPlan
 from eva.plan_nodes.rename_plan import RenamePlan
 from eva.plan_nodes.seq_scan_plan import SeqScanPlan
 from eva.plan_nodes.storage_plan import StoragePlan
 from eva.plan_nodes.union_plan import UnionPlan
+from eva.plan_nodes.vector_index_scan_plan import VectorIndexScanPlan
 
 ##############################################
 # REWRITE RULES START
 
 
 class EmbedFilterIntoGet(Rule):
     def __init__(self):
@@ -236,15 +237,15 @@
 
         if len(valid_exprs) > 0:
             return True
         return False
 
     def apply(self, before: LogicalFilter, context: OptimizerContext):
         # there could be 2^n different combinations with enable and disable option
-        # cache for n functionExpressions. Currently considering only the case where
+        # cache for n function Expressions. Currently considering only the case where
         # cache is enabled for all eligible function expressions
         after_predicate = before.predicate.copy()
         enable_cache_on_expression_tree(after_predicate)
         after_operator = LogicalFilter(
             predicate=after_predicate, children=before.children
         )
         yield after_operator
@@ -269,15 +270,15 @@
         if len(expr.children) > 1 or not isinstance(
             expr.children[0], TupleValueExpression
         ):
             return False
         return True
 
     def apply(self, before: LogicalApplyAndMerge, context: OptimizerContext):
-        # todo: this will create a ctaalog entry even in the case of explain command
+        # todo: this will create a catalog entry even in the case of explain command
         # We should run this code conditionally
         new_func_expr = enable_cache(before.func_expr)
         after = LogicalApplyAndMerge(
             func_expr=new_func_expr, alias=before.alias, do_unnest=before.do_unnest
         )
         after.append_child(before.children[0])
         yield after
@@ -342,15 +343,15 @@
 
         yield new_join_node
 
 
 class XformLateralJoinToLinearFlow(Rule):
     """If the inner node of a lateral join is a function-valued expression, we
     eliminate the join node and make the inner node the parent of the outer node. This
-    produces a linear #data flow path. Because this scenario is common in our system,
+    produces a linear data flow path. Because this scenario is common in our system,
     we chose to explicitly convert it to a linear flow, which simplifies the
     implementation of other optimizations such as UDF reuse and parallelized plans by
     removing the join."""
 
     def __init__(self):
         pattern = Pattern(OperatorType.LOGICALJOIN)
         pattern.append_child(Pattern(OperatorType.DUMMY))
@@ -438,18 +439,62 @@
         if rem_pred:
             root_node = LogicalFilter(predicate=rem_pred)
             root_node.append_child(apply_and_merge)
 
         yield root_node
 
 
-class CombineSimilarityOrderByAndLimitToFaissIndexScan(Rule):
+class XformExtractObjectToLinearFlow(Rule):
+    """If the inner node of a lateral join is a Extract_Object function-valued
+    expression, we eliminate the join node and make the inner node the parent of the
+    outer node. This produces a linear data flow path.
+    TODO: We need to add a sorting operation after detector to ensure we always provide tracker data in order.
     """
-    This rule currently rewrites Order By + Limit to a Faiss index scan.
-    Because Faiss index only works for similarity search, the rule will
+
+    #                                          LogicalApplyAndMerge(tracker)
+    #     LogicalJoin(Lateral)                         |
+    #     /           \                 ->    LogicalApplyAndMerge(detector)
+    #    A        LogicalExtractObject                 |
+    #                                                  A
+
+    def __init__(self):
+        pattern = Pattern(OperatorType.LOGICALJOIN)
+        pattern.append_child(Pattern(OperatorType.DUMMY))
+        pattern.append_child(Pattern(OperatorType.LOGICAL_EXTRACT_OBJECT))
+        super().__init__(RuleType.XFORM_EXTRACT_OBJECT_TO_LINEAR_FLOW, pattern)
+
+    def promise(self):
+        return Promise.XFORM_EXTRACT_OBJECT_TO_LINEAR_FLOW
+
+    def check(self, before: LogicalJoin, context: OptimizerContext):
+        if before.join_type == JoinType.LATERAL_JOIN:
+            return True
+        return False
+
+    def apply(self, before: LogicalJoin, context: OptimizerContext):
+        A: Dummy = before.children[0]
+        logical_extract_obj: LogicalExtractObject = before.children[1]
+
+        detector = LogicalApplyAndMerge(
+            logical_extract_obj.detector, alias=logical_extract_obj.detector.alias
+        )
+        tracker = LogicalApplyAndMerge(
+            logical_extract_obj.tracker,
+            alias=logical_extract_obj.alias,
+            do_unnest=logical_extract_obj.do_unnest,
+        )
+        detector.append_child(A)
+        tracker.append_child(detector)
+        yield tracker
+
+
+class CombineSimilarityOrderByAndLimitToVectorIndexScan(Rule):
+    """
+    This rule currently rewrites Order By + Limit to a vector index scan.
+    Because vector index only works for similarity search, the rule will
     only be applied when the Order By is on Similarity expression. For
     simplicity, we also only enable this rule when the Similarity expression
     applies to the full table. Predicated query will yield incorrect results
     if we use an index scan.
 
     Limit(10)
         |
@@ -460,23 +505,23 @@
 
     def __init__(self):
         pattern = Pattern(OperatorType.LOGICALLIMIT)
         orderby_pattern = Pattern(OperatorType.LOGICALORDERBY)
         orderby_pattern.append_child(Pattern(OperatorType.DUMMY))
         pattern.append_child(orderby_pattern)
         super().__init__(
-            RuleType.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN, pattern
+            RuleType.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_VECTOR_INDEX_SCAN, pattern
         )
 
-        # Entries populate after rule egibility validation.
+        # Entries populate after rule eligibility validation.
         self._index_catalog_entry = None
         self._query_func_expr = None
 
     def promise(self):
-        return Promise.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN
+        return Promise.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_VECTOR_INDEX_SCAN
 
     def check(self, before: LogicalLimit, context: OptimizerContext):
         return True
 
     def apply(self, before: LogicalLimit, context: OptimizerContext):
         catalog_manager = CatalogManager()
 
@@ -529,23 +574,24 @@
             catalog_manager.get_index_catalog_entry_by_column_and_udf_signature(
                 column_catalog_entry, udf_signature
             )
         )
         if not index_catalog_entry:
             return
 
-        # Construct the Faiss index scan plan.
-        faiss_index_scan_node = LogicalFaissIndexScan(
+        # Construct the Vector index scan plan.
+        vector_index_scan_node = LogicalVectorIndexScan(
             index_catalog_entry.name,
+            index_catalog_entry.type,
             limit_node.limit_count,
             query_func_expr,
         )
         for child in orderby_node.children:
-            faiss_index_scan_node.append_child(child)
-        yield faiss_index_scan_node
+            vector_index_scan_node.append_child(child)
+        yield vector_index_scan_node
 
 
 # REWRITE RULES END
 ##############################################
 
 ##############################################
 # LOGICAL RULES START
@@ -590,15 +636,15 @@
         pattern.append_child(Pattern(OperatorType.DUMMY))
         super().__init__(RuleType.REORDER_PREDICATES, pattern)
 
     def promise(self):
         return Promise.REORDER_PREDICATES
 
     def check(self, before: LogicalFilter, context: OptimizerContext):
-        # there exists atleast one Function Expression
+        # there exists at least one Function Expression
         return len(list(before.predicate.find_all(FunctionExpression))) > 0
 
     def apply(self, before: LogicalFilter, context: OptimizerContext):
         # Decompose the expression tree into a list of conjuncts
         conjuncts = to_conjunction_list(before.predicate)
 
         # Segregate the conjuncts into simple and function expressions
@@ -710,31 +756,31 @@
             before.impl_path,
             before.udf_type,
             before.metadata,
         )
         yield after
 
 
-class LogicalCreateIndexToFaiss(Rule):
+class LogicalCreateIndexToVectorIndex(Rule):
     def __init__(self):
         pattern = Pattern(OperatorType.LOGICALCREATEINDEX)
-        super().__init__(RuleType.LOGICAL_CREATE_INDEX_TO_FAISS, pattern)
+        super().__init__(RuleType.LOGICAL_CREATE_INDEX_TO_VECTOR_INDEX, pattern)
 
     def promise(self):
-        return Promise.LOGICAL_CREATE_INDEX_TO_FAISS
+        return Promise.LOGICAL_CREATE_INDEX_TO_VECTOR_INDEX
 
     def check(self, before: Operator, context: OptimizerContext):
         return True
 
     def apply(self, before: LogicalCreateIndex, context: OptimizerContext):
         after = CreateIndexPlan(
             before.name,
             before.table_ref,
             before.col_list,
-            before.index_type,
+            before.vector_store_type,
             before.udf_func,
         )
         yield after
 
 
 class LogicalDropUDFToPhysical(Rule):
     def __init__(self):
@@ -815,15 +861,15 @@
 
     def check(self, before: Operator, context: OptimizerContext):
         return True
 
     def apply(self, before: LogicalGet, context: OptimizerContext):
         # Configure the batch_mem_size. It decides the number of rows
         # read in a batch from storage engine.
-        # ToDO: Experiment heuristics.
+        # Todo: Experiment heuristics.
         after = SeqScanPlan(None, before.target_list, before.alias)
         after.append_child(
             StoragePlan(
                 before.table_obj,
                 before.video,
                 predicate=before.predicate,
                 sampling_rate=before.sampling_rate,
@@ -1166,29 +1212,32 @@
     def apply(self, before: LogicalApplyAndMerge, context: OptimizerContext):
         after = ApplyAndMergePlan(before.func_expr, before.alias, before.do_unnest)
         for child in before.children:
             after.append_child(child)
         yield after
 
 
-class LogicalFaissIndexScanToPhysical(Rule):
+class LogicalVectorIndexScanToPhysical(Rule):
     def __init__(self):
-        pattern = Pattern(OperatorType.LOGICALFAISSINDEXSCAN)
+        pattern = Pattern(OperatorType.LOGICAL_VECTOR_INDEX_SCAN)
         pattern.append_child(Pattern(OperatorType.DUMMY))
-        super().__init__(RuleType.LOGICAL_FAISS_INDEX_SCAN_TO_PHYSICAL, pattern)
+        super().__init__(RuleType.LOGICAL_VECTOR_INDEX_SCAN_TO_PHYSICAL, pattern)
 
     def promise(self):
-        return Promise.LOGICAL_FAISS_INDEX_SCAN_TO_PHYSICAL
+        return Promise.LOGICAL_VECTOR_INDEX_SCAN_TO_PHYSICAL
 
     def check(self, grp_id: int, context: OptimizerContext):
         return True
 
-    def apply(self, before: LogicalFaissIndexScan, context: OptimizerContext):
-        after = FaissIndexScanPlan(
-            before.index_name, before.limit_count, before.search_query_expr
+    def apply(self, before: LogicalVectorIndexScan, context: OptimizerContext):
+        after = VectorIndexScanPlan(
+            before.index_name,
+            before.vector_store_type,
+            before.limit_count,
+            before.search_query_expr,
         )
         for child in before.children:
             after.append_child(child)
         yield after
 
 
 # IMPLEMENTATION RULES END
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/rules/rules_base.py` & `evadb-0.2.4/eva/optimizer/rules/rules_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,32 +30,33 @@
     """
 
     # Don't move this enum, else will break rule exploration logic
     INVALID_RULE = 0
 
     # REWRITE RULES TOP DOWN APPLY FIRST (LOGICAL -> LOGICAL)
     XFORM_LATERAL_JOIN_TO_LINEAR_FLOW = auto()
-    TOP_DOWN_DELIMETER = auto()
+    XFORM_EXTRACT_OBJECT_TO_LINEAR_FLOW = auto()
+    TOP_DOWN_DELIMITER = auto()
 
     # REWRITE RULES BOTTOM UP APPLY SECOND (LOGICAL -> LOGICAL)
     EMBED_FILTER_INTO_GET = auto()
     EMBED_SAMPLE_INTO_GET = auto()
     PUSHDOWN_FILTER_THROUGH_JOIN = auto()
     PUSHDOWN_FILTER_THROUGH_APPLY_AND_MERGE = auto()
-    COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN = auto()
+    COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_VECTOR_INDEX_SCAN = auto()
     REORDER_PREDICATES = auto()
 
-    REWRITE_DELIMETER = auto()
+    REWRITE_DELIMITER = auto()
 
     # TRANSFORMATION RULES (LOGICAL -> LOGICAL)
     LOGICAL_INNER_JOIN_COMMUTATIVITY = auto()
     CACHE_FUNCTION_EXPRESISON_IN_APPLY = auto()
     CACHE_FUNCTION_EXPRESISON_IN_FILTER = auto()
     CACHE_FUNCTION_EXPRESISON_IN_PROJECT = auto()
-    TRANSFORMATION_DELIMETER = auto()  # do not reposition
+    TRANSFORMATION_DELIMITER = auto()  # do not reposition
 
     # IMPLEMENTATION RULES (LOGICAL -> PHYSICAL)
     LOGICAL_EXCHANGE_TO_PHYSICAL = auto()
     LOGICAL_UNION_TO_PHYSICAL = auto()
     LOGICAL_GROUPBY_TO_PHYSICAL = auto()
     LOGICAL_ORDERBY_TO_PHYSICAL = auto()
     LOGICAL_LIMIT_TO_PHYSICAL = auto()
@@ -75,19 +76,18 @@
     LOGICAL_JOIN_TO_PHYSICAL_NESTED_LOOP_JOIN = auto()
     LOGICAL_FUNCTION_SCAN_TO_PHYSICAL = auto()
     LOGICAL_FILTER_TO_PHYSICAL = auto()
     LOGICAL_PROJECT_TO_PHYSICAL = auto()
     LOGICAL_SHOW_TO_PHYSICAL = auto()
     LOGICAL_DROP_UDF_TO_PHYSICAL = auto()
     LOGICAL_EXPLAIN_TO_PHYSICAL = auto()
-    LOGICAL_CREATE_INDEX_TO_FAISS = auto()
+    LOGICAL_CREATE_INDEX_TO_VECTOR_INDEX = auto()
     LOGICAL_APPLY_AND_MERGE_TO_PHYSICAL = auto()
-    LOGICAL_FAISS_INDEX_SCAN_TO_PHYSICAL = auto()
-
-    IMPLEMENTATION_DELIMETER = auto()
+    LOGICAL_VECTOR_INDEX_SCAN_TO_PHYSICAL = auto()
+    IMPLEMENTATION_DELIMITER = auto()
 
     NUM_RULES = auto()
 
 
 class Promise(IntEnum):
     """
     Manages order in which rules should be applied.
@@ -119,34 +119,35 @@
 
     LOGICAL_FUNCTION_SCAN_TO_PHYSICAL = auto()
     LOGICAL_FILTER_TO_PHYSICAL = auto()
     LOGICAL_PROJECT_TO_PHYSICAL = auto()
     LOGICAL_SHOW_TO_PHYSICAL = auto()
     LOGICAL_DROP_UDF_TO_PHYSICAL = auto()
     LOGICAL_EXPLAIN_TO_PHYSICAL = auto()
-    LOGICAL_CREATE_INDEX_TO_FAISS = auto()
+    LOGICAL_CREATE_INDEX_TO_VECTOR_INDEX = auto()
     LOGICAL_APPLY_AND_MERGE_TO_PHYSICAL = auto()
-    LOGICAL_FAISS_INDEX_SCAN_TO_PHYSICAL = auto()
+    LOGICAL_VECTOR_INDEX_SCAN_TO_PHYSICAL = auto()
 
     # IMPLEMENTATION DELIMITER
-    IMPLEMENTATION_DELIMETER = auto()
+    IMPLEMENTATION_DELIMITER = auto()
 
     # TRANSFORMATION RULES (LOGICAL -> LOGICAL)
     LOGICAL_INNER_JOIN_COMMUTATIVITY = auto()
     CACHE_FUNCTION_EXPRESISON_IN_APPLY = auto()
     CACHE_FUNCTION_EXPRESISON_IN_FILTER = auto()
     CACHE_FUNCTION_EXPRESISON_IN_PROJECT = auto()
 
     # REWRITE RULES
     EMBED_FILTER_INTO_GET = auto()
     EMBED_SAMPLE_INTO_GET = auto()
+    XFORM_EXTRACT_OBJECT_TO_LINEAR_FLOW = auto()
     XFORM_LATERAL_JOIN_TO_LINEAR_FLOW = auto()
     PUSHDOWN_FILTER_THROUGH_JOIN = auto()
     PUSHDOWN_FILTER_THROUGH_APPLY_AND_MERGE = auto()
-    COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN = auto()
+    COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_VECTOR_INDEX_SCAN = auto()
     REORDER_PREDICATES = auto()
 
 
 class Rule(ABC):
     """Base class to define any optimization rule
 
     Arguments:
@@ -167,30 +168,30 @@
     def pattern(self):
         return self._pattern
 
     def top_match(self, opr: Operator) -> bool:
         return opr.opr_type == self.pattern.opr_type
 
     def is_implementation_rule(self):
-        return self.rule_type.value > RuleType.TRANSFORMATION_DELIMETER.value
+        return self.rule_type.value > RuleType.TRANSFORMATION_DELIMITER.value
 
     def is_logical_rule(self):
         return (
-            self.rule_type.value > RuleType.REWRITE_DELIMETER.value
-            and self.rule_type.value < RuleType.TRANSFORMATION_DELIMETER.value
+            self.rule_type.value > RuleType.REWRITE_DELIMITER.value
+            and self.rule_type.value < RuleType.TRANSFORMATION_DELIMITER.value
         )
 
     def is_stage_two_rewrite_rules(self):
         return (
-            self.rule_type.value > RuleType.TOP_DOWN_DELIMETER.value
-            and self.rule_type.value < RuleType.REWRITE_DELIMETER.value
+            self.rule_type.value > RuleType.TOP_DOWN_DELIMITER.value
+            and self.rule_type.value < RuleType.REWRITE_DELIMITER.value
         )
 
     def is_stage_one_rewrite_rules(self):
-        return self.rule_type.value < RuleType.TOP_DOWN_DELIMETER.value
+        return self.rule_type.value < RuleType.TOP_DOWN_DELIMITER.value
 
     @abstractmethod
     def promise(self) -> int:
         raise NotImplementedError
 
     @abstractmethod
     def check(self, before: Operator, context: OptimizerContext) -> bool:
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/rules/rules_manager.py` & `evadb-0.2.4/eva/optimizer/rules/rules_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,27 @@
 from eva.experimental.ray.optimizer.rules.rules import (
     LogicalProjectToPhysical as DistributedLogicalProjectToPhysical,
 )
 from eva.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CacheFunctionExpressionInFilter,
     CacheFunctionExpressionInProject,
-    CombineSimilarityOrderByAndLimitToFaissIndexScan,
+    CombineSimilarityOrderByAndLimitToVectorIndexScan,
     EmbedFilterIntoGet,
     EmbedSampleIntoGet,
     LogicalApplyAndMergeToPhysical,
-    LogicalCreateIndexToFaiss,
+    LogicalCreateIndexToVectorIndex,
     LogicalCreateMaterializedViewToPhysical,
     LogicalCreateToPhysical,
     LogicalCreateUDFToPhysical,
     LogicalDeleteToPhysical,
     LogicalDerivedGetToPhysical,
     LogicalDropToPhysical,
     LogicalDropUDFToPhysical,
     LogicalExplainToPhysical,
-    LogicalFaissIndexScanToPhysical,
     LogicalFilterToPhysical,
     LogicalFunctionScanToPhysical,
 )
 from eva.optimizer.rules.rules import (
     LogicalGetToSeqScan as SequentialLogicalGetToSeqScan,
 )
 from eva.optimizer.rules.rules import (
@@ -63,17 +62,19 @@
 from eva.optimizer.rules.rules import (
     LogicalProjectToPhysical as SequentialLogicalProjectToPhysical,
 )
 from eva.optimizer.rules.rules import (
     LogicalRenameToPhysical,
     LogicalShowToPhysical,
     LogicalUnionToPhysical,
+    LogicalVectorIndexScanToPhysical,
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
+    XformExtractObjectToLinearFlow,
     XformLateralJoinToLinearFlow,
 )
 from eva.optimizer.rules.rules_base import Rule
 
 
 class RulesManager:
     def __init__(self):
@@ -82,23 +83,24 @@
             CacheFunctionExpressionInApply(),
             CacheFunctionExpressionInFilter(),
             CacheFunctionExpressionInProject(),
         ]
 
         self._stage_one_rewrite_rules = [
             XformLateralJoinToLinearFlow(),
+            XformExtractObjectToLinearFlow(),
         ]
 
         self._stage_two_rewrite_rules = [
             EmbedFilterIntoGet(),
             # EmbedFilterIntoDerivedGet(),
             EmbedSampleIntoGet(),
             PushDownFilterThroughJoin(),
             PushDownFilterThroughApplyAndMerge(),
-            CombineSimilarityOrderByAndLimitToFaissIndexScan(),
+            CombineSimilarityOrderByAndLimitToVectorIndexScan(),
             ReorderPredicates(),
         ]
 
         ray_enabled = ConfigurationManager().get_value("experimental", "ray")
 
         self._implementation_rules = [
             LogicalCreateToPhysical(),
@@ -124,17 +126,17 @@
             LogicalCreateMaterializedViewToPhysical(),
             LogicalFilterToPhysical(),
             DistributedLogicalProjectToPhysical()
             if ray_enabled
             else SequentialLogicalProjectToPhysical(),
             LogicalShowToPhysical(),
             LogicalExplainToPhysical(),
-            LogicalCreateIndexToFaiss(),
+            LogicalCreateIndexToVectorIndex(),
             LogicalApplyAndMergeToPhysical(),
-            LogicalFaissIndexScanToPhysical(),
+            LogicalVectorIndexScanToPhysical(),
         ]
 
         if ray_enabled:
             self._implementation_rules.append(LogicalExchangeToPhysical())
         self._all_rules = (
             self._stage_one_rewrite_rules
             + self._stage_two_rewrite_rules
@@ -205,15 +207,15 @@
 
 
 @contextmanager
 def disable_rules(rules: List[Rule]):
     """Use this function to temporarily drop rules.
         Useful for testing and debugging purposes.
     Args:
-        rules (List[Rule]): List of rules to temporirly drop
+        rules (List[Rule]): List of rules to temporarily drop
     """
     try:
         rules_manager = RulesManager()
         rules_manager.disable_rules(rules)
         yield rules_manager
     finally:
         rules_manager.add_rules(rules)
```

### Comparing `evadb-0.2.3.post0/eva/optimizer/statement_to_opr_convertor.py` & `evadb-0.2.4/eva/optimizer/statement_to_opr_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     LogicalCreateIndex,
     LogicalCreateMaterializedView,
     LogicalCreateUDF,
     LogicalDelete,
     LogicalDrop,
     LogicalDropUDF,
     LogicalExplain,
+    LogicalExtractObject,
     LogicalFilter,
     LogicalFunctionScan,
     LogicalGet,
     LogicalGroupBy,
     LogicalInsert,
     LogicalJoin,
     LogicalLimit,
@@ -53,18 +54,19 @@
 from eva.parser.insert_statement import InsertTableStatement
 from eva.parser.load_statement import LoadDataStatement
 from eva.parser.rename_statement import RenameTableStatement
 from eva.parser.select_statement import SelectStatement
 from eva.parser.show_statement import ShowStatement
 from eva.parser.statement import AbstractStatement
 from eva.parser.table_ref import TableRef
+from eva.parser.types import UDFType
 from eva.utils.logging_manager import logger
 
 
-class StatementToPlanConvertor:
+class StatementToPlanConverter:
     def __init__(self):
         self._plan = None
 
     def visit_table_ref(self, table_ref: TableRef):
         """Bind table ref object and convert to LogicalGet, LogicalJoin,
             LogicalFunctionScan, or LogicalQueryDerivedGet
 
@@ -74,19 +76,27 @@
         if table_ref.is_table_atom():
             # Table
             catalog_entry = table_ref.table.table_obj
             self._plan = LogicalGet(table_ref, catalog_entry, table_ref.alias)
 
         elif table_ref.is_table_valued_expr():
             tve = table_ref.table_valued_expr
-            self._plan = LogicalFunctionScan(
-                func_expr=tve.func_expr,
-                alias=table_ref.alias,
-                do_unnest=tve.do_unnest,
-            )
+            if tve.func_expr.name.lower() == str(UDFType.EXTRACT_OBJECT).lower():
+                self._plan = LogicalExtractObject(
+                    detector=tve.func_expr.children[1],
+                    tracker=tve.func_expr.children[2],
+                    alias=table_ref.alias,
+                    do_unnest=tve.do_unnest,
+                )
+            else:
+                self._plan = LogicalFunctionScan(
+                    func_expr=tve.func_expr,
+                    alias=table_ref.alias,
+                    do_unnest=tve.do_unnest,
+                )
 
         elif table_ref.is_select():
             # NestedQuery
             self.visit_select(table_ref.select_statement)
             child_plan = self._plan
             self._plan = LogicalQueryDerivedGet(table_ref.alias)
             self._plan.append_child(child_plan)
@@ -218,42 +228,42 @@
         # Ready to create Logical node
         insert_opr = LogicalInsert(
             table_ref, table_metainfo, statement.column_list, value_list)
         self._plan = insert_opr
         """
 
     def visit_create(self, statement: AbstractStatement):
-        """Convertor for parsed insert Statement
+        """Converter for parsed insert Statement
 
         Arguments:
             statement {AbstractStatement} - - [Create statement]
         """
         table_info = statement.table_info
         if table_info is None:
             logger.error("Missing Table Name In Create Statement")
 
         create_opr = LogicalCreate(
             table_info, statement.column_list, statement.if_not_exists
         )
         self._plan = create_opr
 
     def visit_rename(self, statement: RenameTableStatement):
-        """Convertor for parsed rename statement
+        """Converter for parsed rename statement
         Arguments:
             statement(RenameTableStatement): [Rename statement]
         """
         rename_opr = LogicalRename(statement.old_table_ref, statement.new_table_name)
         self._plan = rename_opr
 
     def visit_drop(self, statement: DropTableStatement):
         drop_opr = LogicalDrop(statement.table_infos, statement.if_exists)
         self._plan = drop_opr
 
     def visit_create_udf(self, statement: CreateUDFStatement):
-        """Convertor for parsed create udf statement
+        """Converter for parsed create udf statement
 
         Arguments:
             statement {CreateUDFStatement} - - Create UDF Statement
         """
         annotated_inputs = column_definition_to_udf_io(statement.inputs, True)
         annotated_outputs = column_definition_to_udf_io(statement.outputs, False)
         annotated_metadata = metadata_definition_to_udf_metadata(statement.metadata)
@@ -266,23 +276,23 @@
             statement.impl_path,
             statement.udf_type,
             annotated_metadata,
         )
         self._plan = create_udf_opr
 
     def visit_drop_udf(self, statement: DropUDFStatement):
-        """Convertor for parsed DROP UDF statement
+        """Converter for parsed DROP UDF statement
 
         Arguments:
             statement {DropUDFStatement} - Drop UDF Statement
         """
         self._plan = LogicalDropUDF(statement.name, statement.if_exists)
 
     def visit_load_data(self, statement: LoadDataStatement):
-        """Convertor for parsed load data statement
+        """Converter for parsed load data statement
         Arguments:
             statement(LoadDataStatement): [Load data statement]
         """
         load_data_opr = LogicalLoadData(
             statement.table_info,
             statement.path,
             statement.column_list,
@@ -308,15 +318,15 @@
         self._plan = explain_opr
 
     def visit_create_index(self, statement: CreateIndexStatement):
         create_index_opr = LogicalCreateIndex(
             statement.name,
             statement.table_ref,
             statement.col_list,
-            statement.index_type,
+            statement.vector_store_type,
             statement.udf_func,
         )
         self._plan = create_index_opr
 
     def visit_delete(self, statement: DeleteTableStatement):
         delete_opr = LogicalDelete(
             statement.table_ref,
```

### Comparing `evadb-0.2.3.post0/eva/parser/__init__.py` & `evadb-0.2.4/eva/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/alias.py` & `evadb-0.2.4/eva/parser/alias.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/create_index_statement.py` & `evadb-0.2.4/eva/parser/create_index_statement.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
 
-from eva.catalog.catalog_type import IndexType
+from eva.catalog.catalog_type import VectorStoreType
 from eva.expression.function_expression import FunctionExpression
 from eva.parser.create_statement import ColumnDefinition
 from eva.parser.statement import AbstractStatement
 from eva.parser.table_ref import TableRef
 from eva.parser.types import StatementType
 
 
 class CreateIndexStatement(AbstractStatement):
     def __init__(
         self,
         name: str,
         table_ref: TableRef,
         col_list: List[ColumnDefinition],
-        index_type: IndexType,
+        vector_store_type: VectorStoreType,
         udf_func: FunctionExpression = None,
     ):
         super().__init__(StatementType.CREATE_INDEX)
         self._name = name
         self._table_ref = table_ref
         self._col_list = col_list
-        self._index_type = index_type
+        self._vector_store_type = vector_store_type
         self._udf_func = udf_func
 
     def __str__(self) -> str:
         print_str = "CREATE INDEX {} ON {} ({}{}) ".format(
             self._name,
             self._table_ref,
             "" if self._udf_func else self._udf_func,
@@ -56,36 +56,36 @@
         return self._table_ref
 
     @property
     def col_list(self):
         return self._col_list
 
     @property
-    def index_type(self):
-        return self._index_type
+    def vector_store_type(self):
+        return self._vector_store_type
 
     @property
     def udf_func(self):
         return self._udf_func
 
     def __eq__(self, other):
         if not isinstance(other, CreateIndexStatement):
             return False
         return (
             self._name == other.name
             and self._table_ref == other.table_ref
             and self.col_list == other.col_list
-            and self._index_type == other.index_type
+            and self._vector_store_type == other.vector_store_type
             and self._udf_func == other.udf_func
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 super().__hash__(),
                 self._name,
                 self._table_ref,
                 tuple(self.col_list),
-                self._index_type,
+                self._vector_store_type,
                 self._udf_func,
             )
         )
```

### Comparing `evadb-0.2.3.post0/eva/parser/create_mat_view_statement.py` & `evadb-0.2.4/eva/parser/create_mat_view_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/create_statement.py` & `evadb-0.2.4/eva/parser/create_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/create_udf_statement.py` & `evadb-0.2.4/eva/parser/create_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/delete_statement.py` & `evadb-0.2.4/eva/parser/delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/drop_statement.py` & `evadb-0.2.4/eva/parser/drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/drop_udf_statement.py` & `evadb-0.2.4/eva/parser/drop_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/eva.lark` & `evadb-0.2.4/eva/parser/eva.lark`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 // Data Definition Language
 
 //    Create statements
 
 create_database: CREATE DATABASE if_not_exists? uid
 
-create_index: CREATE INDEX uid ON table_name index_elem index_type?
+create_index: CREATE INDEX uid ON table_name index_elem vector_store_type?
 
 create_table: CREATE TABLE if_not_exists? table_name create_definitions 
     
 // Rename statements
 
 rename_table: RENAME TABLE table_name TO table_name
     
@@ -41,15 +41,15 @@
 
 udf_metadata: udf_metadata_key udf_metadata_value
 
 udf_metadata_key: string_literal
 
 udf_metadata_value: string_literal | decimal_literal
 
-index_type: USING HNSW
+vector_store_type: USING (FAISS | QDRANT)
 
 index_elem: ("(" uid_list ")"
           | "(" function_call ")")
 
 create_definitions: "(" create_definition ("," create_definition)* ")"
 
 create_definition: uid column_definition          -> column_declaration
@@ -378,14 +378,16 @@
 FORMAT:               "FORMAT"i
 CSV:                  "CSV"i
 VIDEO:                "VIDEO"i
 IMAGE:                "IMAGE"i
 
 // Index types
 HNSW:                                "HNSW"i
+FAISS:                               "FAISS"i
+QDRANT:                              "QDRANT"i
 
 // Computer vision tasks
 
 OBJECT_DETECTION:                    "OBJECT_DETECTION"i
 ACTION_CLASSICATION:                 "ACTION_CLASSICATION"i
 
 // DATA TYPE Keywords
@@ -441,40 +443,40 @@
 VIEW:                                "VIEW"i
 
 // Common function names
 
 ABS:                                 "ABS"i
 
 // Operators
-// Operators. Assigns
+// Operators. Assignment
 
 VAR_ASSIGN:                          ":="
 PLUS_ASSIGN:                         "+="
 MINUS_ASSIGN:                        "-="
 MULT_ASSIGN:                         "*="
 DIV_ASSIGN:                          "/="
 MOD_ASSIGN:                          "%="
 AND_ASSIGN:                          "&="
 XOR_ASSIGN:                          "^="
 OR_ASSIGN:                           "|="
 
 
-// Operators. Arithmetics
+// Operators. Arithmetic
 
 STAR:                                "*"
 DIVIDE:                              "/"
 MODULUS:                              "%"
 PLUS:                                "+"
 MINUSMINUS:                          "--"
 MINUS:                               "-"
 DIV:                                 "DIV"
 MOD:                                 "MOD"
 
 
-// Operators. Comparation
+// Operators. Comparison
 
 EQUAL_SYMBOL:                        "="
 GREATER_SYMBOL:                      ">"
 LESS_SYMBOL:                         "<"
 EXCLAMATION_SYMBOL:                  "!"
 GREATER_OR_EQUAL_SYMBOL:             "<="
 LESS_OR_EQUAL_SYMBOL:                ">="
```

### Comparing `evadb-0.2.3.post0/eva/parser/explain_statement.py` & `evadb-0.2.4/eva/parser/explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/insert_statement.py` & `evadb-0.2.4/eva/parser/insert_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_parser.py` & `evadb-0.2.4/eva/parser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/__init__.py` & `evadb-0.2.4/eva/parser/lark_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.4/eva/parser/lark_visitor/_common_clauses_ids.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_create_statements.py` & `evadb-0.2.4/eva/parser/lark_visitor/_create_statements.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from lark import Tree
 
-from eva.catalog.catalog_type import ColumnType, IndexType, NdArrayType
+from eva.catalog.catalog_type import ColumnType, NdArrayType, VectorStoreType
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.create_index_statement import CreateIndexStatement
 from eva.parser.create_mat_view_statement import CreateMaterializedViewStatement
 from eva.parser.create_statement import (
     ColConstraintInfo,
     ColumnDefinition,
     CreateTableStatement,
@@ -251,38 +251,40 @@
         col_list = [
             ColumnDefinition(uid.col_name, None, None, None) for uid in uid_list
         ]
         return CreateMaterializedViewStatement(
             view_info, col_list, if_not_exists, query
         )
 
-    def index_type(self, tree):
-        index_type = None
+    def vector_store_type(self, tree):
+        vector_store_type = None
         token = tree.children[1]
 
-        if str.upper(token) == "HNSW":
-            index_type = IndexType.HNSW
-        return index_type
+        if str.upper(token) == "FAISS":
+            vector_store_type = VectorStoreType.FAISS
+        elif str.upper(token) == "QDRANT":
+            vector_store_type = VectorStoreType.QDRANT
+        return vector_store_type
 
     # INDEX CREATION
     def create_index(self, tree):
         index_name = None
         table_name = None
-        index_type = None
+        vector_store_type = None
         index_elem = None
 
         for child in tree.children:
             if isinstance(child, Tree):
                 if child.data == "uid":
                     index_name = self.visit(child)
                 elif child.data == "table_name":
                     table_name = self.visit(child)
                     table_ref = TableRef(table_name)
-                elif child.data == "index_type":
-                    index_type = self.visit(child)
+                elif child.data == "vector_store_type":
+                    vector_store_type = self.visit(child)
                 elif child.data == "index_elem":
                     index_elem = self.visit(child)
 
         # Parse either a single UDF function call or column list.
         col_list, udf_func = None, None
         if not isinstance(index_elem, list):
             udf_func = index_elem
@@ -294,9 +296,9 @@
 
         col_list = [
             ColumnDefinition(tv_expr.col_name, None, None, None)
             for tv_expr in index_elem
         ]
 
         return CreateIndexStatement(
-            index_name, table_ref, col_list, index_type, udf_func
+            index_name, table_ref, col_list, vector_store_type, udf_func
         )
```

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.4/eva/parser/lark_visitor/_delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.4/eva/parser/lark_visitor/_drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.4/eva/parser/lark_visitor/_explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_expressions.py` & `evadb-0.2.4/eva/parser/lark_visitor/_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def binary_comparison_predicate(self, tree):
         left = self.visit(tree.children[0])
         op = self.visit(tree.children[1])
         right = self.visit(tree.children[2])
         return ComparisonExpression(op, left, right)
 
     def nested_expression_atom(self, tree):
-        # ToDo Can there be >1 expression in this case
+        # Todo Can there be >1 expression in this case
         expr = tree.children[0]
         return self.visit(expr)
 
     def comparison_operator(self, tree):
         op = str(tree.children[0])
 
         if op == "=":
```

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_functions.py` & `evadb-0.2.4/eva/parser/lark_visitor/_functions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.4/eva/parser/lark_visitor/_insert_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_load_statement.py` & `evadb-0.2.4/eva/parser/lark_visitor/_load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.4/eva/parser/lark_visitor/_rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_select_statement.py` & `evadb-0.2.4/eva/parser/lark_visitor/_select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_show_statements.py` & `evadb-0.2.4/eva/parser/lark_visitor/_show_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/lark_visitor/_table_sources.py` & `evadb-0.2.4/eva/parser/lark_visitor/_table_sources.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/load_statement.py` & `evadb-0.2.4/eva/parser/load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/parser.py` & `evadb-0.2.4/eva/parser/parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/rename_statement.py` & `evadb-0.2.4/eva/parser/rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/select_statement.py` & `evadb-0.2.4/eva/parser/select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/show_statement.py` & `evadb-0.2.4/eva/parser/show_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/statement.py` & `evadb-0.2.4/eva/parser/statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/table_ref.py` & `evadb-0.2.4/eva/parser/table_ref.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/parser/types.py` & `evadb-0.2.4/eva/parser/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,7 +63,11 @@
     CSV  # noqa: F821
     IMAGE  # noqa: F821
 
 
 class ShowType(EVAEnum):
     UDFS  # noqa: F821
     TABLES  # noqa: F821
+
+
+class UDFType(EVAEnum):
+    EXTRACT_OBJECT  # noqa: F821
```

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/__init__.py` & `evadb-0.2.4/eva/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/abstract_join_plan.py` & `evadb-0.2.4/eva/plan_nodes/abstract_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/abstract_plan.py` & `evadb-0.2.4/eva/plan_nodes/abstract_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.4/eva/plan_nodes/abstract_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.4/eva/plan_nodes/apply_and_merge_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/create_index_plan.py` & `evadb-0.2.4/eva/plan_nodes/create_index_plan.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
 
-from eva.catalog.catalog_type import IndexType
+from eva.catalog.catalog_type import VectorStoreType
 from eva.expression.function_expression import FunctionExpression
 from eva.parser.create_statement import ColumnDefinition
 from eva.parser.table_ref import TableRef
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.plan_nodes.types import PlanOprType
 
 
 class CreateIndexPlan(AbstractPlan):
     def __init__(
         self,
         name: str,
         table_ref: TableRef,
         col_list: List[ColumnDefinition],
-        index_type: IndexType,
+        vector_store_type: VectorStoreType,
         udf_func: FunctionExpression = None,
     ):
         super().__init__(PlanOprType.CREATE_INDEX)
         self._name = name
         self._table_ref = table_ref
         self._col_list = col_list
-        self._index_type = index_type
+        self._vector_store_type = vector_store_type
         self._udf_func = udf_func
 
     @property
     def name(self):
         return self._name
 
     @property
@@ -47,38 +47,38 @@
         return self._table_ref
 
     @property
     def col_list(self):
         return self._col_list
 
     @property
-    def index_type(self):
-        return self._index_type
+    def vector_store_type(self):
+        return self._vector_store_type
 
     @property
     def udf_func(self):
         return self._udf_func
 
     def __str__(self):
         return "CreateIndexPlan(name={}, \
             table_ref={}, \
             col_list={}, \
-            index_type={}, \
+            vector_store_type={}, \
             {})".format(
             self._name,
             self._table_ref,
             tuple(self._col_list),
-            self._index_type,
+            self._vector_store_type,
             "" if not self._udf_func else "udf_func={}".format(self._udf_func),
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 super().__hash__(),
                 self.name,
                 self.table_ref,
                 tuple(self.col_list),
-                self.index_type,
+                self.vector_store_type,
                 self.udf_func,
             )
         )
```

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.4/eva/plan_nodes/create_mat_view_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/create_plan.py` & `evadb-0.2.4/eva/plan_nodes/create_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/create_udf_plan.py` & `evadb-0.2.4/eva/plan_nodes/create_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/delete_plan.py` & `evadb-0.2.4/eva/plan_nodes/delete_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/drop_plan.py` & `evadb-0.2.4/eva/plan_nodes/drop_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/drop_udf_plan.py` & `evadb-0.2.4/eva/plan_nodes/drop_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/explain_plan.py` & `evadb-0.2.4/eva/plan_nodes/explain_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/faiss_index_scan_plan.py` & `evadb-0.2.4/eva/plan_nodes/vector_index_scan_plan.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,62 +8,73 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from eva.catalog.catalog_type import VectorStoreType
 from eva.expression.constant_value_expression import ConstantValueExpression
 from eva.expression.function_expression import FunctionExpression
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.plan_nodes.types import PlanOprType
 
 
-class FaissIndexScanPlan(AbstractPlan):
+class VectorIndexScanPlan(AbstractPlan):
     """
     The plan first evaluates the `search_query_expr` expression and searches the output
-    in the Faiss index. The plan finally projects `limit_count` number of results.
+    in the vector index. The plan finally projects `limit_count` number of results.
 
     Arguments:
-        index_name (str): The Faiss index name.
+        index_name (str): The vector index name.
         limit_count (ConstantValueExpression): Number of top results to project.
         search_query_expr (FunctionExpression): function expression to evaluate, whose
-        results will be searched in the Faiss index.
+        results will be searched in the vector index.
     """
 
     def __init__(
         self,
         index_name: str,
+        vector_store_type: VectorStoreType,
         limit_count: ConstantValueExpression,
         search_query_expr: FunctionExpression,
     ):
-        super().__init__(PlanOprType.FAISS_INDEX_SCAN)
+        super().__init__(PlanOprType.VECTOR_INDEX_SCAN)
         self._index_name = index_name
+        self._vector_store_type = vector_store_type
         self._limit_count = limit_count
         self._search_query_expr = search_query_expr
 
     @property
     def index_name(self):
         return self._index_name
 
     @property
+    def vector_store_type(self):
+        return self._vector_store_type
+
+    @property
     def limit_count(self):
         return self._limit_count
 
     @property
     def search_query_expr(self):
         return self._search_query_expr
 
     def __str__(self):
-        return "FaissIndexScan(index_name={}, limit_count={}, search_query_expr={})".format(
-            self._index_name, self._limit_count, self._search_query_expr
+        return "VectorIndexScan(index_name={}, vector_store_type={}, limit_count={}, search_query_expr={})".format(
+            self._index_name,
+            self.vector_store_type,
+            self._limit_count,
+            self._search_query_expr,
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 super().__hash__(),
                 self.index_name,
+                self.vector_store_type,
                 self.limit_count,
                 self.search_query_expr,
             )
         )
```

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/function_scan_plan.py` & `evadb-0.2.4/eva/plan_nodes/function_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/groupby_plan.py` & `evadb-0.2.4/eva/plan_nodes/groupby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.4/eva/plan_nodes/hash_join_build_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class HashJoinBuildPlan(AbstractPlan):
     """
     This plan is used for storing information required for hashjoin build side.
     It prepares the hash table of preferably the smaller relation
     which is used by the probe side to find relevant rows.
     Arguments:
         build_keys (List[ColumnCatalogEntry]) : list of equi-key columns.
-                        If empty, then Cartitian product.
+                        If empty, then Cartesian product.
     """
 
     def __init__(self, join_type: JoinType, build_keys: List[ColumnCatalogEntry]):
         self.join_type = join_type
         self.build_keys = build_keys
         super().__init__(PlanOprType.HASH_BUILD)
```

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.4/eva/plan_nodes/hash_join_probe_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/insert_plan.py` & `evadb-0.2.4/eva/plan_nodes/insert_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/lateral_join_plan.py` & `evadb-0.2.4/eva/plan_nodes/lateral_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/limit_plan.py` & `evadb-0.2.4/eva/plan_nodes/limit_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/load_data_plan.py` & `evadb-0.2.4/eva/plan_nodes/load_data_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.4/eva/plan_nodes/nested_loop_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/orderby_plan.py` & `evadb-0.2.4/eva/plan_nodes/orderby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/pp_plan.py` & `evadb-0.2.4/eva/plan_nodes/pp_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/predicate_plan.py` & `evadb-0.2.4/eva/plan_nodes/predicate_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/project_plan.py` & `evadb-0.2.4/eva/plan_nodes/project_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/rename_plan.py` & `evadb-0.2.4/eva/plan_nodes/rename_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/sample_plan.py` & `evadb-0.2.4/eva/plan_nodes/sample_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/seq_scan_plan.py` & `evadb-0.2.4/eva/plan_nodes/seq_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/show_info_plan.py` & `evadb-0.2.4/eva/plan_nodes/show_info_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/storage_plan.py` & `evadb-0.2.4/eva/plan_nodes/storage_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/types.py` & `evadb-0.2.4/eva/plan_nodes/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,9 +43,9 @@
     PREDICATE_FILTER = auto()
     PROJECT = auto()
     SHOW_INFO = auto()
     DROP_UDF = auto()
     EXPLAIN = auto()
     CREATE_INDEX = auto()
     APPLY_AND_MERGE = auto()
-    FAISS_INDEX_SCAN = auto()
+    VECTOR_INDEX_SCAN = auto()
     # add other types
```

### Comparing `evadb-0.2.3.post0/eva/plan_nodes/union_plan.py` & `evadb-0.2.4/eva/plan_nodes/union_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/readers/__init__.py` & `evadb-0.2.4/eva/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/readers/abstract_reader.py` & `evadb-0.2.4/eva/readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/readers/csv_reader.py` & `evadb-0.2.4/eva/readers/csv_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,18 @@
             to read from the CSV file
         """
 
         self._column_list = column_list
         super().__init__(*args, **kwargs)
 
     def _read(self) -> Iterator[Dict]:
-
         # TODO: What is a good location to put this code?
         def convert_csv_string_to_ndarray(row_string):
             """
-            Conver a string of comma seperated values to a numpy
+            Convert a string of comma separated values to a numpy
             float array
             """
             return np.array([np.float32(val) for val in row_string.split(",")])
 
         logger.info("Reading CSV frames")
 
         # TODO: Need to add strong sanity checks on the columns.
@@ -54,23 +53,20 @@
             col.col_name
             for col in self._column_list
             if col.col_name != IDENTIFIER_COLUMN
         ]
 
         col_map = {col.col_name: col for col in self._column_list}
         for chunk in pd.read_csv(self.file_url, chunksize=512, usecols=col_list_names):
-
             # apply the required conversions
             for col in chunk.columns:
-
                 # TODO: Is there a better way to do this?
                 if (
                     isinstance(chunk[col].iloc[0], str)
                     and col_map[col].col_object.type.name == "NDARRAY"
                 ):
-
                     # convert the string to a numpy array
                     chunk[col] = chunk[col].apply(convert_csv_string_to_ndarray)
 
             # yield the chunk
             for chunk_index, chunk_row in chunk.iterrows():
                 yield chunk_row
```

### Comparing `evadb-0.2.3.post0/eva/readers/decord_reader.py` & `evadb-0.2.4/eva/readers/decord_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         Args:
             predicate (AbstractExpression, optional): If only subset of frames
             need to be read. The predicate should be only on single column and
             can be converted to ranges. Defaults to None.
             sampling_rate (int, optional): Set if the caller wants one frame
             every `sampling_rate` number of frames. For example, if `sampling_rate = 10`, it returns every 10th frame. If both `predicate` and `sampling_rate` are specified, `sampling_rate` is given precedence.
-            sampling_type (str, optional): Set as IFRAMES if caller want to sample on top on iframes only. e.g if the IFRAME frame numbers are [10,20,30,40,50] then'SAMPLE IFRAMES 2' will return [10,30,50]
+            sampling_type (str, optional): Set as IFRAMES if caller want to sample on top on iframes only. e.g if the IFRAME frame numbers are [10,20,30,40,50] then 'SAMPLE IFRAMES 2' will return [10,30,50]
             read_audio (bool, optional): Whether to read audio stream from the video. Defaults to False
             read_video (bool, optional): Whether to read video stream from the video. Defaults to True
         """
         self._predicate = predicate
         self._sampling_rate = sampling_rate or 1
         self._sampling_type = sampling_type
         self._read_audio = read_audio
```

### Comparing `evadb-0.2.3.post0/eva/readers/image/__init__.py` & `evadb-0.2.4/eva/readers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/readers/image/opencv_image_reader.py` & `evadb-0.2.4/test/integration_tests/test_create_table_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Dict, Iterator
+import unittest
 
-import cv2
+from eva.executor.executor_utils import ExecutorError
+from eva.server.command_handler import execute_query_fetch_all
 
-from eva.readers.abstract_reader import AbstractReader
 
+class CreateTableTest(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        pass
 
-class CVImageReader(AbstractReader):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    @classmethod
+    def tearDownClass(cls):
+        pass
 
-    def _read(self) -> Iterator[Dict]:
-        im_bgr = cv2.imread(str(self.file_url))
-        im_rgb = cv2.cvtColor(im_bgr, cv2.COLOR_BGR2RGB)
-        assert im_rgb is not None, f"Failed to read image file {self.file_url}"
-        yield {"data": im_rgb}
+    def test_currently_cannot_create_boolean_table(self):
+        query = """ CREATE TABLE BooleanTable( A BOOLEAN);"""
+
+        with self.assertRaises(ExecutorError):
+            execute_query_fetch_all(query)
```

### Comparing `evadb-0.2.3.post0/eva/server/__init__.py` & `evadb-0.2.4/eva/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/server/command_handler.py` & `evadb-0.2.4/eva/server/command_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 
 from eva.binder.statement_binder import StatementBinder
 from eva.binder.statement_binder_context import StatementBinderContext
 from eva.executor.plan_executor import PlanExecutor
 from eva.models.server.response import Response, ResponseStatus
 from eva.models.storage.batch import Batch
 from eva.optimizer.plan_generator import PlanGenerator
-from eva.optimizer.statement_to_opr_convertor import StatementToPlanConvertor
+from eva.optimizer.statement_to_opr_converter import StatementToPlanConverter
 from eva.parser.parser import Parser
 from eva.utils.logging_manager import logger
 from eva.utils.stats import Timer
 
 
 def execute_query(query, report_time: bool = False, **kwargs) -> Iterator[Batch]:
     """
     Execute the query and return a result generator.
     """
     query_compile_time = Timer()
     plan_generator = kwargs.pop("plan_generator", PlanGenerator())
     with query_compile_time:
         stmt = Parser().parse(query)[0]
         StatementBinder(StatementBinderContext()).bind(stmt)
-        l_plan = StatementToPlanConvertor().visit(stmt)
+        l_plan = StatementToPlanConverter().visit(stmt)
         p_plan = asyncio.run(plan_generator.build(l_plan))
         output = PlanExecutor(p_plan).execute_plan()
 
     query_compile_time.log_elapsed_time("Query Compile Time")
     return output
```

### Comparing `evadb-0.2.3.post0/eva/server/db_api.py` & `evadb-0.2.4/eva/server/db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/server/interpreter.py` & `evadb-0.2.4/eva/server/interpreter.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,32 +52,31 @@
     return stream_reader
 
 
 async def read_from_client_and_send_to_server(
     stdin_reader: StreamReader, writer: StreamWriter, server_reader: StreamReader
 ):
     VERSION = VERSION_DICT["VERSION"]
-    intro = "eva (v " + VERSION + ')\nType "EXIT;" to exit the client' + "\n"
-    sys.stdout.write(intro)
-    sys.stdout.flush()
+    intro = f"eva (v{VERSION})\nType 'EXIT;' to exit the client \n"
+    print(intro, flush=True)
 
     prompt = "eva=#"
 
     connection = EVAConnection(server_reader, writer)
     cursor = connection.cursor()
 
     while True:
         sys.stdout.write(prompt)
         sys.stdout.flush()
         query = await read_line(stdin_reader)
         logger.debug("Query: --|" + query + "|--")
 
         query = query.lstrip()
         query = query.rstrip()
-        if query in ["EXIT", "QUIT"]:
+        if query.upper() in ["EXIT", "QUIT"]:
             return
 
         await cursor.execute_async(query)
         response = await cursor.fetch_all_async()
         sys.stdout.write(str(response) + "\n")
         sys.stdout.flush()
```

### Comparing `evadb-0.2.3.post0/eva/server/server.py` & `evadb-0.2.4/eva/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         Start the server
         Server objects are asynchronous context managers.
 
         hostname: hostname of the server
         port: port of the server
         """
         logger.info("Start Server")
+        print(f"EVA Server started at host {host} and port {port}", flush=True)
 
         self._server = await asyncio.start_server(self.accept_client, host, port)
 
         async with self._server:
             await self._server.serve_forever()
 
         logger.info("Successfully shutdown server")
@@ -73,15 +74,15 @@
                 data = await asyncio.wait_for(client_reader.readline(), timeout=None)
                 if data == b"":
                     break
 
                 message = data.decode().rstrip()
                 logger.debug("Received --|%s|--", message)
 
-                if message in ["EXIT;", "QUIT;"]:
+                if message.upper() in ["EXIT;", "QUIT;"]:
                     logger.info("Close client")
                     return
 
                 logger.debug("Handle request")
                 asyncio.create_task(handle_request(client_writer, message))
 
         except Exception as e:
```

### Comparing `evadb-0.2.3.post0/eva/storage/__init__.py` & `evadb-0.2.4/eva/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/storage/abstract_media_storage_engine.py` & `evadb-0.2.4/eva/storage/abstract_media_storage_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
             )
         )
 
     def _xform_file_url_to_file_name(self, file_url: Path) -> str:
         # Convert media_path to file name. This is done to support duplicate media_names with
         # different complete paths. Without conversion, we cannot copy files with same name but
         # different paths. Eg., a/b/my.mp4 and a/b/c/my.mp4.
-        # xfromed_file_name = zlib.crc32(str(file_url).encode("utf-8")) & 0xFFFFFFFF
-        # return str(xfromed_file_name)
+        # xformed_file_name = zlib.crc32(str(file_url).encode("utf-8")) & 0xFFFFFFFF
+        # return str(xformed_file_name)
 
         # Previous approach with hashing is commented out above. Since we now use symbolic link, the only
         # thing we need to worry about is the same file name under different directory. This motivates us
-        # to just breakdown directory also as part of file name. Additionaly, it does not use hashing,
-        # whcih avoids computation overhead.
+        # to just breakdown directory also as part of file name. Additionally, it does not use hashing,
+        # which avoids computation overhead.
         file_path_str = str(file_url)
         file_path = re.sub(r"[^a-zA-Z0-9 \.\n]", "_", file_path_str)
         return file_path
 
     def create(self, table: TableCatalogEntry, if_not_exists=True):
         """
         Create the directory to store the images.
```

### Comparing `evadb-0.2.3.post0/eva/storage/abstract_storage_engine.py` & `evadb-0.2.4/eva/storage/abstract_storage_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def read(
         self,
         table: TableCatalogEntry,
         batch_mem_size: int = 30000000,
         predicate: AbstractExpression = None,
     ) -> Iterator[Batch]:
         """Interface responsible for yielding row/rows to the client.
-        This should be implemeneted as an interator over of table. Helpful
+        This should be implemented as an iterator over of table. Helpful
         while doing full table scan. `pos` parameter is used if user wants
         to fetch specific rows.
 
         Attributes:
             table: storage unit to be read
             pos: row position to be returned
```

### Comparing `evadb-0.2.3.post0/eva/storage/image_storage_engine.py` & `evadb-0.2.4/eva/storage/image_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/storage/sqlite_storage_engine.py` & `evadb-0.2.4/eva/storage/sqlite_storage_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     def _dict_to_sql_row(self, dict_row: dict, columns: List[ColumnCatalogEntry]):
         # Serialize numpy data
         for col in columns:
             if col.type == ColumnType.NDARRAY:
                 dict_row[col.name] = self._serializer.serialize(dict_row[col.name])
             elif isinstance(dict_row[col.name], (np.generic,)):
-                # SqlAlchemy does not consume numpy generic data types
+                # Sqlalchemy does not consume numpy generic data types
                 # convert numpy datatype to python generic datatype using tolist()
                 # eg. np.int64 -> int
                 # https://stackoverflow.com/a/53067954
                 dict_row[col.name] = dict_row[col.name].tolist()
         return dict_row
 
     def _sql_row_to_dict(self, sql_row: tuple, columns: List[ColumnCatalogEntry]):
@@ -94,16 +94,18 @@
         # the sqlalchemy engine.
         table_columns = [col for col in table.columns if col.name != IDENTIFIER_COLUMN]
         sqlalchemy_schema = SchemaUtils.xform_to_sqlalchemy_schema(table_columns)
 
         attr_dict.update(sqlalchemy_schema)
         # dynamic schema generation
         # https://sparrigan.github.io/sql/sqla/2016/01/03/dynamic-tables.html
-        new_table = type("__placeholder_class_name", (BaseModel,), attr_dict)()
-        BaseModel.metadata.tables[table.name].create(self._sql_engine)
+        new_table = type("__placeholder_class_name__", (BaseModel,), attr_dict)()
+        table = BaseModel.metadata.tables[table.name]
+        if not table.exists():
+            BaseModel.metadata.tables[table.name].create(self._sql_engine)
         self._sql_session.commit()
         return new_table
 
     def drop(self, table: TableCatalogEntry):
         try:
             table_to_remove = self._try_loading_table_via_reflection(table.name)
             table_to_remove.drop()
@@ -133,15 +135,15 @@
             # During table writes, assume row_id is automatically handled by
             # the sqlalchemy engine. Another assumption we make here is the
             # updated data need not to take care of row_id.
             table_columns = [
                 col for col in table.columns if col.name != IDENTIFIER_COLUMN
             ]
 
-            # ToDo: validate the data type before inserting into the table
+            # Todo: validate the data type before inserting into the table
             for record in rows.frames.values:
                 row_data = {col: record[idx] for idx, col in enumerate(columns)}
                 data.append(self._dict_to_sql_row(row_data, table_columns))
             self._sql_engine.execute(table_to_update.insert(), data)
             self._sql_session.commit()
         except Exception as e:
             err_msg = f"Failed to update the table {table.name} with exception {str(e)}"
@@ -163,15 +165,15 @@
         """
         try:
             table_to_read = self._try_loading_table_via_reflection(table.name)
             result = self._sql_engine.execute(table_to_read.select())
             data_batch = []
             row_size = None
             for row in result:
-                # Todo: Verfiy the order of columns in row matches the table.columns
+                # Todo: Verify the order of columns in row matches the table.columns
                 # For table read, we provide row_id so that user can also retrieve
                 # row_id from the table.
                 data_batch.append(self._sql_row_to_dict(row, table.columns))
                 if row_size is None:
                     row_size = 0
                     row_size = get_size(data_batch)
                 if len(data_batch) * row_size >= batch_mem_size:
```

### Comparing `evadb-0.2.3.post0/eva/storage/storage_engine.py` & `evadb-0.2.4/eva/storage/storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/storage/video_storage_engine.py` & `evadb-0.2.4/eva/storage/video_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/third_party/__init__.py` & `evadb-0.2.4/eva/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/third_party/huggingface/__init__.py` & `evadb-0.2.4/eva/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""huggingface related utils"""
+"""general eva utils"""
```

### Comparing `evadb-0.2.3.post0/eva/third_party/huggingface/binder.py` & `evadb-0.2.4/eva/third_party/huggingface/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/third_party/huggingface/create.py` & `evadb-0.2.4/eva/third_party/huggingface/create.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/third_party/huggingface/model.py` & `evadb-0.2.4/eva/third_party/huggingface/model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/__init__.py` & `evadb-0.2.4/eva/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/abstract/__init__.py` & `evadb-0.2.4/eva/udfs/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/abstract/abstract_udf.py` & `evadb-0.2.4/eva/udfs/abstract/abstract_udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return self.name
 
     """Abstract Methods all UDFs must implement. """
 
     @abstractmethod
     def setup(self, *args, **kwargs) -> None:
         """
-        Do necessary setup in here. Gets called automatically on intialization.
+        Do necessary setup in here. Gets called automatically on initialization.
         """
         pass
 
     @abstractmethod
     def forward(self, frames: InputType) -> InputType:
         """
         Implement UDF function call by overriding this function.
```

### Comparing `evadb-0.2.3.post0/eva/udfs/abstract/hf_abstract_udf.py` & `evadb-0.2.4/eva/udfs/abstract/hf_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.4/eva/udfs/abstract/pytorch_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/asl_action_recognition.py` & `evadb-0.2.4/eva/udfs/asl_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/chatgpt.py` & `evadb-0.2.4/eva/udfs/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class ChatGPT(AbstractUDF):
     @property
     def name(self) -> str:
         return "ChatGPT"
 
-    @setup(cachable=False, udf_type="chat-completion", batchable=True)
+    @setup(cacheable=False, udf_type="chat-completion", batchable=True)
     def setup(
         self,
         model="gpt-3.5-turbo",
         temperature: float = 0,
     ) -> None:
         openai.api_key = ConfigurationManager().get_value(
             "third_party", "openai_api_key"
```

### Comparing `evadb-0.2.3.post0/eva/udfs/decorators/__init__.py` & `evadb-0.2.4/eva/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/decorators/decorators.py` & `evadb-0.2.4/eva/udfs/decorators/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 from typing import List
 
 from eva.udfs.decorators.io_descriptors.abstract_types import IOArgument
 
 
-def setup(cachable: bool = False, udf_type: str = "Abstract", batchable: bool = True):
+def setup(cacheable: bool = False, udf_type: str = "Abstract", batchable: bool = True):
     """decorator for the setup function. It will be used to set the cache, batching and
     udf_type parameters in the catalog
 
     Args:
         use_cache (bool): True if the udf should be cached
         udf_type (str): Type of the udf
         batch (bool): True if the udf should be batched
@@ -31,15 +31,15 @@
 
     def inner_fn(arg_fn):
         def wrapper(*args, **kwargs):
             # calling the setup function defined by the user inside the udf implementation
             arg_fn(*args, **kwargs)
 
         tags = {}
-        tags["cachable"] = cachable
+        tags["cacheable"] = cacheable
         tags["udf_type"] = udf_type
         tags["batchable"] = batchable
         wrapper.tags = tags
         return wrapper
 
     return inner_fn
```

### Comparing `evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.4/eva/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.4/eva/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         """
         pass
 
 
 class IOColumnArgument(IOArgument):
     """
-    Base class for IO arguments that are represented indvidually as columns in the catalog.
+    Base class for IO arguments that are represented individually as columns in the catalog.
     """
 
     @abstractmethod
     def __init__(
         self,
         name: str = None,
         type: ColumnType = None,
```

### Comparing `evadb-0.2.3.post0/eva/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.4/eva/udfs/decorators/io_descriptors/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         if not self.column_types:
             self.column_types = [NdArrayType.ANYTYPE] * len(self.columns)
 
         if not self.column_shapes:
             self.column_shapes = [Dimension.ANYDIM] * len(self.columns)
 
-        # check that columns, column_types and column_shpes are of same length
+        # check that columns, column_types and column_shapes are of same length
         if len(self.columns) != len(self.column_types) or len(self.columns) != len(
             self.column_shapes
         ):
             raise UDFIODefinitionError(
                 "columns, column_types and column_shapes should be of same length if specified. "
             )
```

### Comparing `evadb-0.2.3.post0/eva/udfs/decorators/utils.py` & `evadb-0.2.4/eva/udfs/decorators/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,12 +27,27 @@
         udf (Object): UDF object
         is_input (bool, optional): True if inputs are to be loaded. Defaults to False.
 
     Returns:
         Type[UdfIOCatalogEntry]: UdfIOCatalogEntry object created from the input decorator in setup
     """
     tag_key = "input" if is_input else "output"
-    io_signature = udf.forward.tags[tag_key]
+    io_signature = None
+    if hasattr(udf.forward, "tags") and tag_key in udf.forward.tags:
+        io_signature = udf.forward.tags[tag_key]
+    else:
+        # Attempt to populate from the parent class and stop at the first parent class
+        # where the required tags are found.
+        for base_class in udf.__bases__:
+            if hasattr(base_class, "forward") and hasattr(base_class.forward, "tags"):
+                if tag_key in base_class.forward.tags:
+                    io_signature = base_class.forward.tags[tag_key]
+                    break
+
+    assert (
+        io_signature is not None
+    ), f"Cannot infer io signature from the decorator for {udf}."
+
     result_list = []
     for io in io_signature:
         result_list.extend(io.generate_catalog_entries(is_input))
     return result_list
```

### Comparing `evadb-0.2.3.post0/eva/udfs/emotion_detector.py` & `evadb-0.2.4/eva/udfs/emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/face_detector.py` & `evadb-0.2.4/eva/udfs/face_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/fastrcnn_object_detector.py` & `evadb-0.2.4/eva/udfs/fastrcnn_object_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     """
 
     @property
     def name(self) -> str:
         return "fastrcnn"
 
-    @setup(cachable=True, udf_type="object_detection", batchable=True)
+    @setup(cacheable=True, udf_type="object_detection", batchable=True)
     def setup(self, threshold=0.85):
         self.threshold = threshold
         self.model = torchvision.models.detection.fasterrcnn_resnet50_fpn(
             weights="COCO_V1", progress=False
         )
         self.model.eval()
```

### Comparing `evadb-0.2.3.post0/eva/udfs/feature_extractor.py` & `evadb-0.2.4/eva/udfs/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/gpu_compatible.py` & `evadb-0.2.4/eva/udfs/gpu_compatible.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/mvit_action_recognition.py` & `evadb-0.2.4/eva/udfs/mvit_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ndarray/__init__.py` & `evadb-0.2.4/eva/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ndarray/array_count.py` & `evadb-0.2.4/eva/udfs/ndarray/array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ndarray/crop.py` & `evadb-0.2.4/eva/udfs/ndarray/crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.4/eva/udfs/ndarray/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ndarray/open.py` & `evadb-0.2.4/eva/udfs/ndarray/open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ndarray/similarity.py` & `evadb-0.2.4/eva/udfs/ndarray/similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/ocr_extractor.py` & `evadb-0.2.4/eva/udfs/ocr_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/udfs/udf_bootstrap_queries.py` & `evadb-0.2.4/eva/udfs/udf_bootstrap_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,14 +147,27 @@
         TYPE  Classification
         IMPL  '{}/udfs/asl_action_recognition.py';
         """.format(
     EVA_INSTALLATION_DIR
 )
 
 
+norfair_obj_tracker_query = """CREATE UDF IF NOT EXISTS NorFairTracker
+                  IMPL  '{}/udfs/trackers/nor_fair.py';
+        """.format(
+    EVA_INSTALLATION_DIR
+)
+
+Sift_udf_query = """CREATE UDF IF NOT EXISTS SiftFeatureExtractor
+        IMPL  '{}/udfs/sift_feature_extractor.py';
+        """.format(
+    EVA_INSTALLATION_DIR
+)
+
+
 def init_builtin_udfs(mode: str = "debug") -> None:
     """Load the built-in UDFs into the system during system bootstrapping.
 
     The function loads a set of pre-defined UDF queries based on the `mode` argument.
     In 'debug' mode, the function loads debug UDFs along with release UDFs.
     In 'release' mode, only release UDFs are loaded. In addition, in 'debug' mode,
     the function loads a smaller model to accelerate the test suite time.
@@ -167,18 +180,20 @@
     # list of UDF queries to load
     queries = [
         Fastrcnn_udf_query,
         ArrayCount_udf_query,
         Crop_udf_query,
         Open_udf_query,
         Similarity_udf_query,
-        # Disabled because required packages might not be preinstalled
+        norfair_obj_tracker_query,
+        # Disabled because required packages (eg., easy_ocr might not be preinstalled)
         # face_detection_udf_query,
         # ocr_udf_query,
         # Mvit_udf_query, - Disabled as it requires specific pytorch package
+        # Sift_udf_query, - requires package kornia
     ]
 
     if mode == "release":
         # if mode is 'release', add the Yolo query to the list
         queries.append(Yolo_udf_query)
     else:
         # if mode is 'debug', add debug UDFs and a smaller Yolo model
```

### Comparing `evadb-0.2.3.post0/eva/udfs/yolo_object_detector.py` & `evadb-0.2.4/eva/udfs/yolo_object_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         threshold (float): Threshold for classifier confidence score
     """
 
     @property
     def name(self) -> str:
         return "yolo"
 
-    @setup(cachable=True, udf_type="object_detection", batchable=True)
+    @setup(cacheable=True, udf_type="object_detection", batchable=True)
     def setup(self, model: str, threshold=0.3):
         self.threshold = threshold
         self.model = YOLO(model)
         self.device = "cpu"
 
     @forward(
         input_signatures=[
```

### Comparing `evadb-0.2.3.post0/eva/utils/__init__.py` & `evadb-0.2.4/test/executor/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,19 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""general eva utils"""
+from typing import List
+
+from eva.models.storage.batch import Batch
+
+
+class DummyExecutor:
+    def __init__(self, batch_list: List[Batch]):
+        self.batch_list = batch_list
+
+    def exec(self):
+        for batch in self.batch_list:
+            yield batch
```

### Comparing `evadb-0.2.3.post0/eva/utils/errors.py` & `evadb-0.2.4/eva/utils/errors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/utils/generic_utils.py` & `evadb-0.2.4/eva/utils/generic_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,29 +17,38 @@
 import inspect
 import os
 import pickle
 import shutil
 import sys
 import uuid
 from pathlib import Path
+from typing import List
 
 from aenum import AutoEnum, unique
 
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.utils.logging_manager import logger
 
 
 def validate_kwargs(
-    kwargs, allowed_kwargs, error_message="Keyword argument not understood:"
+    kwargs,
+    allowed_keys: List[str],
+    required_keys: List[str],
+    error_message="Keyword argument not understood:",
 ):
     """Checks that all keyword arguments are in the set of allowed keys."""
+    if required_keys is None:
+        required_keys = allowed_keys
     for kwarg in kwargs:
-        if kwarg not in allowed_kwargs:
+        if kwarg not in allowed_keys:
             raise TypeError(error_message, kwarg)
 
+    missing_keys = [key for key in required_keys if key not in kwargs]
+    assert len(missing_keys) == 0, f"Missing required keys, {missing_keys}"
+
 
 def str_to_class(class_path: str):
     """
     Convert string representation of a class path to Class
 
     Arguments:
         class_path (str): absolute path of import
```

### Comparing `evadb-0.2.3.post0/eva/utils/kv_cache.py` & `evadb-0.2.4/eva/utils/kv_cache.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/utils/logging_manager.py` & `evadb-0.2.4/eva/utils/logging_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/utils/s3_utils.py` & `evadb-0.2.4/eva/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/utils/stats.py` & `evadb-0.2.4/eva/utils/stats.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/eva/version.py` & `evadb-0.2.4/eva/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 _MAJOR = "0"
 _MINOR = "2"
-_REVISION = "3.post0"
+_REVISION = "4"
 
 VERSION_SHORT = f"{_MAJOR}.{_MINOR}"
 VERSION = f"{_MAJOR}.{_MINOR}.{_REVISION}"
```

### Comparing `evadb-0.2.3.post0/evadb.egg-info/PKG-INFO` & `evadb-0.2.4/evadb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.3.post0
+Version: 0.2.4
 Summary: EVA AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
 Download-URL: https://github.com/georgia-tech-db/eva
 Description: <div >
@@ -27,15 +27,15 @@
                 <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
                 <a href="https://github.com/orgs/georgia-tech-db/projects/3">
                     <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
                 </a>
                 <a href="https://pepy.tech/project/evadb">
                   <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
                 </a>
-                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>       
+                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
         </div>
         
         <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
         
         EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
         
         ## Quick Links
@@ -63,25 +63,25 @@
         
         ## Demo
         
         Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
         
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
-        
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
          * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
          * ð® <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
          * ð® <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
         
         ## Documentation
         
         * [Detailed Documentation](https://evadb.readthedocs.io/)
-          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>.
+          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/aidb.html">Video Database Systems</a>.
           - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
           - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
         * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
         * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
         * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
         * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
         
@@ -191,15 +191,15 @@
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
         
         ### ð® [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
         
-        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication Models)
+        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
         
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
         
         ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.3.post0 Summary: EVA AI-
-Relational Database System Home-page: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group Author-email: arulraj@gatech.edu License:
-Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/eva
-Description:
+Metadata-Version: 2.1 Name: evadb Version: 0.2.4 Summary: EVA AI-Relational
+Database System Home-page: https://github.com/georgia-tech-db/eva Author:
+Georgia Tech Database Group Author-email: arulraj@gatech.edu License: Apache
+License 2.0 Download-URL: https://github.com/georgia-tech-db/eva Description:
 [EVA]
 # EVA AI-Relational Database System
 [Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
 [Downloads] [Python Versions]
 **** EVA is a database system for building simpler and faster AI-powered
 applications. ****
 EVA is designed for supporting database applications that operate on both
@@ -31,26 +30,27 @@
 user-defined functions - Ã°ÂÂÂ¦ Built-in caching to eliminate redundant model
 invocations across queries - Ã¢ÂÂ¨Ã¯Â¸Â First-class support for PyTorch and
 HuggingFace models - Ã°ÂÂÂ Installable via pip and fully implemented in
 Python ## Demo Here are some illustrative EVA-backed applications (all of them
 are Jupyter notebooks that can be opened in Google Colab): * Ã°ÂÂÂ® Using
 ChatGPT_to_ask_questions_based_on_videos * Ã°ÂÂÂ® Analysing_traffic_flow_at
 an_intersection * Ã°ÂÂÂ® Examining_the_emotion_palette_of_actors_in_a_movie *
-Ã°ÂÂÂ® Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image
-Segmentation_using_Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates *
-Ã°ÂÂÂ® Analysing_toxicity_of_social_media_memes ## Documentation * [Detailed
-Documentation](https://evadb.readthedocs.io/) - If you are wondering why you
-might need an AI-relational database system, start with the page on Video
-Database_Systems. - The Getting_Started page shows how you can use EVA for
-different AI pipelines, and how you can easily extend EVA by defining an user-
-defined function that wraps around your custom deep learning model. - The User
-Guides section contains Jupyter Notebooks that demonstrate how to use various
-features of EVA. Each notebook includes a link to Google Colab to run the code.
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
-emotion-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
+Ã°ÂÂÂ® Image_Similarity_Search_on_Reddit_[FAISS_+_Qdrant] * Ã°ÂÂÂ®
+Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image_Segmentation_using
+Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates * Ã°ÂÂÂ® Analysing
+toxicity_of_social_media_memes ## Documentation * [Detailed Documentation]
+(https://evadb.readthedocs.io/) - If you are wondering why you might need an
+AI-relational database system, start with the page on Video_Database_Systems. -
+The Getting_Started page shows how you can use EVA for different AI pipelines,
+and how you can easily extend EVA by defining an user-defined function that
+wraps around your custom deep learning model. - The User_Guides section
+contains Jupyter Notebooks that demonstrate how to use various features of EVA.
+Each notebook includes a link to Google Colab to run the code. * [Tutorials]
+(https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
 shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
 (https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
 github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 ## Quick Start - Install EVA using the pip package manager. EVA supports Python
 versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
 EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
 notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
@@ -101,15 +101,15 @@
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [MNIST Digit
 Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
 mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
 ----------|--------------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ®
 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/
-tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classfication
+tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification
 Models) | Source Video | Query Result | |---------------|--------------| |
 [Source Video] |[Query Result] | ### Ã°ÂÂÂ® [License Plate Recognition]
 (https://github.com/georgia-tech-db/eva-application-template) (Plate Detection
 + OCR Extraction Models) | Query Result | |--------------| [Query Result] | ###
 Ã°ÂÂÂ® [Meme Toxicity Classification](https://github.com/georgia-tech-db/
 toxicity-classification) (OCR Extraction + Toxicity Classification Models) |
 Query Result | |--------------| [Query Result] | ## Community and Support
```

### Comparing `evadb-0.2.3.post0/evadb.egg-info/SOURCES.txt` & `evadb-0.2.4/evadb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 eva/executor/create_udf_executor.py
 eva/executor/delete_executor.py
 eva/executor/drop_executor.py
 eva/executor/drop_udf_executor.py
 eva/executor/execution_context.py
 eva/executor/executor_utils.py
 eva/executor/explain_executor.py
-eva/executor/faiss_index_scan_executor.py
 eva/executor/function_scan_executor.py
 eva/executor/groupby_executor.py
 eva/executor/hash_join_executor.py
 eva/executor/insert_executor.py
 eva/executor/join_build_executor.py
 eva/executor/lateral_join_executor.py
 eva/executor/limit_executor.py
@@ -75,14 +74,15 @@
 eva/executor/project_executor.py
 eva/executor/rename_executor.py
 eva/executor/sample_executor.py
 eva/executor/seq_scan_executor.py
 eva/executor/show_info_executor.py
 eva/executor/storage_executor.py
 eva/executor/union_executor.py
+eva/executor/vector_index_scan_executor.py
 eva/experimental/__init__.py
 eva/experimental/ray/__init__.py
 eva/experimental/ray/executor/__init__.py
 eva/experimental/ray/executor/exchange_executor.py
 eva/experimental/ray/executor/ray_stage.py
 eva/experimental/ray/optimizer/__init__.py
 eva/experimental/ray/optimizer/rules/__init__.py
@@ -116,15 +116,15 @@
 eva/optimizer/operators.py
 eva/optimizer/optimizer_context.py
 eva/optimizer/optimizer_task_stack.py
 eva/optimizer/optimizer_tasks.py
 eva/optimizer/optimizer_utils.py
 eva/optimizer/plan_generator.py
 eva/optimizer/property.py
-eva/optimizer/statement_to_opr_convertor.py
+eva/optimizer/statement_to_opr_converter.py
 eva/optimizer/rules/__init__.py
 eva/optimizer/rules/pattern.py
 eva/optimizer/rules/rules.py
 eva/optimizer/rules/rules_base.py
 eva/optimizer/rules/rules_manager.py
 eva/parser/__init__.py
 eva/parser/alias.py
@@ -143,18 +143,14 @@
 eva/parser/parser.py
 eva/parser/rename_statement.py
 eva/parser/select_statement.py
 eva/parser/show_statement.py
 eva/parser/statement.py
 eva/parser/table_ref.py
 eva/parser/types.py
-eva/parser/evaql/evaql_lexer.py
-eva/parser/evaql/evaql_parser.py
-eva/parser/evaql/evaql_parserListener.py
-eva/parser/evaql/evaql_parserVisitor.py
 eva/parser/lark_visitor/__init__.py
 eva/parser/lark_visitor/_common_clauses_ids.py
 eva/parser/lark_visitor/_create_statements.py
 eva/parser/lark_visitor/_delete_statement.py
 eva/parser/lark_visitor/_drop_statement.py
 eva/parser/lark_visitor/_explain_statement.py
 eva/parser/lark_visitor/_expressions.py
@@ -174,15 +170,14 @@
 eva/plan_nodes/create_mat_view_plan.py
 eva/plan_nodes/create_plan.py
 eva/plan_nodes/create_udf_plan.py
 eva/plan_nodes/delete_plan.py
 eva/plan_nodes/drop_plan.py
 eva/plan_nodes/drop_udf_plan.py
 eva/plan_nodes/explain_plan.py
-eva/plan_nodes/faiss_index_scan_plan.py
 eva/plan_nodes/function_scan_plan.py
 eva/plan_nodes/groupby_plan.py
 eva/plan_nodes/hash_join_build_plan.py
 eva/plan_nodes/hash_join_probe_plan.py
 eva/plan_nodes/insert_plan.py
 eva/plan_nodes/lateral_join_plan.py
 eva/plan_nodes/limit_plan.py
@@ -195,14 +190,15 @@
 eva/plan_nodes/rename_plan.py
 eva/plan_nodes/sample_plan.py
 eva/plan_nodes/seq_scan_plan.py
 eva/plan_nodes/show_info_plan.py
 eva/plan_nodes/storage_plan.py
 eva/plan_nodes/types.py
 eva/plan_nodes/union_plan.py
+eva/plan_nodes/vector_index_scan_plan.py
 eva/readers/__init__.py
 eva/readers/abstract_reader.py
 eva/readers/csv_reader.py
 eva/readers/decord_reader.py
 eva/readers/image/__init__.py
 eva/readers/image/opencv_image_reader.py
 eva/server/__init__.py
@@ -218,47 +214,57 @@
 eva/storage/storage_engine.py
 eva/storage/video_storage_engine.py
 eva/third_party/__init__.py
 eva/third_party/huggingface/__init__.py
 eva/third_party/huggingface/binder.py
 eva/third_party/huggingface/create.py
 eva/third_party/huggingface/model.py
+eva/third_party/vector_stores/__init__.py
+eva/third_party/vector_stores/faiss.py
+eva/third_party/vector_stores/qdrant.py
+eva/third_party/vector_stores/types.py
+eva/third_party/vector_stores/utils.py
 eva/udfs/__init__.py
 eva/udfs/asl_action_recognition.py
 eva/udfs/chatgpt.py
 eva/udfs/emotion_detector.py
 eva/udfs/face_detector.py
 eva/udfs/fastrcnn_object_detector.py
 eva/udfs/feature_extractor.py
 eva/udfs/gpu_compatible.py
 eva/udfs/mvit_action_recognition.py
 eva/udfs/ocr_extractor.py
+eva/udfs/sift_feature_extractor.py
 eva/udfs/udf_bootstrap_queries.py
 eva/udfs/yolo_object_detector.py
 eva/udfs/abstract/__init__.py
 eva/udfs/abstract/abstract_udf.py
 eva/udfs/abstract/hf_abstract_udf.py
 eva/udfs/abstract/pytorch_abstract_udf.py
+eva/udfs/abstract/tracker_abstract_udf.py
 eva/udfs/decorators/__init__.py
 eva/udfs/decorators/decorators.py
 eva/udfs/decorators/utils.py
 eva/udfs/decorators/io_descriptors/__init__.py
 eva/udfs/decorators/io_descriptors/abstract_types.py
 eva/udfs/decorators/io_descriptors/data_types.py
 eva/udfs/ndarray/__init__.py
 eva/udfs/ndarray/array_count.py
 eva/udfs/ndarray/crop.py
 eva/udfs/ndarray/fuzzy_join.py
 eva/udfs/ndarray/open.py
 eva/udfs/ndarray/similarity.py
+eva/udfs/trackers/__init__.py
+eva/udfs/trackers/nor_fair.py
 eva/utils/__init__.py
 eva/utils/errors.py
 eva/utils/generic_utils.py
 eva/utils/kv_cache.py
 eva/utils/logging_manager.py
+eva/utils/math_utils.py
 eva/utils/s3_utils.py
 eva/utils/stats.py
 evadb.egg-info/PKG-INFO
 evadb.egg-info/SOURCES.txt
 evadb.egg-info/dependency_links.txt
 evadb.egg-info/entry_points.txt
 evadb.egg-info/requires.txt
@@ -272,15 +278,14 @@
 test/benchmark_tests/__init__.py
 test/benchmark_tests/conftest.py
 test/benchmark_tests/test_benchmark_pytorch.py
 test/binder/__init__.py
 test/binder/test_binder_utils.py
 test/binder/test_statement_binder.py
 test/binder/test_statement_binder_context.py
-test/binder/test_statement_binder_python37.py
 test/catalog/__init__.py
 test/catalog/test_catalog_manager.py
 test/catalog/test_column_type.py
 test/catalog/test_sqlalchemy.py
 test/catalog/models/__init__.py
 test/catalog/models/test_models.py
 test/catalog/services/__init__.py
@@ -351,15 +356,15 @@
 test/optimizer/test_cascade_optimizer.py
 test/optimizer/test_cost_model.py
 test/optimizer/test_group.py
 test/optimizer/test_memo.py
 test/optimizer/test_optimizer_context.py
 test/optimizer/test_optimizer_task.py
 test/optimizer/test_optimizer_utils.py
-test/optimizer/test_statement_to_opr_convertor.py
+test/optimizer/test_statement_to_opr_converter.py
 test/optimizer/rules/__init__.py
 test/optimizer/rules/test_rules.py
 test/parser/__init__.py
 test/parser/test_parser.py
 test/parser/test_parser_statements.py
 test/plan_nodes/__init__.py
 test/plan_nodes/test_plan.py
```

### Comparing `evadb-0.2.3.post0/evadb.egg-info/requires.txt` & `evadb-0.2.4/evadb.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 eva-decord>=0.6.1
 facenet-pytorch>=2.5.2
 faiss-cpu
 importlib-metadata<5.0
 ipython<8.13.0
 lark>=1.0.0
 nest_asyncio
+norfair>=2.2.0
 numpy>=1.19.5
 openai>=0.27.4
-opencv-python>=4.6.0.66
+opencv-contrib-python-headless>=4.6.0.66
 pandas>=1.1.5
 pyyaml>=5.1
 ray>=1.13.0
 sqlalchemy-utils>=0.36.6
 sqlalchemy<2.0.0,>=1.4.0
 thefuzz
 timm>=0.6.13
@@ -25,43 +26,49 @@
 ultralytics>=8.0.93
 
 [dev]
 Pillow>=8.4.0
 aenum>=2.2.0
 black>=23.1.0
 boto3
+codespell
 coveralls>=3.0.1
 diskcache>=5.4.0
 eva-decord>=0.6.1
 facenet-pytorch>=2.5.2
 faiss-cpu
 flake8>=3.9.1
 importlib-metadata<5.0
 ipython<8.13.0
 ipywidgets>=7.7.2
 isort>=5.10.1
+kornia
 lark>=1.0.0
 matplotlib>=3.3.4
 moto[s3]>=4.1.1
 nbmake>=1.2.1
 nest-asyncio>=1.5.6
 nest_asyncio
+norfair>=2.2.0
 numpy>=1.19.5
 openai>=0.27.4
-opencv-python>=4.6.0.66
+opencv-contrib-python-headless>=4.6.0.66
 pandas>=1.1.5
+pyenchant
+pylint
 pymysql>=0.10.1
 pytest-asyncio
 pytest-benchmark
 pytest-cov>=2.11.1
 pytest-random-order>=1.0.4
 pytest-virtualenv
 pytest-xdist
 pytest>=6.1.2
 pyyaml>=5.1
+qdrant-client>=1.1.7
 ray>=1.13.0
 scriv>=0.16.0
 sqlalchemy-utils>=0.36.6
 sqlalchemy<2.0.0,>=1.4.0
 thefuzz
 timm>=0.6.13
 torch>=1.10.0
```

### Comparing `evadb-0.2.3.post0/setup.py` & `evadb-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import os
 
 # to read contents of README file
 from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
+from setuptools.command.install import install
+from subprocess import check_call
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 DESCRIPTION = "EVA AI-Relational Database System"
 NAME = "evadb"
 AUTHOR = "Georgia Tech Database Group"
@@ -35,27 +37,27 @@
 DOWNLOAD_URL = "https://github.com/georgia-tech-db/eva"
 LICENSE = "Apache License 2.0"
 VERSION = VERSION_DICT["VERSION"]
 
 minimal_requirement = [
     "numpy>=1.19.5",
     "pandas>=1.1.5",
-    "opencv-python>=4.6.0.66",
+    "opencv-contrib-python-headless>=4.6.0.66",
     "Pillow>=8.4.0",
     "sqlalchemy>=1.4.0,<2.0.0",  # major changes in 2.0.0
     "sqlalchemy-utils>=0.36.6",
     "lark>=1.0.0",
     "pyyaml>=5.1",
     "importlib-metadata<5.0",
     "ray>=1.13.0",
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
     "eva-decord>=0.6.1",
     "boto3",
-    "nest_asyncio"
+    "nest_asyncio",
 ]
 
 formatter_libs = ["black>=23.1.0", "isort>=5.10.1"]
 
 test_libs = [
     "pytest>=6.1.2",
     "pytest-cov>=2.11.1",
@@ -82,15 +84,15 @@
     "faiss-cpu",  # faiss-gpu does not work on mac
 ]
 
 benchmark_libs = [
     "pytest-benchmark",
 ]
 
-doc_libs = []
+doc_libs = ["pyenchant", "codespell", "pylint"]
 
 dist_libs = ["wheel>=0.37.1", "scriv>=0.16.0"]
 
 ### NEEDED FOR AN ALTERNATE DATA SYSTEM OTHER THAN SQLITE
 database_libs = ["pymysql>=0.10.1"]
 
 ### NEEDED FOR A BATTERIES-LOADED EXPERIENCE
@@ -98,14 +100,21 @@
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
     "ipython<8.13.0",  # NOTEBOOKS
     "thefuzz",  # FUZZY STRING MATCHING
     "ultralytics>=8.0.93",  # OBJECT DETECTION
     "transformers>=4.27.4",  # HUGGINGFACE
     "openai>=0.27.4",  # CHATGPT
     "timm>=0.6.13",  # HUGGINGFACE VISION TASKS
+    "norfair>=2.2.0",  # OBJECT TRACKING
+]
+
+### NEEDED FOR EXPERIMENTAL FEATURES
+third_party_libs = [
+    "qdrant-client>=1.1.7",  # Qdrant vector store client
+    "kornia",  # SIFT features
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 experimental_libs = []
 
 INSTALL_REQUIRES = minimal_requirement + integration_test_libs + udf_libs
 DEV_REQUIRES = (
@@ -114,14 +123,15 @@
     + test_libs
     + notebook_libs
     + benchmark_libs
     + doc_libs
     + database_libs
     + dist_libs
     + experimental_libs
+    + third_party_libs
 )
 
 EXTRA_REQUIRES = {"dev": DEV_REQUIRES}
 
 setup(
     name=NAME,
     version=VERSION,
```

### Comparing `evadb-0.2.3.post0/test/__init__.py` & `evadb-0.2.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/benchmark_tests/__init__.py` & `evadb-0.2.4/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/benchmark_tests/conftest.py` & `evadb-0.2.4/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.4/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/binder/__init__.py` & `evadb-0.2.4/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/binder/test_binder_utils.py` & `evadb-0.2.4/test/binder/test_binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/binder/test_statement_binder.py` & `evadb-0.2.4/test/binder/test_statement_binder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import unittest
 from unittest.mock import MagicMock, patch
 
 from eva.binder.binder_utils import BinderError
 from eva.binder.statement_binder import StatementBinder
 from eva.binder.statement_binder_context import StatementBinderContext
 from eva.catalog.catalog_manager import CatalogManager
-from eva.catalog.catalog_type import IndexType, NdArrayType
+from eva.catalog.catalog_type import NdArrayType
 from eva.parser.alias import Alias
 
 
 class StatementBinderTests(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -36,24 +36,24 @@
             binder._bind_tuple_expr(tve)
             col_alias = "{}.{}".format("table_alias", "col_name")
             mock.assert_called_once()
             self.assertEqual(tve.col_object, "col_obj")
             self.assertEqual(tve.col_alias, col_alias)
 
     @patch("eva.binder.statement_binder.bind_table_info")
-    def test_bind_tableref(self, mock_bind_tabe_info):
+    def test_bind_tableref(self, mock_bind_table_info):
         with patch.object(StatementBinderContext, "add_table_alias") as mock:
             binder = StatementBinder(StatementBinderContext())
             tableref = MagicMock()
             tableref.is_table_atom.return_value = True
             binder._bind_tableref(tableref)
             mock.assert_called_with(
                 tableref.alias.alias_name, tableref.table.table_name
             )
-            mock_bind_tabe_info.assert_called_once_with(tableref.table)
+            mock_bind_table_info.assert_called_once_with(tableref.table)
 
         with patch.object(StatementBinder, "bind") as mock_binder:
             with patch.object(
                 StatementBinderContext, "add_derived_table_alias"
             ) as mock_context:
                 binder = StatementBinder(StatementBinderContext())
                 tableref = MagicMock()
@@ -134,23 +134,23 @@
             name="func_expr", alias=Alias("func_expr"), output_col_aliases=[]
         )
         func_expr.name.lower.return_value = "func_expr"
         obj1 = MagicMock()
         obj1.name.lower.return_value = "out1"
         obj2 = MagicMock()
         obj2.name.lower.return_value = "out2"
-        func_ouput_objs = [obj1, obj2]
+        func_output_objs = [obj1, obj2]
         udf_obj = MagicMock()
         mock_get_name = mock_catalog().get_udf_catalog_entry_by_name = MagicMock()
         mock_get_name.return_value = udf_obj
 
         mock_get_udf_outputs = (
             mock_catalog().get_udf_io_catalog_output_entries
         ) = MagicMock()
-        mock_get_udf_outputs.return_value = func_ouput_objs
+        mock_get_udf_outputs.return_value = func_output_objs
         mock_load_udf_class_from_file.return_value.return_value = (
             "load_udf_class_from_file"
         )
         mock_get_file_checksum.return_value = udf_obj.checksum
 
         # Case 1 set output
         func_expr.output = "out1"
@@ -179,15 +179,15 @@
 
         mock_get_file_checksum.assert_called_with(udf_obj.impl_file_path)
         mock_get_name.assert_called_with(func_expr.name)
         mock_get_udf_outputs.assert_called_with(udf_obj)
         mock_load_udf_class_from_file.assert_called_with(
             udf_obj.impl_file_path, udf_obj.name
         )
-        self.assertEqual(func_expr.output_objs, func_ouput_objs)
+        self.assertEqual(func_expr.output_objs, func_output_objs)
         self.assertEqual(
             func_expr.alias,
             Alias(
                 "func_expr",
                 ["out1", "out2"],
             ),
         )
@@ -247,49 +247,30 @@
         class UnknownType:
             pass
 
         with self.assertRaises(NotImplementedError):
             binder = StatementBinder(StatementBinderContext())
             binder.bind(UnknownType())
 
-    @patch("eva.binder.statement_binder.sys")
-    def test_bind_with_python37(self, mock_sys):
-        mock_sys.version_info = (3, 8)
-        with patch.object(StatementBinderContext, "get_binded_column") as mock:
-            mock.return_value = ["table_alias", "col_obj"]
-            binder = StatementBinder(StatementBinderContext())
-            tve = MagicMock()
-            tve.col_name = "col_name"
-            binder._bind_tuple_expr(tve)
-            col_alias = "{}.{}".format("table_alias", "col_name")
-            mock.assert_called_once()
-            self.assertEqual(tve.col_object, "col_obj")
-            self.assertEqual(tve.col_alias, col_alias)
-
     def test_bind_create_index(self):
         with patch.object(StatementBinder, "bind"):
             binder = StatementBinder(StatementBinderContext())
             create_index_statement = MagicMock()
 
             with self.assertRaises(AssertionError):
                 binder._bind_create_index_statement(create_index_statement)
 
             create_index_statement.col_list = ["foo"]
-            create_index_statement.index_type = "bar"
-            with self.assertRaises(AssertionError):
-                binder._bind_create_index_statement(create_index_statement)
-
             udf_obj = MagicMock()
             output = MagicMock()
             udf_obj.outputs = [output]
 
             with patch.object(
                 CatalogManager, "get_udf_catalog_entry_by_name", return_value=udf_obj
             ):
-                create_index_statement.index_type = IndexType.HNSW
                 with self.assertRaises(AssertionError):
                     binder._bind_create_index_statement(create_index_statement)
                 output.array_type = NdArrayType.FLOAT32
                 with self.assertRaises(AssertionError):
                     binder._bind_create_index_statement(create_index_statement)
                 output.array_dimensions = [1, 100]
                 binder._bind_create_index_statement(create_index_statement)
```

### Comparing `evadb-0.2.3.post0/test/binder/test_statement_binder_context.py` & `evadb-0.2.4/test/binder/test_statement_binder_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         # key exists
         ctx = StatementBinderContext()
         ctx._table_alias_map["alias"] = "table_obj"
         result = ctx._check_table_alias_map("alias", "col_name")
         mock_get_column_object.assert_called_once_with("table_obj", "col_name")
         self.assertEqual(result, "catalog_value")
 
-        # key does not exixt
+        # key does not exist
         mock_get_column_object.reset_mock()
         ctx = StatementBinderContext()
         result = ctx._check_table_alias_map("alias", "col_name")
         mock_get_column_object.assert_not_called()
         self.assertEqual(result, None)
 
     def test_check_derived_table_alias_map(self):
@@ -140,15 +140,16 @@
         obj2 = MagicMock()
         col_map = {"col1": obj1, "col2": obj2}
         ctx._derived_table_alias_map["alias"] = col_map
         result = ctx._check_derived_table_alias_map("alias", "col1")
         self.assertEqual(result, obj1)
         result = ctx._check_derived_table_alias_map("alias", "col2")
         self.assertEqual(result, obj2)
-        # key does not exixt
+
+        # key does not exist
         ctx = StatementBinderContext()
         result = ctx._check_derived_table_alias_map("alias", "col3")
         self.assertEqual(result, None)
 
     def test_search_all_alias_maps(self):
         ctx = StatementBinderContext()
         check_table_map = ctx._check_table_alias_map = MagicMock()
```

### Comparing `evadb-0.2.3.post0/test/catalog/__init__.py` & `evadb-0.2.4/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/models/__init__.py` & `evadb-0.2.4/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/models/test_models.py` & `evadb-0.2.4/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/services/__init__.py` & `evadb-0.2.4/test/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/services/test_column_catalog_service.py` & `evadb-0.2.4/test/catalog/services/test_column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/services/test_index_catalog_service.py` & `evadb-0.2.4/test/catalog/services/test_index_catalog_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from unittest import TestCase
 
 import pytest
 from mock import MagicMock, patch
 from sqlalchemy.orm.exc import NoResultFound
 
 from eva.catalog.catalog_manager import CatalogManager
-from eva.catalog.catalog_type import ColumnType, IndexType
+from eva.catalog.catalog_type import ColumnType, VectorStoreType
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
 from eva.catalog.services.index_catalog_service import IndexCatalogService
 
 INDEX_NAME = "name"
 INDEX_ID = 123
 
 
@@ -98,18 +98,20 @@
 
         self.assertEqual(service.get_all_entries(), [])
 
     def test_index_get_all_entries(self):
         CatalogManager().reset()
         INDEX_NAME = "name"
         INDEX_URL = "file1"
-        INDEX_TYPE = IndexType.HNSW
+        VECTOR_STORE_TYPE = VectorStoreType.FAISS
         FEAT_COLUMN = ColumnCatalogEntry("abc", ColumnType.INTEGER)
 
         service = IndexCatalogService()
 
-        service.insert_entry(INDEX_NAME, INDEX_URL, INDEX_TYPE, FEAT_COLUMN, "sig")
+        service.insert_entry(
+            INDEX_NAME, INDEX_URL, VECTOR_STORE_TYPE, FEAT_COLUMN, "sig"
+        )
 
         output = service.get_all_entries()
         self.assertEqual(len(output), 1)
 
         service.delete_entry_by_name(INDEX_NAME)
```

### Comparing `evadb-0.2.3.post0/test/catalog/services/test_table_catalog_service.py` & `evadb-0.2.4/test/catalog/services/test_table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/services/test_udf_catalog_service.py` & `evadb-0.2.4/test/catalog/services/test_udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/services/test_udf_cost_catalog_service.py` & `evadb-0.2.4/test/catalog/services/test_udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/services/test_udf_io_catalog_service.py` & `evadb-0.2.4/test/catalog/services/test_udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/test_catalog_manager.py` & `evadb-0.2.4/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/test_column_type.py` & `evadb-0.2.4/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/catalog/test_sqlalchemy.py` & `evadb-0.2.4/test/catalog/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/configuration/__init__.py` & `evadb-0.2.4/test/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/configuration/test_bootstrap_environment.py` & `evadb-0.2.4/test/configuration/test_bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/configuration/test_configuration_manager.py` & `evadb-0.2.4/test/configuration/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/__init__.py` & `evadb-0.2.4/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_abstract_executor.py` & `evadb-0.2.4/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_create_mat_executor.py` & `evadb-0.2.4/test/executor/test_create_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_create_udf_executor.py` & `evadb-0.2.4/test/executor/test_create_udf_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,14 @@
                 "impl_path": impl_path,
                 "udf_type": "classification",
             },
         )
 
         create_udf_executor = CreateUDFExecutor(plan)
         # check a string in the error message
-        with self.assertRaises(RuntimeError) as ce:
+        with self.assertRaises(RuntimeError) as exc:
             next(create_udf_executor.exec())
         self.assertIn(
-            "Error creating UDF, input/output definition incorrect:", str(ce.exception)
+            "Error creating UDF, input/output definition incorrect:", str(exc.exception)
         )
 
         catalog_instance.insert_udf_catalog_entry.assert_not_called()
```

### Comparing `evadb-0.2.3.post0/test/executor/test_execution_context.py` & `evadb-0.2.4/test/executor/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_executor_utils.py` & `evadb-0.2.4/test/executor/test_executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_limit_executor.py` & `evadb-0.2.4/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_load_executor.py` & `evadb-0.2.4/test/executor/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_orderby_executor.py` & `evadb-0.2.4/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_plan_executor.py` & `evadb-0.2.4/test/executor/test_plan_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from eva.plan_nodes.seq_scan_plan import SeqScanPlan
 from eva.plan_nodes.storage_plan import StoragePlan
 
 
 class PlanExecutorTest(unittest.TestCase):
     def test_tree_structure_for_build_execution_tree(self):
         """
-            Build an Abastract Plan with nodes:
+            Build an Abstract Plan with nodes:
          ß               root
                       /  |  \
                     c1   c2 c3
                     /
                    c1_1
         """
 
@@ -238,28 +238,28 @@
         mock_build.return_value = tree
         actual = list(PlanExecutor(None).execute_plan())
         tree.exec.assert_called_once()
         mock_build.assert_called_once_with(None)
         mock_clean.assert_called_once()
         self.assertEqual(actual, [])
 
-    @unittest.skip("disk_based_storage_depricated")
+    @unittest.skip("disk_based_storage_deprecated")
     @patch("eva.executor.disk_based_storage_executor.Loader")
     def test_should_return_the_new_path_after_execution(self, mock_class):
-        class_instatnce = mock_class.return_value
+        class_instance = mock_class.return_value
 
         dummy_expr = type(
             "dummy_expr", (), {"evaluate": lambda x=None: [True, False, True]}
         )
 
         # Build plan tree
         video = TableCatalogEntry("dataset", "dummy.avi", table_type=TableType.VIDEO)
         batch_1 = Batch(pd.DataFrame({"data": [1, 2, 3]}))
         batch_2 = Batch(pd.DataFrame({"data": [4, 5, 6]}))
-        class_instatnce.load.return_value = map(lambda x: x, [batch_1, batch_2])
+        class_instance.load.return_value = map(lambda x: x, [batch_1, batch_2])
 
         storage_plan = StoragePlan(video, batch_mem_size=3000)
         seq_scan = SeqScanPlan(predicate=dummy_expr, column_ids=[])
         seq_scan.append_child(storage_plan)
 
         # Execute the plan
         executor = PlanExecutor(seq_scan)
```

### Comparing `evadb-0.2.3.post0/test/executor/test_pp_executor.py` & `evadb-0.2.4/test/executor/test_pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_sample_executor.py` & `evadb-0.2.4/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/test_seq_scan_executor.py` & `evadb-0.2.4/test/executor/test_seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/executor/utils.py` & `evadb-0.2.4/test/models/catalog/test_frame_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List
+import unittest
 
-from eva.models.storage.batch import Batch
+from eva.models.catalog.frame_info import FrameInfo
+from eva.models.catalog.properties import ColorSpace
 
 
-class DummyExecutor:
-    def __init__(self, batch_list: List[Batch]):
-        self.batch_list = batch_list
-
-    def exec(self):
-        for batch in self.batch_list:
-            yield batch
+class FrameInfoTest(unittest.TestCase):
+    def test_frame_info_equality(self):
+        info1 = FrameInfo(
+            height=250, width=250, channels=3, color_space=ColorSpace.GRAY
+        )
+        info2 = FrameInfo(250, 250, 3, color_space=ColorSpace.GRAY)
+        self.assertEqual(info1, info2)
```

### Comparing `evadb-0.2.3.post0/test/expression/__init__.py` & `evadb-0.2.4/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_abstract_expression.py` & `evadb-0.2.4/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_aggregation.py` & `evadb-0.2.4/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_arithmetic.py` & `evadb-0.2.4/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_comparison.py` & `evadb-0.2.4/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_expression_tree.py` & `evadb-0.2.4/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_expression_utils.py` & `evadb-0.2.4/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_function_expression.py` & `evadb-0.2.4/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/expression/test_logical.py` & `evadb-0.2.4/test/expression/test_logical.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/__init__.py` & `evadb-0.2.4/test/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_array_count.py` & `evadb-0.2.4/test/integration_tests/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_chatgpt.py` & `evadb-0.2.4/test/integration_tests/test_chatgpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.4/test/integration_tests/test_create_index_executor.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,44 +8,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 import unittest
 from pathlib import Path
 from test.util import load_udfs_for_testing
 
 import faiss
 import numpy as np
 import pandas as pd
 import pytest
-from mock import patch
 
 from eva.catalog.catalog_manager import CatalogManager
-from eva.catalog.catalog_type import ColumnType, IndexType, NdArrayType, TableType
-from eva.catalog.catalog_utils import xform_column_definitions_to_catalog_entries
-from eva.catalog.sql_config import IDENTIFIER_COLUMN
+from eva.catalog.catalog_type import VectorStoreType
 from eva.configuration.configuration_manager import ConfigurationManager
-from eva.executor.executor_utils import ExecutorError
 from eva.models.storage.batch import Batch
-from eva.parser.create_statement import ColumnDefinition
 from eva.server.command_handler import execute_query_fetch_all
 from eva.storage.storage_engine import StorageEngine
-from eva.utils.generic_utils import generate_file_path
 
 
 @pytest.mark.notparallel
 class CreateIndexTest(unittest.TestCase):
     def _index_save_path(self):
         return str(
             Path(ConfigurationManager().get_value("storage", "index_dir"))
-            / Path("{}_{}.index".format("HNSW", "testCreateIndexName"))
+            / Path("{}_{}.index".format("FAISS", "testCreateIndexName"))
         )
 
     @classmethod
     def setUpClass(cls):
         # Bootstrap configuration manager.
         ConfigurationManager()
 
@@ -59,79 +52,67 @@
         feat3 = np.array([[200, 200, 200]]).astype(np.float32)
 
         input1 = np.array([[0, 0, 0]]).astype(np.uint8)
         input2 = np.array([[100, 100, 100]]).astype(np.uint8)
         input3 = np.array([[200, 200, 200]]).astype(np.uint8)
 
         # Create table.
-        feat_col_list = [
-            ColumnDefinition("feat", ColumnType.NDARRAY, NdArrayType.FLOAT32, (1, 3)),
-        ]
-        feat_col_entries = xform_column_definitions_to_catalog_entries(feat_col_list)
-
-        input_col_list = [
-            ColumnDefinition("input", ColumnType.NDARRAY, NdArrayType.UINT8, (1, 3)),
-        ]
-        input_col_entries = xform_column_definitions_to_catalog_entries(input_col_list)
-
-        feat_tb_entry = CatalogManager().insert_table_catalog_entry(
-            "testCreateIndexFeatTable",
-            str(generate_file_path("testCreateIndexFeatTable")),
-            feat_col_entries,
-            identifier_column=IDENTIFIER_COLUMN,
-            table_type=TableType.STRUCTURED_DATA,
+        execute_query_fetch_all(
+            """create table if not exists testCreateIndexFeatTable (
+                feat NDARRAY FLOAT32(1,3)
+            );"""
+        )
+        execute_query_fetch_all(
+            """create table if not exists testCreateIndexInputTable (
+                input NDARRAY UINT8(1,3)
+            );"""
         )
-        storage_engine = StorageEngine.factory(feat_tb_entry)
-        storage_engine.create(feat_tb_entry)
-
-        input_tb_entry = CatalogManager().insert_table_catalog_entry(
-            "testCreateIndexInputTable",
-            str(generate_file_path("testCreateIndexInputTable")),
-            input_col_entries,
-            identifier_column=IDENTIFIER_COLUMN,
-            table_type=TableType.STRUCTURED_DATA,
-        )
-        storage_engine = StorageEngine.factory(input_tb_entry)
-        storage_engine.create(input_tb_entry)
 
         # Create pandas dataframe.
         feat_batch_data = Batch(
             pd.DataFrame(
                 data={
                     "feat": [feat1, feat2, feat3],
                 }
             )
         )
+        feat_tb_entry = CatalogManager().get_table_catalog_entry(
+            "testCreateIndexFeatTable"
+        )
+        storage_engine = StorageEngine.factory(feat_tb_entry)
         storage_engine.write(feat_tb_entry, feat_batch_data)
 
         input_batch_data = Batch(
             pd.DataFrame(
                 data={
                     "input": [input1, input2, input3],
                 }
             )
         )
+        input_tb_entry = CatalogManager().get_table_catalog_entry(
+            "testCreateIndexInputTable"
+        )
         storage_engine.write(input_tb_entry, input_batch_data)
 
     @classmethod
     def tearDownClass(cls):
         query = "DROP TABLE testCreateIndexFeatTable;"
         execute_query_fetch_all(query)
         query = "DROP TABLE testCreateIndexInputTable;"
         execute_query_fetch_all(query)
 
-    def test_should_create_index(self):
-        query = "CREATE INDEX testCreateIndexName ON testCreateIndexFeatTable (feat) USING HNSW;"
+    def test_should_create_index_faiss(self):
+        query = "CREATE INDEX testCreateIndexName ON testCreateIndexFeatTable (feat) USING FAISS;"
         execute_query_fetch_all(query)
 
         # Test index catalog.
         index_catalog_entry = CatalogManager().get_index_catalog_entry_by_name(
             "testCreateIndexName"
         )
-        self.assertEqual(index_catalog_entry.type, IndexType.HNSW)
+        self.assertEqual(index_catalog_entry.type, VectorStoreType.FAISS)
         self.assertEqual(
             index_catalog_entry.save_file_path,
             self._index_save_path(),
         )
         self.assertEqual(
             index_catalog_entry.udf_signature,
             None,
@@ -150,34 +131,23 @@
         distance, row_id = index.search(np.array([[0, 0, 0]]).astype(np.float32), 1)
         self.assertEqual(distance[0][0], 0)
         self.assertEqual(row_id[0][0], 1)
 
         # Cleanup.
         CatalogManager().drop_index_catalog_entry("testCreateIndexName")
 
-    @patch("eva.executor.create_index_executor.faiss")
-    def test_should_cleanup_when_exception(self, faiss_mock):
-        faiss_mock.write_index.side_effect = Exception("Test exception.")
-
-        query = "CREATE INDEX testCreateIndexName ON testCreateIndexFeatTable (feat) USING HNSW;"
-        with self.assertRaises(ExecutorError):
-            execute_query_fetch_all(query)
-
-        # Check faulty index is not persisted on the disk
-        self.assertFalse(os.path.exists(self._index_save_path()))
-
     def test_should_create_index_with_udf(self):
-        query = "CREATE INDEX testCreateIndexName ON testCreateIndexInputTable (DummyFeatureExtractor(input)) USING HNSW;"
+        query = "CREATE INDEX testCreateIndexName ON testCreateIndexInputTable (DummyFeatureExtractor(input)) USING FAISS;"
         execute_query_fetch_all(query)
 
         # Test index udf signature.
         index_catalog_entry = CatalogManager().get_index_catalog_entry_by_name(
             "testCreateIndexName"
         )
-        self.assertEqual(index_catalog_entry.type, IndexType.HNSW)
+        self.assertEqual(index_catalog_entry.type, VectorStoreType.FAISS)
         self.assertEqual(
             index_catalog_entry.save_file_path,
             self._index_save_path(),
         )
 
         # Test referenced column.
         input_table_entry = CatalogManager().get_table_catalog_entry(
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.4/test/optimizer/test_optimizer_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 
-from eva.executor.executor_utils import ExecutorError
-from eva.server.command_handler import execute_query_fetch_all
+from mock import MagicMock
 
+from eva.optimizer.cost_model import CostModel
+from eva.optimizer.optimizer_context import OptimizerContext
 
-class CreateTableTest(unittest.TestCase):
-    @classmethod
-    def setUpClass(cls):
-        pass
 
-    @classmethod
-    def tearDownClass(cls):
-        pass
+class TestOptimizerContext(unittest.TestCase):
+    def test_add_root(self):
+        fake_opr = MagicMock()
+        fake_opr.children = []
 
-    def test_currently_cannot_create_boolean_table(self):
-        query = """ CREATE TABLE BooleanTable( A BOOLEAN);"""
-
-        with self.assertRaises(ExecutorError):
-            execute_query_fetch_all(query)
+        opt_ctxt = OptimizerContext(CostModel())
+        opt_ctxt.add_opr_to_group(fake_opr)
+        self.assertEqual(len(opt_ctxt.memo.group_exprs), 1)
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_delete_executor.py` & `evadb-0.2.4/test/integration_tests/test_delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_drop_executor.py` & `evadb-0.2.4/test/integration_tests/test_drop_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     # integration test
     def test_should_drop_table(self):
         catalog_manager = CatalogManager()
         query = f"""LOAD VIDEO '{self.video_file_path}' INTO MyVideo;"""
         execute_query_fetch_all(query)
 
-        # catalog should contain vidoe table and the metedata table
+        # catalog should contain video table and the metadata table
         table_catalog_entry = catalog_manager.get_table_catalog_entry("MyVideo")
         video_dir = table_catalog_entry.file_url
         self.assertFalse(table_catalog_entry is None)
         column_objects = catalog_manager.get_column_catalog_entries_by_table(
             table_catalog_entry
         )
         # no of column objects should equal what we have defined plus one for row_id
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.2.4/test/integration_tests/test_error_handling_with_ray.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_explain_executor.py` & `evadb-0.2.4/test/integration_tests/test_explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.4/test/integration_tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.2.4/test/integration_tests/test_huggingface_udfs.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_insert_executor.py` & `evadb-0.2.4/test/integration_tests/test_insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_like.py` & `evadb-0.2.4/test/integration_tests/test_like.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_load_executor.py` & `evadb-0.2.4/test/integration_tests/test_load_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
 
         drop_query = "DROP TABLE IF EXISTS MyLargeScaleImages;"
         execute_query_fetch_all(drop_query)
 
         # Clean up large scale image directory.
         shutil.rmtree(large_scale_image_files_path)
 
-    def test_parallel_load_should_raise_exeception(self):
+    def test_parallel_load_should_raise_exception(self):
         # Create images.
         large_scale_image_files_path = create_large_scale_image_dataset(
             mp.cpu_count() * 10
         )
 
         # Corrupt an image.
         with open(os.path.join(large_scale_image_files_path, "img0.jpg"), "w") as f:
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_mat_executor.py` & `evadb-0.2.4/test/integration_tests/test_mat_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,14 +117,16 @@
 
         self.assertEqual(len(actual_batch), 5)
         # non-trivial test case
         res = actual_batch.frames
         for idx in res.index:
             self.assertTrue("car" in res["uadtrac_fastrcnn.labels"][idx])
 
+        execute_query_fetch_all("DROP TABLE IF EXISTS uadtrac_fastRCNN;")
+
     @pytest.mark.torchtest
     def test_should_mat_view_with_fastrcnn_lateral_join(self):
         select_query = (
             "SELECT id, label, bbox FROM UATRAC JOIN LATERAL "
             "Yolo(data) AS T(label, bbox, score) WHERE id < 5;"
         )
         query = (
@@ -138,7 +140,9 @@
         actual_batch.sort()
 
         self.assertEqual(len(actual_batch), 5)
         # non-trivial test case
         res = actual_batch.frames
         for idx in res.index:
             self.assertTrue("car" in res["uadtrac_fastrcnn_new.label"][idx])
+
+        execute_query_fetch_all("DROP TABLE IF EXISTS uadtrac_fastRCNN;")
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_open.py` & `evadb-0.2.4/test/integration_tests/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.4/test/integration_tests/test_optimizer_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from test.util import get_physical_query_plan, load_udfs_for_testing, shutdown_ray
 
+import numpy as np
+import pandas as pd
 import pytest
 from mock import MagicMock, patch
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.configuration.constants import EVA_ROOT_DIR
 from eva.expression.comparison_expression import ComparisonExpression
+from eva.models.storage.batch import Batch
 from eva.optimizer.plan_generator import PlanGenerator
 from eva.optimizer.rules.rules import (
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
     XformLateralJoinToLinearFlow,
 )
@@ -51,15 +54,26 @@
 
     @classmethod
     def tearDownClass(cls):
         shutdown_ray()
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     @patch("eva.expression.function_expression.FunctionExpression.evaluate")
-    def test_should_benefit_from_pushdown(self, evaluate_mock):
+    @patch("eva.models.storage.batch.Batch.merge_column_wise")
+    def test_should_benefit_from_pushdown(self, merge_mock, evaluate_mock):
+        # added to mock away the
+        evaluate_mock.return_value = Batch(
+            pd.DataFrame(
+                {
+                    "obj.labels": ["car"],
+                    "obj.bboxes": [np.array([1, 2, 3, 4])],
+                    "obj.scores": [0.8],
+                }
+            )
+        )
         query = """SELECT id, obj.labels
                   FROM MyVideo JOIN LATERAL
                     FastRCNNObjectDetector(data) AS obj(labels, bboxes, scores)
                   WHERE id < 2;"""
 
         time_with_rule = Timer()
         result_with_rule = None
@@ -206,21 +220,21 @@
             if name == "DummyMultiObjectDetector":
                 return MagicMock(cost=10)
             else:
                 return MagicMock(cost=5)
 
         mock.side_effect = side_effect_func
 
-        chepeast_pred = "id<10"
+        cheapest_pred = "id<10"
         cheap_pred = "DummyObjectDetector(data).label = ['person']"
         costly_pred = "DummyMultiObjectDetector(data).labels @> ['person']"
 
         query = (
             f"SELECT id FROM MyVideo WHERE {costly_pred} AND {cheap_pred} AND "
-            f"{chepeast_pred};"
+            f"{cheapest_pred};"
         )
 
         plan = get_physical_query_plan(query)
         predicate_plans = list(plan.find_all(PredicatePlan))
         self.assertEqual(len(predicate_plans), 1)
 
         left = predicate_plans[0].predicate.children[0]
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_pytorch.py` & `evadb-0.2.4/test/integration_tests/test_pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -241,17 +241,40 @@
         self.assertEqual(len(actual_batch), 5)
 
         # non-trivial test case for MNIST
         res = actual_batch.frames
         self.assertTrue(res["ocrextractor.labels"][0][0] == "4")
         self.assertTrue(res["ocrextractor.scores"][2][0] > 0.9)
 
+    @pytest.mark.torchtest
+    def test_should_run_extract_object(self):
+        select_query = """
+            SELECT id, T.iids, T.bboxes, T.scores, T.labels
+            FROM MyVideo JOIN LATERAL EXTRACT_OBJECT(data, Yolo, NorFairTracker)
+                AS T(iids, labels, bboxes, scores)
+            WHERE id < 30;
+            """
+        actual_batch = execute_query_fetch_all(select_query)
+        self.assertEqual(len(actual_batch), 30)
+
+        num_of_entries = actual_batch.frames["T.iids"].apply(lambda x: len(x)).sum()
+
+        select_query = """
+            SELECT id, T.iid, T.bbox, T.score, T.label
+            FROM MyVideo JOIN LATERAL
+                UNNEST(EXTRACT_OBJECT(data, Yolo, NorFairTracker)) AS T(iid, label, bbox, score)
+            WHERE id < 30;
+            """
+        actual_batch = execute_query_fetch_all(select_query)
+        # do some more meaningful check
+        self.assertEqual(len(actual_batch), num_of_entries)
+
     def test_check_unnest_with_predicate_on_yolo(self):
         query = """SELECT id, Yolo.label, Yolo.bbox, Yolo.score
                   FROM MyVideo
                   JOIN LATERAL UNNEST(Yolo(data)) AS Yolo(label, bbox, score)
                   WHERE Yolo.label = 'car' AND id < 2;"""
 
         actual_batch = execute_query_fetch_all(query)
 
-        # due to unnest the number of returned tuples should be atleast > 10
+        # due to unnest the number of returned tuples should be at least > 10
         self.assertTrue(len(actual_batch) > 2)
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_rename_executor.py` & `evadb-0.2.4/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_reuse.py` & `evadb-0.2.4/test/integration_tests/test_reuse.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,19 @@
             LATERAL HFObjectDetector(data) AS Obj(score, label, bbox) WHERE id < 5;"""
         select_query2 = """SELECT id, label FROM DETRAC JOIN
             LATERAL HFObjectDetector(data) AS Obj(score, label, bbox) WHERE id < 15;"""
 
         batches, exec_times = self._reuse_experiment([select_query1, select_query2])
         self._verify_reuse_correctness(select_query2, batches[1])
 
-    def test_reuse_in_with_multiple_occurences(self):
+    def test_reuse_in_with_multiple_occurrences(self):
         select_query1 = """SELECT id, label FROM DETRAC JOIN
             LATERAL HFObjectDetector(data) AS Obj(score, label, bbox) WHERE id < 10;"""
 
-        # multiple occurences of the same function expression
+        # multiple occurrences of the same function expression
         select_query2 = """SELECT id, HFObjectDetector(data).label FROM DETRAC JOIN
             LATERAL HFObjectDetector(data) AS Obj(score, label, bbox) WHERE id < 5;"""
 
         batches, exec_times = self._reuse_experiment([select_query1, select_query2])
 
         self._verify_reuse_correctness(select_query2, batches[1])
 
@@ -156,24 +156,33 @@
         self._verify_reuse_correctness(query2, batches[1])
         # reuse should be faster than no reuse
         self.assertGreater(exec_times[0], exec_times[1])
 
     def test_reuse_filter_with_project(self):
         project_query = """
             SELECT id, Yolo(data).labels FROM DETRAC WHERE id < 5;"""
-
         select_query = """
             SELECT id FROM DETRAC
             WHERE ArrayCount(Yolo(data).labels, 'car') > 3 AND id < 5;"""
-
         batches, exec_times = self._reuse_experiment([project_query, select_query])
         self._verify_reuse_correctness(select_query, batches[1])
         # reuse should be faster than no reuse
         self.assertGreater(exec_times[0], exec_times[1])
 
+    def test_reuse_in_extract_object(self):
+        select_query = """
+            SELECT id, T.iids, T.bboxes, T.scores, T.labels
+            FROM DETRAC JOIN LATERAL EXTRACT_OBJECT(data, Yolo, NorFairTracker)
+                AS T(iids, labels, bboxes, scores)
+            WHERE id < 30;
+            """
+        batches, exec_times = self._reuse_experiment([select_query, select_query])
+        self._verify_reuse_correctness(select_query, batches[1])
+        self.assertGreater(exec_times[0], exec_times[1])
+
     @windows_skip_marker
     def test_reuse_after_server_shutdown(self):
         select_query = """SELECT id, label FROM DETRAC JOIN
             LATERAL Yolo(data) AS Obj(label, bbox, conf) WHERE id < 4;"""
         execute_query_fetch_all(select_query)
 
         # Stop and restart server
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.4/test/integration_tests/test_s3_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_select_executor.py` & `evadb-0.2.4/test/integration_tests/test_select_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.4/test/integration_tests/test_show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_similarity.py` & `evadb-0.2.4/test/integration_tests/test_similarity.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import os
 import unittest
+from test.markers import ray_skip_marker
 from test.util import create_sample_image, load_udfs_for_testing, shutdown_ray
 
+import cv2
 import numpy as np
 import pandas as pd
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
+from eva.configuration.configuration_manager import ConfigurationManager
 from eva.models.storage.batch import Batch
 from eva.server.command_handler import execute_query_fetch_all
 from eva.storage.storage_engine import StorageEngine
 
 
 @pytest.mark.notparallel
 class SimilarityTests(unittest.TestCase):
@@ -87,23 +91,37 @@
                                 ),
                                 "dummy": i,
                             }
                         ]
                     )
                 ),
             )
+
+            # Create an actual image dataset.
+            img_save_path = os.path.join(
+                ConfigurationManager().get_value("storage", "tmp_dir"),
+                f"test_similar_img{i}.jpg",
+            )
+            cv2.imwrite(img_save_path, base_img)
+            load_image_query = (
+                f"LOAD IMAGE '{img_save_path}' INTO testSimilarityImageDataset;"
+            )
+            execute_query_fetch_all(load_image_query)
+
             base_img -= 1
 
     def tearDown(self):
         shutdown_ray()
 
         drop_table_query = "DROP TABLE testSimilarityTable;"
         execute_query_fetch_all(drop_table_query)
         drop_table_query = "DROP TABLE testSimilarityFeatureTable;"
         execute_query_fetch_all(drop_table_query)
+        drop_table_query = "DROP TABLE IF EXISTS testSimilarityImageDataset;"
+        execute_query_fetch_all(drop_table_query)
 
     def test_similarity_should_work_in_order(self):
         ###############################################
         # Test case runs with UDF on raw input table. #
         ###############################################
 
         # Top 1 - assume table contains base data_col.
@@ -181,15 +199,15 @@
         ].to_numpy()[1]
         self.assertTrue(np.array_equal(actual_open, base_img + 1))
         # actual_distance = actual_batch.frames["similarity.distance"].to_numpy()[0]
         # self.assertEqual(actual_distance, 0)
         # actual_distance = actual_batch.frames["similarity.distance"].to_numpy()[1]
         # self.assertEqual(actual_distance, 27)
 
-    def test_should_do_faiss_index_scan(self):
+    def test_should_do_vector_index_scan(self):
         ###########################################
         # Test case runs on feature vector table. #
         ###########################################
 
         # Execution without index scan.
         select_query = """SELECT feature_col FROM testSimilarityFeatureTable
                             ORDER BY Similarity(DummyFeatureExtractor(Open("{}")), feature_col)
@@ -197,24 +215,24 @@
             self.img_path
         )
         expected_batch = execute_query_fetch_all(select_query)
 
         # Execution with index scan.
         create_index_query = """CREATE INDEX testFaissIndexScanRewrite1
                                     ON testSimilarityFeatureTable (feature_col)
-                                    USING HNSW;"""
+                                    USING FAISS;"""
         execute_query_fetch_all(create_index_query)
         select_query = """SELECT feature_col FROM testSimilarityFeatureTable
                             ORDER BY Similarity(DummyFeatureExtractor(Open("{}")), feature_col)
                             LIMIT 3;""".format(
             self.img_path
         )
         explain_query = """EXPLAIN {}""".format(select_query)
         explain_batch = execute_query_fetch_all(explain_query)
-        self.assertTrue("FaissIndexScan" in explain_batch.frames[0][0])
+        self.assertTrue("VectorIndexScan" in explain_batch.frames[0][0])
         actual_batch = execute_query_fetch_all(select_query)
 
         self.assertEqual(len(actual_batch), 3)
         for i in range(3):
             self.assertTrue(
                 np.array_equal(
                     expected_batch.frames[
@@ -237,24 +255,24 @@
             self.img_path
         )
         expected_batch = execute_query_fetch_all(select_query)
 
         # Execution with index scan.
         create_index_query = """CREATE INDEX testFaissIndexScanRewrite2
                                     ON testSimilarityTable (DummyFeatureExtractor(data_col))
-                                    USING HNSW;"""
+                                    USING FAISS;"""
         execute_query_fetch_all(create_index_query)
         select_query = """SELECT data_col FROM testSimilarityTable
                             ORDER BY Similarity(DummyFeatureExtractor(Open("{}")), DummyFeatureExtractor(data_col))
                             LIMIT 3;""".format(
             self.img_path
         )
         explain_query = """EXPLAIN {}""".format(select_query)
         explain_batch = execute_query_fetch_all(explain_query)
-        self.assertTrue("FaissIndexScan" in explain_batch.frames[0][0])
+        self.assertTrue("VectorIndexScan" in explain_batch.frames[0][0])
         actual_batch = execute_query_fetch_all(select_query)
 
         self.assertEqual(len(actual_batch), 3)
         for i in range(3):
             self.assertTrue(
                 np.array_equal(
                     expected_batch.frames["testsimilaritytable.data_col"].to_numpy()[i],
@@ -262,19 +280,19 @@
                 )
             )
 
         # Cleanup
         CatalogManager().drop_index_catalog_entry("testFaissIndexScanRewrite1")
         CatalogManager().drop_index_catalog_entry("testFaissIndexScanRewrite2")
 
-    def test_should_not_do_faiss_index_scan_with_predicate(self):
+    def test_should_not_do_vector_index_scan_with_predicate(self):
         # Execution with index scan.
         create_index_query = """CREATE INDEX testFaissIndexScanRewrite
                                     ON testSimilarityTable (DummyFeatureExtractor(data_col))
-                                    USING HNSW;"""
+                                    USING FAISS;"""
         execute_query_fetch_all(create_index_query)
 
         explain_query = """
             EXPLAIN
                 SELECT data_col FROM testSimilarityTable WHERE dummy = 0
                   ORDER BY Similarity(DummyFeatureExtractor(Open("{}")), DummyFeatureExtractor(data_col))
                   LIMIT 3;
@@ -284,7 +302,40 @@
         batch = execute_query_fetch_all(explain_query)
 
         # Index scan should not be used.
         self.assertFalse("FaissIndexScan" in batch.frames[0][0])
 
         # Cleanup
         CatalogManager().drop_index_catalog_entry("testFaissIndexScanRewrite")
+
+    def test_end_to_end_index_scan_should_work_correctly_on_image_dataset(self):
+        create_index_query = """CREATE INDEX testFaissIndexImageDataset
+                                    ON testSimilarityImageDataset (DummyFeatureExtractor(data))
+                                    USING FAISS;"""
+        execute_query_fetch_all(create_index_query)
+        select_query = """SELECT _row_id FROM testSimilarityImageDataset
+                            ORDER BY Similarity(DummyFeatureExtractor(Open("{}")), DummyFeatureExtractor(data))
+                            LIMIT 1;""".format(
+            self.img_path
+        )
+        res_batch = execute_query_fetch_all(select_query)
+        self.assertEqual(res_batch.frames["testsimilarityimagedataset._row_id"][0], 5)
+
+    @ray_skip_marker
+    def test_end_to_end_index_scan_should_work_correctly_on_image_dataset_qdrant(self):
+        create_index_query = """CREATE INDEX testFaissIndexImageDataset
+                                    ON testSimilarityImageDataset (DummyFeatureExtractor(data))
+                                    USING QDRANT;"""
+        execute_query_fetch_all(create_index_query)
+        select_query = """SELECT _row_id FROM testSimilarityImageDataset
+                            ORDER BY Similarity(DummyFeatureExtractor(Open("{}")), DummyFeatureExtractor(data))
+                            LIMIT 1;""".format(
+            self.img_path
+        )
+
+        """|__ ProjectPlan
+            |__ VectorIndexScanPlan
+                |__ SeqScanPlan
+                    |__ StoragePlan"""
+
+        res_batch = execute_query_fetch_all(select_query)
+        self.assertEqual(res_batch.frames["testsimilarityimagedataset._row_id"][0], 5)
```

### Comparing `evadb-0.2.3.post0/test/integration_tests/test_udf_executor.py` & `evadb-0.2.4/test/integration_tests/test_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/markers.py` & `evadb-0.2.4/test/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 
 memory_skip_marker = pytest.mark.skipif(
     sys.platform == "linux", reason="Test case consumes too much memory"
 )
 
 ray_skip_marker = pytest.mark.skipif(
     ConfigurationManager().get_value("experimental", "ray"),
-    reason="Only test for ray execution.",
+    reason="Skip test for ray execution.",
 )
 
+
 duplicate_skip_marker = pytest.mark.skipif(
     sys.platform == "linux",
     reason="Test case is duplicate. Disabling to speed up test suite",
 )
 
 ocr_skip_marker = pytest.mark.skipif(
     sys.platform == "linux",
```

### Comparing `evadb-0.2.3.post0/test/models/__init__.py` & `evadb-0.2.4/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/models/catalog/__init__.py` & `evadb-0.2.4/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/models/storage/__init__.py` & `evadb-0.2.4/test/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/models/storage/test_batch.py` & `evadb-0.2.4/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/__init__.py` & `evadb-0.2.4/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/rules/__init__.py` & `evadb-0.2.4/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/rules/test_rules.py` & `evadb-0.2.4/test/optimizer/rules/test_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,28 +35,27 @@
     LogicalJoin,
     LogicalSample,
 )
 from eva.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CacheFunctionExpressionInFilter,
     CacheFunctionExpressionInProject,
-    CombineSimilarityOrderByAndLimitToFaissIndexScan,
+    CombineSimilarityOrderByAndLimitToVectorIndexScan,
     EmbedFilterIntoGet,
     EmbedSampleIntoGet,
     LogicalApplyAndMergeToPhysical,
-    LogicalCreateIndexToFaiss,
+    LogicalCreateIndexToVectorIndex,
     LogicalCreateMaterializedViewToPhysical,
     LogicalCreateToPhysical,
     LogicalCreateUDFToPhysical,
     LogicalDeleteToPhysical,
     LogicalDerivedGetToPhysical,
     LogicalDropToPhysical,
     LogicalDropUDFToPhysical,
     LogicalExplainToPhysical,
-    LogicalFaissIndexScanToPhysical,
     LogicalFilterToPhysical,
     LogicalFunctionScanToPhysical,
 )
 from eva.optimizer.rules.rules import (
     LogicalGetToSeqScan as SequentialLogicalGetToSeqScan,
 )
 from eva.optimizer.rules.rules import (
@@ -73,20 +72,22 @@
 from eva.optimizer.rules.rules import (
     LogicalProjectToPhysical as SequentialLogicalProjectToPhysical,
 )
 from eva.optimizer.rules.rules import (
     LogicalRenameToPhysical,
     LogicalShowToPhysical,
     LogicalUnionToPhysical,
+    LogicalVectorIndexScanToPhysical,
     Promise,
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
     Rule,
     RuleType,
+    XformExtractObjectToLinearFlow,
     XformLateralJoinToLinearFlow,
 )
 from eva.optimizer.rules.rules_manager import RulesManager, disable_rules
 from eva.parser.types import JoinType
 from eva.server.command_handler import execute_query_fetch_all
 
 
@@ -109,20 +110,21 @@
         rewrite_promises = [
             Promise.LOGICAL_INNER_JOIN_COMMUTATIVITY,
             Promise.EMBED_FILTER_INTO_GET,
             Promise.EMBED_SAMPLE_INTO_GET,
             Promise.XFORM_LATERAL_JOIN_TO_LINEAR_FLOW,
             Promise.PUSHDOWN_FILTER_THROUGH_JOIN,
             Promise.PUSHDOWN_FILTER_THROUGH_APPLY_AND_MERGE,
-            Promise.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_FAISS_INDEX_SCAN,
+            Promise.COMBINE_SIMILARITY_ORDERBY_AND_LIMIT_TO_VECTOR_INDEX_SCAN,
             Promise.REORDER_PREDICATES,
+            Promise.XFORM_EXTRACT_OBJECT_TO_LINEAR_FLOW,
         ]
 
         for promise in rewrite_promises:
-            self.assertTrue(promise > Promise.IMPLEMENTATION_DELIMETER)
+            self.assertTrue(promise > Promise.IMPLEMENTATION_DELIMITER)
 
         # Promise of implementation rules should be lesser than rewrite rules
         implementation_promises = [
             Promise.LOGICAL_EXCHANGE_TO_PHYSICAL,
             Promise.LOGICAL_UNION_TO_PHYSICAL,
             Promise.LOGICAL_MATERIALIZED_VIEW_TO_PHYSICAL,
             Promise.LOGICAL_GROUPBY_TO_PHYSICAL,
@@ -143,40 +145,41 @@
             Promise.LOGICAL_JOIN_TO_PHYSICAL_NESTED_LOOP_JOIN,
             Promise.LOGICAL_FUNCTION_SCAN_TO_PHYSICAL,
             Promise.LOGICAL_FILTER_TO_PHYSICAL,
             Promise.LOGICAL_PROJECT_TO_PHYSICAL,
             Promise.LOGICAL_SHOW_TO_PHYSICAL,
             Promise.LOGICAL_DROP_UDF_TO_PHYSICAL,
             Promise.LOGICAL_EXPLAIN_TO_PHYSICAL,
-            Promise.LOGICAL_CREATE_INDEX_TO_FAISS,
+            Promise.LOGICAL_CREATE_INDEX_TO_VECTOR_INDEX,
             Promise.LOGICAL_APPLY_AND_MERGE_TO_PHYSICAL,
-            Promise.LOGICAL_FAISS_INDEX_SCAN_TO_PHYSICAL,
+            Promise.LOGICAL_VECTOR_INDEX_SCAN_TO_PHYSICAL,
         ]
 
         for promise in implementation_promises:
-            self.assertTrue(promise < Promise.IMPLEMENTATION_DELIMETER)
+            self.assertTrue(promise < Promise.IMPLEMENTATION_DELIMITER)
 
         promise_count = len(Promise)
         rewrite_count = len(set(rewrite_promises))
         implementation_count = len(set(implementation_promises))
 
-        # rewrite_count + implementation_count + 1 (for IMPLEMENTATION_DELIMETER)
+        # rewrite_count + implementation_count + 1 (for IMPLEMENTATION_DELIMITER)
         self.assertEqual(rewrite_count + implementation_count + 4, promise_count)
 
     def test_supported_rules(self):
         # adding/removing rules should update this test
         supported_rewrite_rules = [
             EmbedFilterIntoGet(),
             #    EmbedFilterIntoDerivedGet(),
             EmbedSampleIntoGet(),
             XformLateralJoinToLinearFlow(),
             PushDownFilterThroughApplyAndMerge(),
             PushDownFilterThroughJoin(),
-            CombineSimilarityOrderByAndLimitToFaissIndexScan(),
+            CombineSimilarityOrderByAndLimitToVectorIndexScan(),
             ReorderPredicates(),
+            XformExtractObjectToLinearFlow(),
         ]
         rewrite_rules = (
             RulesManager().stage_one_rewrite_rules
             + RulesManager().stage_two_rewrite_rules
         )
         self.assertEqual(
             len(supported_rewrite_rules),
@@ -232,17 +235,17 @@
             LogicalCreateMaterializedViewToPhysical(),
             LogicalFilterToPhysical(),
             DistributedLogicalProjectToPhysical()
             if ray_enabled
             else SequentialLogicalProjectToPhysical(),
             LogicalShowToPhysical(),
             LogicalExplainToPhysical(),
-            LogicalCreateIndexToFaiss(),
+            LogicalCreateIndexToVectorIndex(),
             LogicalApplyAndMergeToPhysical(),
-            LogicalFaissIndexScanToPhysical(),
+            LogicalVectorIndexScanToPhysical(),
         ]
 
         if ray_enabled:
             supported_implementation_rules.append(LogicalExchangeToPhysical())
         self.assertEqual(
             len(supported_implementation_rules),
             len(RulesManager().implementation_rules),
```

### Comparing `evadb-0.2.3.post0/test/optimizer/test_binder.py` & `evadb-0.2.4/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_cascade_optimizer.py` & `evadb-0.2.4/test/optimizer/test_cascade_optimizer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_cost_model.py` & `evadb-0.2.4/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_group.py` & `evadb-0.2.4/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_memo.py` & `evadb-0.2.4/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_optimizer_task.py` & `evadb-0.2.4/test/optimizer/test_optimizer_task.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.4/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/optimizer/test_statement_to_opr_convertor.py` & `evadb-0.2.4/test/optimizer/test_statement_to_opr_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     LogicalCreateMaterializedView,
     LogicalCreateUDF,
     LogicalDelete,
     LogicalDrop,
     LogicalDropUDF,
     LogicalExchange,
     LogicalExplain,
-    LogicalFaissIndexScan,
+    LogicalExtractObject,
     LogicalFilter,
     LogicalFunctionScan,
     LogicalGet,
     LogicalGroupBy,
     LogicalInsert,
     LogicalJoin,
     LogicalLimit,
@@ -42,112 +42,113 @@
     LogicalOrderBy,
     LogicalProject,
     LogicalQueryDerivedGet,
     LogicalRename,
     LogicalSample,
     LogicalShow,
     LogicalUnion,
+    LogicalVectorIndexScan,
     Operator,
 )
-from eva.optimizer.statement_to_opr_convertor import StatementToPlanConvertor
+from eva.optimizer.statement_to_opr_converter import StatementToPlanConverter
 from eva.parser.create_index_statement import CreateIndexStatement
 from eva.parser.create_statement import CreateTableStatement
 from eva.parser.create_udf_statement import CreateUDFStatement
 from eva.parser.drop_statement import DropTableStatement
 from eva.parser.drop_udf_statement import DropUDFStatement
 from eva.parser.explain_statement import ExplainStatement
 from eva.parser.insert_statement import InsertTableStatement
 from eva.parser.rename_statement import RenameTableStatement
 from eva.parser.select_statement import SelectStatement
 from eva.parser.table_ref import TableRef
 
 
 class StatementToOprTest(unittest.TestCase):
-    @patch("eva.optimizer.statement_to_opr_convertor.LogicalGet")
+    @patch("eva.optimizer.statement_to_opr_converter.LogicalGet")
     def test_visit_table_ref_should_create_logical_get_opr(self, mock_lget):
-        converter = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         table_ref = MagicMock(spec=TableRef, alias="alias")
         table_ref.is_select.return_value = False
         table_ref.sample_freq = None
         converter.visit_table_ref(table_ref)
         mock_lget.assert_called_with(table_ref, table_ref.table.table_obj, "alias")
         self.assertEqual(mock_lget.return_value, converter._plan)
 
-    @patch("eva.optimizer.statement_to_opr_convertor.LogicalFilter")
+    @patch("eva.optimizer.statement_to_opr_converter.LogicalFilter")
     def test_visit_select_predicate_should_add_logical_filter(self, mock_lfilter):
-        converter = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         select_predicate = MagicMock()
         converter._visit_select_predicate(select_predicate)
 
         mock_lfilter.assert_called_with(select_predicate)
         mock_lfilter.return_value.append_child.assert_called()
         self.assertEqual(mock_lfilter.return_value, converter._plan)
 
-    @patch("eva.optimizer.statement_to_opr_convertor.LogicalProject")
+    @patch("eva.optimizer.statement_to_opr_converter.LogicalProject")
     def test_visit_projection_should_add_logical_predicate(self, mock_lproject):
-        converter = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         projects = MagicMock()
 
         converter._visit_projection(projects)
         mock_lproject.assert_called_with(projects)
         mock_lproject.return_value.append_child.assert_called()
         self.assertEqual(mock_lproject.return_value, converter._plan)
 
     def test_visit_select_should_call_appropriate_visit_methods(self):
-        converter = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         converter.visit_table_ref = MagicMock()
         converter._visit_projection = MagicMock()
         converter._visit_select_predicate = MagicMock()
         converter._visit_union = MagicMock()
 
         statement = MagicMock()
         statement.from_table = MagicMock(spec=TableRef)
         converter.visit_select(statement)
 
         converter.visit_table_ref.assert_called_with(statement.from_table)
         converter._visit_projection.assert_called_with(statement.target_list)
         converter._visit_select_predicate.assert_called_with(statement.where_clause)
 
     def test_visit_select_should_not_call_visits_for_null_values(self):
-        converter = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         converter.visit_table_ref = MagicMock()
         converter._visit_projection = MagicMock()
         converter._visit_select_predicate = MagicMock()
         converter._visit_union = MagicMock()
 
         statement = SelectStatement()
 
         converter.visit_select(statement)
 
         converter.visit_table_ref.assert_not_called()
         converter._visit_projection.assert_not_called()
         converter._visit_select_predicate.assert_not_called()
 
-    @patch("eva.optimizer.statement_to_opr_convertor.LogicalCreateUDF")
+    @patch("eva.optimizer.statement_to_opr_converter.LogicalCreateUDF")
     @patch(
         "eva.optimizer.\
-statement_to_opr_convertor.column_definition_to_udf_io"
+statement_to_opr_converter.column_definition_to_udf_io"
     )
     @patch(
         "eva.optimizer.\
-statement_to_opr_convertor.metadata_definition_to_udf_metadata"
+statement_to_opr_converter.metadata_definition_to_udf_metadata"
     )
     def test_visit_create_udf(self, metadata_def_mock, col_def_mock, l_create_udf_mock):
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         stmt = MagicMock()
         stmt.name = "name"
         stmt.if_not_exists = True
         stmt.inputs = ["inp"]
         stmt.outputs = ["out"]
         stmt.impl_path = "tmp.py"
         stmt.udf_type = "classification"
         stmt.metadata = [("key1", "value1"), ("key2", "value2")]
         col_def_mock.side_effect = ["inp", "out"]
         metadata_def_mock.side_effect = [{"key1": "value1", "key2": "value2"}]
-        convertor.visit_create_udf(stmt)
+        converter.visit_create_udf(stmt)
         col_def_mock.assert_any_call(stmt.inputs, True)
         col_def_mock.assert_any_call(stmt.outputs, False)
         metadata_def_mock.assert_any_call(stmt.metadata)
         l_create_udf_mock.assert_called_once()
         l_create_udf_mock.assert_called_with(
             stmt.name,
             stmt.if_not_exists,
@@ -156,101 +157,101 @@
             stmt.impl_path,
             stmt.udf_type,
             {"key1": "value1", "key2": "value2"},
         )
 
     def test_visit_should_call_create_udf(self):
         stmt = MagicMock(spec=CreateUDFStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_create_udf = mock
+        converter.visit_create_udf = mock
 
-        convertor.visit(stmt)
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
-    @patch("eva.optimizer.statement_to_opr_convertor.LogicalDropUDF")
+    @patch("eva.optimizer.statement_to_opr_converter.LogicalDropUDF")
     @patch(
         "eva.optimizer.\
-statement_to_opr_convertor.column_definition_to_udf_io"
+statement_to_opr_converter.column_definition_to_udf_io"
     )
     def test_visit_drop_udf(self, mock, l_drop_udf_mock):
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         stmt = MagicMock()
         stmt.name = "name"
         stmt.if_exists = True
-        convertor.visit_drop_udf(stmt)
+        converter.visit_drop_udf(stmt)
         l_drop_udf_mock.assert_called_once()
         l_drop_udf_mock.assert_called_with(stmt.name, stmt.if_exists)
 
     def test_visit_should_call_drop_udf(self):
         stmt = MagicMock(spec=DropUDFStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_drop_udf = mock
+        converter.visit_drop_udf = mock
 
-        convertor.visit(stmt)
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
     def test_visit_should_call_insert(self):
         stmt = MagicMock(spec=InsertTableStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_insert = mock
+        converter.visit_insert = mock
 
-        convertor.visit(stmt)
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
     def test_visit_should_call_create(self):
         stmt = MagicMock(spec=CreateTableStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_create = mock
+        converter.visit_create = mock
 
-        convertor.visit(stmt)
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
     def test_visit_should_call_rename(self):
         stmt = MagicMock(spec=RenameTableStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_rename = mock
+        converter.visit_rename = mock
 
-        convertor.visit(stmt)
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
     def test_visit_should_call_explain(self):
         stmt = MagicMock(spec=ExplainStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_explain = mock
+        converter.visit_explain = mock
 
-        convertor.visit(stmt)
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_once_with(stmt)
 
     def test_visit_should_call_drop(self):
         stmt = MagicMock(spec=DropTableStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_drop = mock
-        convertor.visit(stmt)
+        converter.visit_drop = mock
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
     def test_visit_should_call_create_index(self):
         stmt = MagicMock(spec=CreateIndexStatement)
-        convertor = StatementToPlanConvertor()
+        converter = StatementToPlanConverter()
         mock = MagicMock()
-        convertor.visit_create_index = mock
-        convertor.visit(stmt)
+        converter.visit_create_index = mock
+        converter.visit(stmt)
         mock.assert_called_once()
         mock.assert_called_with(stmt)
 
     def test_inequality_in_operator(self):
         dummy_plan = Dummy(MagicMock(), MagicMock())
         object = MagicMock()
         self.assertNotEqual(dummy_plan, object)
@@ -281,23 +282,27 @@
         exchange_plan = LogicalExchange(MagicMock())
         show_plan = LogicalShow(MagicMock())
         drop_plan = LogicalDrop(MagicMock(), MagicMock())
         drop_udf_plan = LogicalDropUDF(MagicMock(), MagicMock())
         get_plan = LogicalGet(MagicMock(), MagicMock(), MagicMock())
         sample_plan = LogicalSample(MagicMock(), MagicMock())
         filter_plan = LogicalFilter(MagicMock())
-        faiss_plan = LogicalFaissIndexScan(MagicMock(), MagicMock(), MagicMock())
+        faiss_plan = LogicalVectorIndexScan(
+            MagicMock(), MagicMock(), MagicMock(), MagicMock()
+        )
         groupby_plan = LogicalGroupBy(MagicMock())
         order_by_plan = LogicalOrderBy(MagicMock())
         union_plan = LogicalUnion(MagicMock())
         function_scan_plan = LogicalFunctionScan(MagicMock(), MagicMock())
         join_plan = LogicalJoin(MagicMock(), MagicMock(), MagicMock(), MagicMock())
         project_plan = LogicalProject(MagicMock(), MagicMock())
         apply_and_merge_plan = LogicalApplyAndMerge(MagicMock(), MagicMock())
-
+        extract_object_plan = LogicalExtractObject(
+            MagicMock(), MagicMock(), MagicMock(), MagicMock()
+        )
         create_plan.append_child(create_udf_plan)
 
         plans.append(dummy_plan)
         plans.append(create_plan)
         plans.append(create_udf_plan)
         plans.append(create_index_plan)
         plans.append(create_materialized_view_plan)
@@ -319,14 +324,15 @@
         plans.append(join_plan)
         plans.append(apply_and_merge_plan)
         plans.append(show_plan)
         plans.append(explain_plan)
         plans.append(exchange_plan)
         plans.append(faiss_plan)
         plans.append(project_plan)
+        plans.append(extract_object_plan)
 
         derived_operators = list(get_all_subclasses(Operator))
 
         plan_type_list = []
         for plan in plans:
             plan_type_list.append(type(plan))
```

### Comparing `evadb-0.2.3.post0/test/parser/__init__.py` & `evadb-0.2.4/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/parser/test_parser.py` & `evadb-0.2.4/test/parser/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from pathlib import Path
 
-from eva.catalog.catalog_type import ColumnType, IndexType, NdArrayType
+from eva.catalog.catalog_type import ColumnType, NdArrayType, VectorStoreType
 from eva.expression.abstract_expression import ExpressionType
 from eva.expression.comparison_expression import ComparisonExpression
 from eva.expression.constant_value_expression import ConstantValueExpression
 from eva.expression.function_expression import FunctionExpression
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.alias import Alias
 from eva.parser.create_index_statement import CreateIndexStatement
@@ -46,36 +46,36 @@
 class ParserTests(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def test_create_index_statement(self):
         parser = Parser()
 
-        create_index_query = "CREATE INDEX testindex ON MyVideo (featCol) USING HNSW;"
+        create_index_query = "CREATE INDEX testindex ON MyVideo (featCol) USING FAISS;"
         eva_stmt_list = parser.parse(create_index_query)
 
         # check stmt itself
         self.assertIsInstance(eva_stmt_list, list)
         self.assertEqual(len(eva_stmt_list), 1)
         self.assertEqual(eva_stmt_list[0].stmt_type, StatementType.CREATE_INDEX)
 
         expected_stmt = CreateIndexStatement(
             "testindex",
             TableRef(TableInfo("MyVideo")),
             [
                 ColumnDefinition("featCol", None, None, None),
             ],
-            IndexType.HNSW,
+            VectorStoreType.FAISS,
         )
         actual_stmt = eva_stmt_list[0]
         self.assertEqual(actual_stmt, expected_stmt)
 
         # create index on UDF expression
         create_index_query = (
-            "CREATE INDEX testindex ON MyVideo (FeatureExtractor(featCol)) USING HNSW;"
+            "CREATE INDEX testindex ON MyVideo (FeatureExtractor(featCol)) USING FAISS;"
         )
         eva_stmt_list = parser.parse(create_index_query)
 
         # check stmt itself
         self.assertIsInstance(eva_stmt_list, list)
         self.assertEqual(len(eva_stmt_list), 1)
         self.assertEqual(eva_stmt_list[0].stmt_type, StatementType.CREATE_INDEX)
@@ -84,26 +84,26 @@
         func_expr.append_child(TupleValueExpression("featCol"))
         expected_stmt = CreateIndexStatement(
             "testindex",
             TableRef(TableInfo("MyVideo")),
             [
                 ColumnDefinition("featCol", None, None, None),
             ],
-            IndexType.HNSW,
+            VectorStoreType.FAISS,
             func_expr,
         )
         actual_stmt = eva_stmt_list[0]
         self.assertEqual(actual_stmt, expected_stmt)
 
     @unittest.skip("Skip parser exception handling testcase, moved to binder")
     def test_create_index_exception_statement(self):
         parser = Parser()
 
         create_index_query = (
-            "CREATE INDEX testindex USING HNSW ON MyVideo (featCol1, featCol2);"
+            "CREATE INDEX testindex USING FAISS ON MyVideo (featCol1, featCol2);"
         )
 
         with self.assertRaises(Exception):
             parser.parse(create_index_query)
 
     def test_explain_dml_statement(self):
         parser = Parser()
```

### Comparing `evadb-0.2.3.post0/test/parser/test_parser_statements.py` & `evadb-0.2.4/test/parser/test_parser_statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def test_parser_statement_types(self):
         parser = Parser()
 
         queries = [
-            "CREATE INDEX testindex ON MyVideo (featCol) USING HNSW;",
+            "CREATE INDEX testindex ON MyVideo (featCol) USING FAISS;",
             """CREATE TABLE IF NOT EXISTS Persons (
                   Frame_ID INTEGER UNIQUE,
                   Frame_Data TEXT(10),
                   Frame_Value FLOAT(1000, 201),
                   Frame_Array NDARRAY UINT8(5, 100, 2432, 4324, 100)
             )""",
             "RENAME TABLE student TO student_info",
@@ -86,15 +86,15 @@
                     ORDER BY Similarity(FeatureExtractor(Open("abc.jpg")),
                                         FeatureExtractor(data))
                     LIMIT 1;""",
         ]
         # The queries below are the result of randomly changing the case of the
         # characters in the above queries.
         randomized_cases = [
-            "Create index TestIndex on MyVideo (featCol) using HNSW;",
+            "Create index TestIndex on MyVideo (featCol) using FAISS;",
             """create table if not exists Persons (
                     Frame_ID integer unique,
                     Frame_Data text(10),
                     Frame_Value float(1000, 201),
                     Frame_Array ndArray uint8(5, 100, 2432, 4324, 100)
             )""",
             "Rename Table STUDENT to student_info",
```

### Comparing `evadb-0.2.3.post0/test/plan_nodes/__init__.py` & `evadb-0.2.4/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/plan_nodes/test_plan.py` & `evadb-0.2.4/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/readers/__init__.py` & `evadb-0.2.4/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/readers/test_csv_reader.py` & `evadb-0.2.4/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/readers/test_decord_reader.py` & `evadb-0.2.4/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/server/__init__.py` & `evadb-0.2.4/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/server/test_command_handler.py` & `evadb-0.2.4/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/server/test_db_api.py` & `evadb-0.2.4/test/server/test_db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/server/test_interpreter.py` & `evadb-0.2.4/test/server/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/server/test_server.py` & `evadb-0.2.4/test/server/test_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         @patch("asyncio.start_server")
         async def test_server_functions(self, mock_start):
             eva_server = EvaServer()
             host = "localhost"
-            port = 5432
+            port = 8803
 
             await eva_server.start_eva_server(host, port)
 
             # connection made
             client_reader1 = asyncio.StreamReader()
             client_writer1 = MagicMock()
             client_reader2 = asyncio.StreamReader()
```

### Comparing `evadb-0.2.3.post0/test/storage/__init__.py` & `evadb-0.2.4/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.4/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/storage/test_video_storage.py` & `evadb-0.2.4/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/test_eva_imports.py` & `evadb-0.2.4/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/test_eva_server.py` & `evadb-0.2.4/test/test_eva_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,9 +38,9 @@
             mock_udfs.assert_called_with(mode=mock_obj_1())
             mock_start_eva_server.assert_called_once()
             mock_run.assert_called_once()
 
         @patch("eva.eva_server.start_eva_server")
         @patch("asyncio.start_server")
         async def test_start_eva_server(self, mock_start_eva_server, mock_start):
-            await start_eva_server()
+            await start_eva_server("0.0.0.0", 8803)
             mock_start_eva_server.assert_called_once()
```

### Comparing `evadb-0.2.3.post0/test/udfs/__init__.py` & `evadb-0.2.4/test/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/decorators/__init__.py` & `evadb-0.2.4/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.4/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.4/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         self.assertEqual(catalog_entry.type, ColumnType.NDARRAY)
         self.assertEqual(catalog_entry.is_nullable, False)
         self.assertEqual(catalog_entry.array_type, NdArrayType.FLOAT32)
         self.assertEqual(catalog_entry.array_dimensions, (3, 256, 256))
         self.assertEqual(catalog_entry.is_input, False)
 
     def test_raises_error_on_incorrect_pandas_definition(self):
-        # the dataframe should have multipole columns but column_types should be defined for only one
+        # the dataframe should have multiple columns but column_types should be defined for only one
         pandas_dataframe = PandasDataframe(
             columns=["Frame_Array", "Frame_Array_2"],
             column_types=[NdArrayType.UINT8],
             column_shapes=[(3, 256, 256), (3, 256, 256)],
         )
         with self.assertRaises(UDFIODefinitionError):
             pandas_dataframe.generate_catalog_entries()
```

### Comparing `evadb-0.2.3.post0/test/udfs/decorators/test_decorators.py` & `evadb-0.2.4/test/udfs/decorators/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 from eva.catalog.catalog_type import NdArrayType
 from eva.udfs.decorators.decorators import forward, setup
 from eva.udfs.decorators.io_descriptors.data_types import NumpyArray, PandasDataframe
 
 
 class DecoratorTests(unittest.TestCase):
     def test_setup_flags_are_updated(self):
-        @setup(cachable=True, udf_type="classification", batchable=True)
+        @setup(cacheable=True, udf_type="classification", batchable=True)
         def setup_func():
             pass
 
         setup_func()
-        self.assertTrue(setup_func.tags["cachable"])
+        self.assertTrue(setup_func.tags["cacheable"])
         self.assertTrue(setup_func.tags["batchable"])
         self.assertEqual(setup_func.tags["udf_type"], "classification")
 
     def test_setup_flags_are_updated_with_default_values(self):
         @setup()
         def setup_func():
             pass
 
         setup_func()
-        self.assertFalse(setup_func.tags["cachable"])
+        self.assertFalse(setup_func.tags["cacheable"])
         self.assertTrue(setup_func.tags["batchable"])
         self.assertEqual(setup_func.tags["udf_type"], "Abstract")
 
     def test_forward_flags_are_updated(self):
         input_type = PandasDataframe(
             columns=["Frame_Array"],
             column_types=[NdArrayType.UINT8],
```

### Comparing `evadb-0.2.3.post0/test/udfs/ndarray/__init__.py` & `evadb-0.2.4/test/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.4/test/udfs/ndarray/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/ndarray/test_crop.py` & `evadb-0.2.4/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/ndarray/test_open.py` & `evadb-0.2.4/test/udfs/ndarray/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/test_abstract_udf.py` & `evadb-0.2.4/test/udfs/test_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/test_emotion_detector.py` & `evadb-0.2.4/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/test_facenet_udf.py` & `evadb-0.2.4/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.4/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.4/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/util.py` & `evadb-0.2.4/test/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import NdArrayType
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.expression.function_expression import FunctionExpression
 from eva.models.storage.batch import Batch
 from eva.optimizer.operators import LogicalFilter, Operator
 from eva.optimizer.plan_generator import PlanGenerator
-from eva.optimizer.statement_to_opr_convertor import StatementToPlanConvertor
+from eva.optimizer.statement_to_opr_converter import StatementToPlanConverter
 from eva.parser.parser import Parser
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.server.command_handler import execute_query_fetch_all
 from eva.udfs.abstract.abstract_udf import AbstractClassifierUDF
 from eva.udfs.decorators import decorators
 from eva.udfs.decorators.io_descriptors.data_types import NumpyArray, PandasDataframe
 from eva.udfs.udf_bootstrap_queries import init_builtin_udfs
@@ -187,15 +187,15 @@
         query (str): evaql query
 
     Returns:
         Operator: Logical plan generated by eva
     """
     stmt = Parser().parse(query)[0]
     StatementBinder(StatementBinderContext()).bind(stmt)
-    l_plan = StatementToPlanConvertor().visit(stmt)
+    l_plan = StatementToPlanConverter().visit(stmt)
     return l_plan
 
 
 def get_physical_query_plan(
     query: str, rule_manager=None, cost_model=None
 ) -> AbstractPlan:
     """Get the query plan
@@ -555,15 +555,15 @@
 
         ret = pd.DataFrame()
         ret["features"] = df.apply(_extract_feature, axis=1)
         return ret
 
 
 class DummyObjectDetectorDecorators(AbstractClassifierUDF):
-    @decorators.setup(cachable=True, udf_type="object_detection", batchable=True)
+    @decorators.setup(cacheable=True, udf_type="object_detection", batchable=True)
     def setup(self, *args, **kwargs):
         pass
 
     @property
     def name(self) -> str:
         return "DummyObjectDetectorDecorators"
```

### Comparing `evadb-0.2.3.post0/test/utils/__init__.py` & `evadb-0.2.4/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/utils/test_generic_utils.py` & `evadb-0.2.4/test/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/utils/test_timer.py` & `evadb-0.2.4/test/utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.3.post0/test/utils/test_xdist.py` & `evadb-0.2.4/test/utils/test_xdist.py`

 * *Files identical despite different names*

