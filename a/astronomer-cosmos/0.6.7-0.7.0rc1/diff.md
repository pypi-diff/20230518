# Comparing `tmp/astronomer_cosmos-0.6.7.tar.gz` & `tmp/astronomer_cosmos-0.7.0rc1.tar.gz`

## Comparing `astronomer_cosmos-0.6.7.tar` & `astronomer_cosmos-0.7.0rc1.tar`

### file list

```diff
@@ -1,55 +1,76 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/spark.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/warn_parsing.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/LICENSE
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/README.rst
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     8455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0    13421 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/base.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/tests/test_bq_service_account_file.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/token.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/databricks/tests/test_dbr_token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/exasol/tests/test_exasol_user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/postgres/tests/test_pg_user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/redshift/tests/test_redshift_user_pass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/snowflake/tests/test_snowflake_user_pass.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/thrift.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/spark/tests/test_spark_thrift.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_base.py
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/base.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_base.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_certificate.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_jwt.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/trino/tests/test_trino_ldap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/README.rst
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.0rc1/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/core/airflow.py` & `astronomer_cosmos-0.7.0rc1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.7.0rc1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/core/tests/test_airflow.py` & `astronomer_cosmos-0.7.0rc1/cosmos/core/tests/test_airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/dag.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     for additional configs to be passed.
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The path to the dbt root directory
     :param dbt_models_dir: The path to the dbt models directory within the project
     :param dbt_seeds_dir: The path to the dbt seeds directory within the project
     :param conn_id: The Airflow connection ID to use for the dbt profile
+    :param profile_args: Arguments to pass to the dbt profile
     :param dbt_args: Parameters to pass to the underlying dbt operators, can include dbt_executable_path to utilize venv
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
@@ -38,14 +39,15 @@
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
+        profile_args: Dict[str, str] = {},
         dbt_args: Dict[str, Any] = {},
         operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
@@ -69,14 +71,15 @@
             dbt_models_dir=dbt_models_dir,
             dbt_seeds_dir=dbt_seeds_dir,
             task_args=dbt_args,
             operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
+            profile_args=profile_args,
             select=select,
             exclude=exclude,
             execution_mode=execution_mode,
             on_warning_callback=on_warning_callback,
         )
 
         # call the airflow DAG constructor
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,30 @@
 logger = logging.getLogger(__name__)
 
 
 def calculate_operator_class(
     execution_mode: str,
     dbt_class: str,
 ) -> str:
+    "Given an execution mode and dbt class, return the operator class to use"
     return f"cosmos.providers.dbt.core.operators.{execution_mode}.{dbt_class}{execution_mode.capitalize()}Operator"
 
 
 def render_project(
     dbt_project_name: str,
     dbt_root_path: str = "/usr/local/airflow/dags/dbt",
     dbt_models_dir: str = "models",
     dbt_snapshots_dir: str = "snapshots",
     dbt_seeds_dir: str = "seeds",
     task_args: Dict[str, Any] = {},
     operator_args: Dict[str, Any] = {},
     test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
     emit_datasets: bool = True,
     conn_id: str = "default_conn_id",
+    profile_args: Dict[str, str] = {},
     select: Dict[str, List[str]] = {},
     exclude: Dict[str, List[str]] = {},
     execution_mode: Literal["local", "docker", "kubernetes"] = "local",
     on_warning_callback: Optional[Callable] = None,
 ) -> Group:
     """
     Turn a dbt project into a Group
@@ -50,15 +52,16 @@
     :param dbt_root_path: The root path to your dbt folder. Defaults to /usr/local/airflow/dags/dbt
     :param task_args: Arguments to pass to the underlying dbt operators
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
-    :param conn_id: The Airflow connection ID to use in Airflow Datasets
+    :param conn_id: The Airflow connection ID to use
+    :param profile_args: Arguments to pass to the dbt profile
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2]}})
     :param execution_mode: The execution mode in which the dbt project should be run.
         Options are "local", "docker", and "kubernetes".
         Defaults to "local"
      :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
@@ -93,14 +96,21 @@
     if "paths" in select and "paths" in exclude:
         if set(select["paths"]).intersection(exclude["paths"]):
             raise AirflowException(
                 f"Can't specify the same path in `select` and `include`: "
                 f"{set(select['paths']).intersection(exclude['paths'])}"
             )
 
+    # if task_args has a schema, add it to the profile args and add a deprecated warning
+    if "schema" in task_args:
+        profile_args["schema"] = task_args["schema"]
+        logger.warning(
+            "Specifying a schema in the task_args is deprecated. Please use the profile_args instead."
+        )
+
     # iterate over each model once to create the initial tasks
     for model_name, model in itertools.chain(
         project.models.items(), project.snapshots.items(), project.seeds.items()
     ):
         # filters down to a path within the project_dir
         if "paths" in select:
             root_directories = [
@@ -124,16 +134,26 @@
                 continue
 
         if "configs" in exclude:
             # TODO: coverme
             if set(exclude["configs"]).intersection(model.config.config_selectors):
                 continue
 
-        run_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
-        test_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
+        run_args: Dict[str, Any] = {
+            **task_args,
+            **operator_args,
+            "models": model_name,
+            "profile_args": profile_args,
+        }
+        test_args: Dict[str, Any] = {
+            **task_args,
+            **operator_args,
+            "models": model_name,
+            "profile_args": profile_args,
+        }
         # DbtTestOperator specific arg
         test_args["on_warning_callback"] = on_warning_callback
         if emit_datasets:
             outlets = [get_dbt_dataset(conn_id, dbt_project_name, model_name)]
 
             if test_behavior == "after_each":
                 test_args["outlets"] = outlets
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/task_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The path to the dbt root directory
     :param dbt_models_dir: The path to the dbt models directory within the project
     :param dbt_snapshots_dir: The path to the dbt snapshots directory within the project
     :param dbt_seeds_dir: The path to the dbt seeds directory within the project
     :param conn_id: The Airflow connection ID to use for the dbt profile
+    :param profile_args: Arguments to pass to the dbt profile
     :param dbt_args: Parameters to pass to the underlying dbt operators, can include dbt_executable_path to utilize venv
     :param operator_args: Parameters to pass to the underlying operators, can include KubernetesPodOperator
         or DockerOperator parameters
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
@@ -39,14 +40,15 @@
         and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
+        profile_args: Dict[str, str] = {},
         dbt_args: Dict[str, Any] = {},
         operator_args: Dict[str, Any] = {},
         emit_datasets: bool = True,
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_snapshots_dir: str = "snapshots",
         dbt_seeds_dir: str = "seeds",
@@ -72,14 +74,15 @@
             dbt_snapshots_dir=dbt_snapshots_dir,
             dbt_seeds_dir=dbt_seeds_dir,
             task_args=dbt_args,
             operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
+            profile_args=profile_args,
             select=select,
             exclude=exclude,
             execution_mode=execution_mode,
             on_warning_callback=on_warning_callback,
         )
 
         # call the airflow constructor
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/spark.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/bigquery/service_account_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,41 @@
+"Maps Airflow GCP connections to dbt BigQuery profiles if they use a service account file."
 from __future__ import annotations
 
-import logging
-from typing import TYPE_CHECKING
+from typing import Any
 
-if TYPE_CHECKING:
-    from airflow.models import Connection
+from cosmos.providers.dbt.core.profiles.base import BaseProfileMapping
 
-logger = logging.getLogger(__name__)
 
-# spark dbt profile
-spark_profile = {
-    "outputs": {
-        "dev": {
-            "type": "spark",
-            "host": "{{ env_var('SPARK_HOST') }}",
-            "method": "{{ env_var('SPARK_METHOD', 'thrift') }}",
-            "port": "{{ env_var('SPARK_PORT') | as_number }}",
-            "schema": "{{ env_var('SPARK_SCHEMA') }}",
-            "user": "{{ env_var('SPARK_USER') }}",
-        }
-    },
-    "target": "dev",
-}
-
-
-# Create a profile for spark thrift
-def create_profile_vars_spark_thrift(
-    conn: Connection,
-    database_override: str | None = None,
-    schema_override: str | None = None,
-) -> tuple[str, dict[str, str]]:
+class GoogleCloudServiceAccountFileProfileMapping(BaseProfileMapping):
     """
-    https://docs.getdbt.com/reference/warehouse-profiles/spark-profile
-    https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/stable/connections/spark.html
+    Maps Airflow GCP connections to dbt BigQuery profiles if they use a service account file.
+
+    https://docs.getdbt.com/reference/warehouse-setups/bigquery-setup#service-account-file
+    https://airflow.apache.org/docs/apache-airflow-providers-databricks/stable/connections/databricks.html
     """
-    if schema_override:
-        schema = schema_override
-    elif conn.schema:
-        schema = conn.schema
-    else:
-        schema = "default"
-        logging.info(
-            f"Using schema: {schema} as default since none specified in db_name or connection schema"
-        )
-
-    profile_vars = {
-        "SPARK_HOST": conn.host,
-        "SPARK_METHOD": "thrift",
-        "SPARK_PORT": str(conn.port),
-        "SPARK_SCHEMA": schema,
+
+    airflow_connection_type: str = "google-cloud-platform"
+
+    required_fields = [
+        "project",
+        "dataset",
+        "keyfile",
+    ]
+
+    airflow_param_mapping = {
+        "project": "extra.project",
+        "dataset": "dataset",
+        "keyfile": "extra.key_path",
     }
 
-    return "spark_profile", profile_vars
+    def get_profile(self) -> dict[str, Any | None]:
+        "Generates profile. Defaults `threads` to 1."
+        return {
+            "type": "bigquery",
+            "method": "service-account",
+            "project": self.project,
+            "dataset": self.dataset,
+            "threads": self.profile_args.get("threads") or 1,
+            "keyfile": self.keyfile,
+            **self.profile_args,
+        }
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 from typing import Any, Dict, Sequence, Tuple
 
 import yaml
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
 from airflow.utils.operator_helpers import context_to_airflow_vars
 
-from cosmos.providers.dbt.constants import DBT_PROFILE_PATH
-from cosmos.providers.dbt.core.utils.profiles_generator import (
-    create_default_profiles,
-    map_profile,
-)
-
 logger = logging.getLogger(__name__)
 
 
 class DbtBaseOperator(BaseOperator):
     """
     Executes a dbt core cli command.
 
@@ -30,16 +24,14 @@
     :param select: dbt optional argument that specifies which nodes to include.
     :param exclude: dbt optional argument that specifies which models to exclude.
     :param selector: dbt optional argument - the selector name to use, as defined in selectors.yml
     :param vars: dbt optional argument - Supply variables to the project. This argument overrides variables
         defined in your dbt_project.yml file. This argument should be a YAML
         string, eg. '{my_variable: my_value}' (templated)
     :param models: dbt optional argument that specifies which nodes to include.
-    :param profiles_dir: dbt optional argument that specifies which directory to look in for the profiles.yml file.
-    :param profile: dbt optional argument that specifies which profile of the profiles.yml file to use.
     :param cache_selected_only:
     :param no_version_check: dbt optional argument - If set, skip ensuring dbt's version matches the one specified in
         the dbt_project.yml file ('require-dbt-version')
     :param fail_fast: dbt optional argument to make dbt exit immediately if a single resource fails to build.
     :param quiet: dbt optional argument to show only error logs in stdout
     :param warn_error: dbt optional argument to convert dbt warnings into errors
     :param db_name: override the target db instead of the one supplied in the airflow connection
@@ -67,39 +59,36 @@
     global_flags = (
         "project_dir",
         "select",
         "exclude",
         "selector",
         "vars",
         "models",
-        "profiles_dir",
-        "profile",
     )
     global_boolean_flags = (
         "no_version_check",
         "cache_selected_only",
         "fail_fast",
         "quiet",
         "warn_error",
     )
 
+    include_system_env = False
     intercept_flag = True
 
     def __init__(
         self,
         project_dir: str,
         conn_id: str,
         base_cmd: str | list[str] = None,
         select: str = None,
         exclude: str = None,
         selector: str = None,
         vars: dict = None,
         models: str = None,
-        profiles_dir: str = None,
-        profile: str = None,
         cache_selected_only: bool = False,
         no_version_check: bool = False,
         fail_fast: bool = False,
         quiet: bool = False,
         warn_error: bool = False,
         db_name: str = None,
         schema: str = None,
@@ -116,16 +105,14 @@
         self.conn_id = conn_id
         self.base_cmd = base_cmd
         self.select = select
         self.exclude = exclude
         self.selector = selector
         self.vars = vars
         self.models = models
-        self.profiles_dir = profiles_dir
-        self.profile = profile
         self.cache_selected_only = cache_selected_only
         self.no_version_check = no_version_check
         self.fail_fast = fail_fast
         self.quiet = quiet
         self.warn_error = warn_error
         self.db_name = db_name
         self.schema = schema
@@ -135,47 +122,48 @@
         self.skip_exit_code = skip_exit_code
         self.cancel_query_on_kill = cancel_query_on_kill
         # dbt-ol is the OpenLineage wrapper for dbt, which automatically
         # generates and emits lineage data to a specified backend.
         dbt_ol_path = shutil.which("dbt-ol")
         if dbt_executable_path == "dbt" and shutil.which("dbt-ol"):
             self.dbt_executable_path = dbt_ol_path
+        elif dbt_executable_path == "dbt":
+            self.dbt_executable_path = shutil.which("dbt")
         else:
             self.dbt_executable_path = dbt_executable_path
         self.dbt_cmd_flags = dbt_cmd_flags
         super().__init__(**kwargs)
 
     def get_env(self, context: Context, profile_vars: dict[str, str]) -> dict[str, str]:
         """
         Builds the set of environment variables to be exposed for the bash command.
         The order of determination is:
-            1. Environment variables created for dbt profiles, `profile_vars`.
+            1. The env parameter passed to the Operator
             2. The Airflow context as environment variables.
-            3. System environment variables if dbt_args{"append_env": True}
-            4. User specified environment variables, through dbt_args{"vars": {"key": "val"}}
+            3. The profile variables from the dbt profile file.
         If a user accidentally uses a key that is found earlier in the determination order then it is overwritten.
         """
-        system_env = os.environ.copy()
-        env = self.env
-        if env is None:
-            env = system_env
-        elif self.append_env:
-            system_env.update(env)
-            env = system_env
+        env: dict[str, Any] = {}
+
+        # env parameter passed to the Operator
+        if self.env and isinstance(self.env, dict):
+            env.update(self.env)
+
+        # Airflow context as environment variables
         airflow_context_vars = context_to_airflow_vars(context, in_env_var_format=True)
-        self.log.debug(
-            "Exporting the following env vars:\n%s",
-            "\n".join(f"{k}={v}" for k, v in airflow_context_vars.items()),
-        )
-        combined_env = {**env, **airflow_context_vars, **profile_vars}
-        # Eventually the keys & values in the env dict get passed through os.fsencode which enforces this.
+        env.update(airflow_context_vars)
+
+        # profile variables from the dbt profile file
+        env.update(profile_vars)
+
+        # filter out invalid types
         accepted_types = (str, bytes, os.PathLike)
         filtered_env = {
             k: v
-            for k, v in combined_env.items()
+            for k, v in env.items()
             if all((isinstance(k, accepted_types), isinstance(v, accepted_types)))
         }
 
         return filtered_env
 
     def add_global_flags(self) -> list[str]:
         flags = []
@@ -197,32 +185,21 @@
                 flags.append(f"--{global_boolean_flag.replace('_', '-')}")
         return flags
 
     def build_cmd(
         self,
         context: Context,
         cmd_flags: list[str] | None = None,
-        handle_profile: bool = True,
     ) -> Tuple[list[str], dict]:
         dbt_cmd = [self.dbt_executable_path]
         if isinstance(self.base_cmd, str):
             dbt_cmd.append(self.base_cmd)
         else:
             dbt_cmd.extend(self.base_cmd)
         dbt_cmd.extend(self.add_global_flags())
         # add command specific flags
         if cmd_flags:
             dbt_cmd.extend(cmd_flags)
-        # add profile
-        if handle_profile:
-            create_default_profiles(DBT_PROFILE_PATH)
-            profile, profile_vars = map_profile(
-                conn_id=self.conn_id,
-                db_override=self.db_name,
-                schema_override=self.schema,
-            )
-            dbt_cmd.extend(["--profile", profile])
-            # set env vars
-            env = self.get_env(context, profile_vars)
-            return dbt_cmd, env
 
-        return dbt_cmd, {}
+        env = self.get_env(context, profile_vars={})
+
+        return dbt_cmd, env
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,15 @@
         return super().execute(context)
 
     def build_command(self, cmd_flags, context):
         # For the first round, we're going to assume that the command is dbt
         # This means that we don't have openlineage support, but we will create a ticket
         # to add that in the future
         self.dbt_executable_path = "dbt"
-        dbt_cmd, env_vars = self.build_cmd(
-            context=context, cmd_flags=cmd_flags, handle_profile=False
-        )
+        dbt_cmd, env_vars = self.build_cmd(context=context, cmd_flags=cmd_flags)
         # set env vars
         self.environment = {**env_vars, **self.environment}
         self.command = dbt_cmd
 
 
 class DbtLSDockerOperator(DbtDockerBaseOperator):
     """
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
         return super().execute(context)
 
     def build_kube_args(self, cmd_flags, context):
         # For the first round, we're going to assume that the command is dbt
         # This means that we don't have openlineage support, but we will create a ticket
         # to add that in the future
         self.dbt_executable_path = "dbt"
-        dbt_cmd, env_vars = self.build_cmd(
-            context=context, cmd_flags=cmd_flags, handle_profile=False
-        )
+        dbt_cmd, env_vars = self.build_cmd(context=context, cmd_flags=cmd_flags)
         # set env vars
         self.build_env_args(env_vars)
         self.arguments = dbt_cmd
 
 
 class DbtLSKubernetesOperator(DbtKubernetesBaseOperator):
     """
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 import signal
 import tempfile
-from collections import namedtuple
 from pathlib import Path
 from typing import Callable, Optional, Sequence
 
 import yaml
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.utils.context import Context
 from airflow.utils.session import NEW_SESSION, provide_session
 from sqlalchemy.orm import Session
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
+from cosmos.providers.dbt.core.profiles import get_profile_mapping
 from cosmos.providers.dbt.core.utils.adapted_subprocesshook import (
     FullOutputSubprocessHook,
+    FullOutputSubprocessResult,
 )
 from cosmos.providers.dbt.core.utils.warn_parsing import (
     extract_log_issues,
     parse_output,
 )
 
 logger = logging.getLogger(__name__)
 
-FullOutputSubprocessResult = namedtuple(
-    "FullOutputSubprocessResult", ["exit_code", "output", "full_output"]
-)
-
 
 class DbtLocalBaseOperator(DbtBaseOperator):
     """
     Executes a dbt core cli command locally.
 
+    :param profile_args: Arguments to pass to the profile. See
+        :py:class:`cosmos.providers.dbt.core.profiles.BaseProfileMapping`.
     :param install_deps: If true, install dependencies before running the command
     :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
+    include_system_env = True
 
     def __init__(
         self,
         install_deps: bool = False,
         callback: Optional[Callable[[str], None]] = None,
+        profile_args: dict[str, str] = {},
         **kwargs,
     ) -> None:
         self.install_deps = install_deps
+        self.profile_args = profile_args
         self.callback = callback
         self.compiled_sql = ""
         super().__init__(**kwargs)
 
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
@@ -124,14 +126,37 @@
             # need a subfolder because shutil.copytree will fail if the destination dir already exists
             tmp_project_dir = os.path.join(tmp_dir, "dbt_project")
             shutil.copytree(
                 self.project_dir,
                 tmp_project_dir,
             )
 
+            # get the profile name from the dbt_project.yml file
+            dbt_project_path = os.path.join(tmp_project_dir, "dbt_project.yml")
+            with open(dbt_project_path, encoding="utf-8") as f:
+                dbt_project = yaml.safe_load(f)
+
+            profile_name = dbt_project.get("profile")
+
+            # need to write the profile to a file because dbt requires a profile file
+            # and doesn't accept a profile as a string
+            profile_mapping = get_profile_mapping(
+                conn_id=self.conn_id,
+                profile_args=self.profile_args,
+            )
+            profile_file_contents = profile_mapping.get_profile_file_contents(
+                profile_name=profile_name,
+            )
+            profile_file_path = os.path.join(tmp_project_dir, "profiles.yml")
+            with open(profile_file_path, "w", encoding="utf-8") as f:
+                f.write(profile_file_contents)
+
+            # we also need to get the env from the profile mapping
+            env.update(profile_mapping.get_env_vars())
+
             # if we need to install deps, do so
             if self.install_deps:
                 self.subprocess_hook.run_command(
                     command=[self.dbt_executable_path, "deps"],
                     env=env,
                     output_encoding=self.output_encoding,
                     cwd=tmp_project_dir,
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_docker.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 @patch("airflow.providers.cncf.kubernetes.operators.pod.KubernetesPodOperator.hook")
 def test_created_pod(test_hook):
     test_hook.is_in_cluster = False
     test_hook._get_namespace.return_value.to_dict.return_value = "foo"
     ls_kwargs = {"env_vars": {"FOO": "BAR"}}
     ls_kwargs.update(base_kwargs)
     ls_operator = DbtLSKubernetesOperator(**ls_kwargs)
-    ls_operator.build_kube_args(context=MagicMock(), cmd_flags=MagicMock())
+    ls_operator.build_kube_args(context={}, cmd_flags=MagicMock())
     pod_obj = ls_operator.build_pod_request_obj()
     expected_result = {
         "api_version": "v1",
         "kind": "Pod",
         "metadata": {
             "annotations": {},
             "cluster_name": None,
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_local.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/operators/tests/test_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,17 +81,15 @@
     p_context_to_airflow_vars.return_value = {"START_DATE": "2023-02-15 12:30:00"}
     env = dbt_base_operator.get_env(
         Context(execution_date=datetime(2023, 2, 15, 12, 30)),
         profile_vars={
             "SNOWFLAKE_USER": "my_user_id",
             "SNOWFLAKE_PASSWORD": "supersecure123",
             "SNOWFLAKE_ACCOUNT": "my_account",
-            "SNOWFLAKE_ROLE": None,
             "SNOWFLAKE_DATABASE": "my_database",
-            "SNOWFLAKE_WAREHOUSE": None,
             "SNOWFLAKE_SCHEMA": "jaffle_shop",
         },
     )
     expected_env = {
         "start_date": "20220101",
         "end_date": "20220102",
         "some_path": Path(__file__),
```

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/tests/test_profiles.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/profiles/tests/test_profiles.py.tmp`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/warn_parsing.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/tests/test_project.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_dataset.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_export.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_render.py` & `astronomer_cosmos-0.7.0rc1/cosmos/providers/dbt/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/.gitignore` & `astronomer_cosmos-0.7.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/LICENSE` & `astronomer_cosmos-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.7/README.rst` & `astronomer_cosmos-0.7.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     ):
 
         e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
             dbt_project_name="jaffle_shop",
             conn_id="airflow_db",
-            dbt_args={
+            profile_args={
                 "schema": "public",
             },
         )
 
         e2 = EmptyOperator(task_id="post_dbt")
 
         e1 >> dbt_tg >> e2
```

### Comparing `astronomer_cosmos-0.6.7/pyproject.toml` & `astronomer_cosmos-0.7.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -151,24 +151,32 @@
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
 test = "pytest ."
 test-cov = "pytest --cov=cosmos --cov-report=term-missing --cov-report=xml ."
 
 ######################################
+# PYTEST
+######################################
+[tool.pytest.ini_options]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+]
+
+######################################
 # DOCS
 ######################################
 
 [tool.hatch.envs.docs]
 dependencies = [
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx-autobuild",
     "sphinx-tabs",
-    "sphinx-autoapi"
+    "sphinx-autoapi",
 ]
 
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs docs/_build"
 serve = "sphinx-autobuild docs docs/_build"
 
 ######################################
```

### Comparing `astronomer_cosmos-0.6.7/PKG-INFO` & `astronomer_cosmos-0.7.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.7
+Version: 0.7.0rc1
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -132,15 +132,15 @@
     ):
 
         e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
             dbt_project_name="jaffle_shop",
             conn_id="airflow_db",
-            dbt_args={
+            profile_args={
                 "schema": "public",
             },
         )
 
         e2 = EmptyOperator(task_id="post_dbt")
 
         e1 >> dbt_tg >> e2
```

