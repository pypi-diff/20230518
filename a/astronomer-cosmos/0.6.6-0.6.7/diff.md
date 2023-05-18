# Comparing `tmp/astronomer_cosmos-0.6.6.tar.gz` & `tmp/astronomer_cosmos-0.6.7.tar.gz`

## Comparing `astronomer_cosmos-0.6.6.tar` & `astronomer_cosmos-0.6.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/spark.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0    11398 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/warn_parsing.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/LICENSE
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/README.rst
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/spark.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/LICENSE
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/README.rst
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.7/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.6/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.7/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.7/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/core/tests/test_airflow.py` & `astronomer_cosmos-0.6.7/cosmos/core/tests/test_airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/exasol.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/exasol.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/spark.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/spark.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/community/profiles/trino.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/community/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .local import DbtDepsLocalOperator as DbtDepsOperator
+from .local import DbtDocsLocalOperator as DbtDocsOperator
 from .local import DbtLSLocalOperator as DbtLSOperator
 from .local import DbtRunLocalOperator as DbtRunOperator
 from .local import DbtRunOperationLocalOperator as DbtRunOperationOperator
 from .local import DbtSeedLocalOperator as DbtSeedOperator
 from .local import DbtSnapshotLocalOperator as DbtSnapshotOperator
 from .local import DbtTestLocalOperator as DbtTestOperator
 
@@ -10,8 +11,9 @@
     "DbtLSOperator",
     "DbtSeedOperator",
     "DbtSnapshotOperator",
     "DbtRunOperator",
     "DbtTestOperator",
     "DbtRunOperationOperator",
     "DbtDepsOperator",
+    "DbtDocsOperator",
 ]
```

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,30 @@
 
 
 class DbtLocalBaseOperator(DbtBaseOperator):
     """
     Executes a dbt core cli command locally.
 
     :param install_deps: If true, install dependencies before running the command
+    :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
 
     def __init__(
         self,
         install_deps: bool = False,
+        callback: Optional[Callable[[str], None]] = None,
         **kwargs,
     ) -> None:
         self.install_deps = install_deps
+        self.callback = callback
         self.compiled_sql = ""
         super().__init__(**kwargs)
 
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
@@ -139,14 +142,16 @@
                 env=env,
                 output_encoding=self.output_encoding,
                 cwd=tmp_project_dir,
             )
 
             self.exception_handling(result)
             self.store_compiled_sql(tmp_project_dir, context)
+            if self.callback:
+                self.callback(tmp_project_dir)
 
             return result
 
     def build_and_run_cmd(
         self, context: Context, cmd_flags: list[str] | None = None
     ) -> FullOutputSubprocessResult:
         dbt_cmd, env = self.build_cmd(context=context, cmd_flags=cmd_flags)
@@ -336,14 +341,31 @@
 
     def execute(self, context: Context):
         cmd_flags = self.add_cmd_flags()
         result = self.build_and_run_cmd(context=context, cmd_flags=cmd_flags)
         return result.output
 
 
+class DbtDocsLocalOperator(DbtLocalBaseOperator):
+    """
+    Executes `dbt docs generate` command.
+    Use the `callback` parameter to specify a callback function to run after the command completes.
+    """
+
+    ui_color = "#8194E0"
+
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
+        self.base_cmd = ["docs", "generate"]
+
+    def execute(self, context: Context):
+        result = self.build_and_run_cmd(context=context)
+        return result.output
+
+
 class DbtDepsLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core deps command.
     """
 
     ui_color = "#8194E0"
```

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_docker.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/operators/tests/test_local.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/operators/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/profiles/tests/test_profiles.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/profiles/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/warn_parsing.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/parser/tests/test_project.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_dataset.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_export.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/cosmos/providers/dbt/tests/test_render.py` & `astronomer_cosmos-0.6.7/cosmos/providers/dbt/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/.gitignore` & `astronomer_cosmos-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/LICENSE` & `astronomer_cosmos-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/README.rst` & `astronomer_cosmos-0.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.6/pyproject.toml` & `astronomer_cosmos-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -135,21 +135,22 @@
 
     "apache-airflow-providers-docker>=3.5.0",
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
 ]
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10"]
-airflow = ["2.3", "2.4", "2.5"]
+airflow = ["2.3", "2.4", "2.5", "2.6"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.airflow.dependencies = [
     { value = "apache-airflow==2.3", if = ["2.3"] },
     { value = "apache-airflow==2.4", if = ["2.4"] },
     { value = "apache-airflow==2.5", if = ["2.5"] },
+    { value = "apache-airflow==2.6", if = ["2.6"] },
 ]
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
 test = "pytest ."
 test-cov = "pytest --cov=cosmos --cov-report=term-missing --cov-report=xml ."
```

### Comparing `astronomer_cosmos-0.6.6/PKG-INFO` & `astronomer_cosmos-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.6
+Version: 0.6.7
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

