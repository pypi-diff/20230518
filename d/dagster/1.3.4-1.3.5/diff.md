# Comparing `tmp/dagster-1.3.4.tar.gz` & `tmp/dagster-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.4.tar", last modified: Thu May 11 16:59:05 2023, max compression
+gzip compressed data, was "dagster-1.3.5.tar", last modified: Thu May 18 20:38:25 2023, max compression
```

## Comparing `dagster-1.3.4.tar` & `dagster-1.3.5.tar`

### file list

```diff
@@ -1,624 +1,626 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-11 16:58:41.000000 dagster-1.3.4/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-11 16:58:41.000000 dagster-1.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-11 16:58:41.000000 dagster-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-11 16:59:05.300600 dagster-1.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-05-11 16:58:41.000000 dagster-1.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.236600 dagster-1.3.4/dagster/
--rw-r--r--   0 root         (0) root         (0)    26157 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26783 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5695 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29862 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.240600 dagster-1.3.4/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14686 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18799 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16880 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.244600 dagster-1.3.4/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    71379 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    16671 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.244600 dagster-1.3.4/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.244600 dagster-1.3.4/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7626 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29445 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36842 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    47566 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    18474 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    64232 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24005 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     3681 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20769 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42826 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8656 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6695 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    20546 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39988 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21013 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16195 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44740 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    50969 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32319 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    55971 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    37817 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47274 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27270 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18856 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17401 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    16979 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    16162 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    24105 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    38400 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    36722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    46040 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    14249 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    12225 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    74641 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.256600 dagster-1.3.4/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    64981 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7783 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.260600 dagster-1.3.4/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38474 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    30251 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14476 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.260600 dagster-1.3.4/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21992 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9369 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    26845 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27417 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    33974 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    44193 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18544 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5426 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8540 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14467 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23031 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16270 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27355 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)     9984 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37831 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    59386 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19377 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15667 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14328 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2789 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33529 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32103 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    69817 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    17368 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.264600 dagster-1.3.4/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   103988 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24318 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    21250 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18257 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.268600 dagster-1.3.4/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2815 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.276600 dagster-1.3.4/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.276600 dagster-1.3.4/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.284600 dagster-1.3.4/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.284600 dagster-1.3.4/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    23527 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11640 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14381 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3630 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    78441 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7408 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18950 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    26292 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23189 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15454 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46394 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    19749 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18920 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.288600 dagster-1.3.4/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26620 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6828 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17726 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    37649 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2722 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.232601 dagster-1.3.4/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.292600 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28114 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38178 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18324 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    22000 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    54827 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26359 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31794 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37037 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.296600 dagster-1.3.4/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    23982 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2372 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10412 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    23902 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.300600 dagster-1.3.4/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:58:41.000000 dagster-1.3.4/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 16:59:05.236600 dagster-1.3.4/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24949 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 16:59:05.000000 dagster-1.3.4/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-11 16:59:05.304600 dagster-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6432 2023-05-11 16:58:41.000000 dagster-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-18 20:38:07.000000 dagster-1.3.5/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-1.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-18 20:38:07.000000 dagster-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-05-18 20:38:25.105472 dagster-1.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-05-18 20:38:07.000000 dagster-1.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.029472 dagster-1.3.5/dagster/
+-rw-r--r--   0 root         (0) root         (0)    26157 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27119 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29822 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.037473 dagster-1.3.5/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15864 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.037473 dagster-1.3.5/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    71109 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.037473 dagster-1.3.5/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.041473 dagster-1.3.5/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30229 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36842 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    56981 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    64232 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24005 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/auto_materialize_condition.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20795 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    17905 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42826 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8656 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    20546 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39988 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21013 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16195 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44740 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    51147 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32319 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    55971 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22629 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    37817 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47274 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27231 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18856 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17401 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    16917 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    16162 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38400 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    36719 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    46037 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14249 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    76525 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15645 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    64981 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.057473 dagster-1.3.5/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38315 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    30249 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14476 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.061473 dagster-1.3.5/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    26845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27417 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    33974 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    44193 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18501 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.061473 dagster-1.3.5/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23031 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16270 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27355 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37831 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    57790 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19280 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15667 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14328 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33518 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32089 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    70934 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    17368 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   103917 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24318 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6629 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17249 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21475 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.069472 dagster-1.3.5/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.069472 dagster-1.3.5/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.069472 dagster-1.3.5/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16654 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.073473 dagster-1.3.5/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.077473 dagster-1.3.5/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.085472 dagster-1.3.5/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.085472 dagster-1.3.5/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    23596 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14381 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    78441 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7408 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18950 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    27079 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23189 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15454 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46394 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6256 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    22092 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18922 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    26620 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17726 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    37645 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.025472 dagster-1.3.5/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28114 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38178 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18324 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    21967 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    51206 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31790 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.101472 dagster-1.3.5/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37613 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.101472 dagster-1.3.5/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.101472 dagster-1.3.5/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    24259 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12340 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10412 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    26853 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.029472 dagster-1.3.5/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25105 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-18 20:38:25.105472 dagster-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6440 2023-05-18 20:38:07.000000 dagster-1.3.5/setup.py
```

### Comparing `dagster-1.3.4/COPYING` & `dagster-1.3.5/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/LICENSE` & `dagster-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/PKG-INFO` & `dagster-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.4
+Version: 1.3.5
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.4/README.md` & `dagster-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/__init__.py` & `dagster-1.3.5/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_annotations.py` & `dagster-1.3.5/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/get_server_id.py` & `dagster-1.3.5/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/list_repositories.py` & `dagster-1.3.5/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/notebook_data.py` & `dagster-1.3.5/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.5/dagster/_api/snapshot_execution_plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,38 +20,38 @@
 
 def sync_get_external_execution_plan_grpc(
     api_client: "DagsterGrpcClient",
     job_origin: ExternalJobOrigin,
     run_config: Mapping[str, Any],
     job_snapshot_id: str,
     asset_selection: Optional[AbstractSet[AssetKey]] = None,
-    solid_selection: Optional[Sequence[str]] = None,
+    op_selection: Optional[Sequence[str]] = None,
     step_keys_to_execute: Optional[Sequence[str]] = None,
     known_state: Optional[KnownExecutionState] = None,
     instance: Optional[DagsterInstance] = None,
 ) -> ExecutionPlanSnapshot:
     from dagster._grpc.client import DagsterGrpcClient
 
     check.inst_param(api_client, "api_client", DagsterGrpcClient)
     check.inst_param(job_origin, "job_origin", ExternalJobOrigin)
-    solid_selection = check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
+    op_selection = check.opt_sequence_param(op_selection, "op_selection", of_type=str)
     asset_selection = check.opt_nullable_set_param(
         asset_selection, "asset_selection", of_type=AssetKey
     )
     run_config = check.mapping_param(run_config, "run_config", key_type=str)
     check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
     check.str_param(job_snapshot_id, "job_snapshot_id")
     check.opt_inst_param(known_state, "known_state", KnownExecutionState)
     check.opt_inst_param(instance, "instance", DagsterInstance)
 
     result = deserialize_value(
         api_client.execution_plan_snapshot(
             execution_plan_snapshot_args=ExecutionPlanSnapshotArgs(
                 job_origin=job_origin,
-                solid_selection=solid_selection,
+                op_selection=op_selection,
                 run_config=run_config,
                 mode=DEFAULT_MODE_NAME,
                 step_keys_to_execute=step_keys_to_execute,
                 job_snapshot_id=job_snapshot_id,
                 known_state=known_state,
                 instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
                 asset_selection=asset_selection,
```

### Comparing `dagster-1.3.4/dagster/_api/snapshot_job.py` & `dagster-1.3.5/dagster/_api/snapshot_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import TYPE_CHECKING, AbstractSet, Optional, Sequence
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.errors import DagsterUserCodeProcessError
 from dagster._core.host_representation.external_data import ExternalJobSubsetResult
 from dagster._core.host_representation.origin import ExternalJobOrigin
 from dagster._grpc.types import JobSubsetSnapshotArgs
@@ -11,29 +11,31 @@
 if TYPE_CHECKING:
     from dagster._grpc.client import DagsterGrpcClient
 
 
 def sync_get_external_job_subset_grpc(
     api_client: "DagsterGrpcClient",
     job_origin: ExternalJobOrigin,
-    solid_selection: Optional[Sequence[str]] = None,
-    asset_selection: Optional[Sequence[AssetKey]] = None,
+    op_selection: Optional[Sequence[str]] = None,
+    asset_selection: Optional[AbstractSet[AssetKey]] = None,
 ) -> ExternalJobSubsetResult:
     from dagster._grpc.client import DagsterGrpcClient
 
     check.inst_param(api_client, "api_client", DagsterGrpcClient)
     job_origin = check.inst_param(job_origin, "job_origin", ExternalJobOrigin)
-    solid_selection = check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
-    asset_selection = check.opt_sequence_param(asset_selection, "asset_selection", of_type=AssetKey)
+    op_selection = check.opt_nullable_sequence_param(op_selection, "op_selection", of_type=str)
+    asset_selection = check.opt_nullable_set_param(
+        asset_selection, "asset_selection", of_type=AssetKey
+    )
 
     result = deserialize_value(
         api_client.external_pipeline_subset(
             pipeline_subset_snapshot_args=JobSubsetSnapshotArgs(
                 job_origin=job_origin,
-                solid_selection=solid_selection,
+                op_selection=op_selection,
                 asset_selection=asset_selection,
             ),
         ),
         ExternalJobSubsetResult,
     )
 
     if result.error:
```

### Comparing `dagster-1.3.4/dagster/_api/snapshot_partition.py` & `dagster-1.3.5/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/snapshot_repository.py` & `dagster-1.3.5/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/snapshot_schedule.py` & `dagster-1.3.5/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_api/snapshot_sensor.py` & `dagster-1.3.5/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_check/README.md` & `dagster-1.3.5/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_check/__init__.py` & `dagster-1.3.5/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/__init__.py` & `dagster-1.3.5/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/api.py` & `dagster-1.3.5/dagster/_cli/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import json
 import logging
 import os
 import sys
+import threading
 import zlib
 from contextlib import ExitStack
 from typing import Any, Callable, Optional, cast
 
 import click
 
 import dagster._check as check
@@ -28,14 +29,15 @@
     get_python_environment_entry_point,
 )
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
 from dagster._core.utils import coerce_valid_log_level
 from dagster._grpc import DagsterGrpcClient, DagsterGrpcServer
 from dagster._grpc.impl import core_execute_run
+from dagster._grpc.server import DagsterApiServer
 from dagster._grpc.types import ExecuteRunArgs, ExecuteStepArgs, ResumeRunArgs
 from dagster._serdes import deserialize_value, serialize_value
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.hosted_user_process import recon_job_from_origin
 from dagster._utils.interrupts import capture_interrupts
 from dagster._utils.log import configure_loggers
 
@@ -416,15 +418,15 @@
         else:
             repository_load_data = None
 
         recon_job = (
             recon_job_from_origin(cast(JobPythonOrigin, dagster_run.job_code_origin))
             .with_repository_load_data(repository_load_data)
             .get_subset(
-                op_selection=dagster_run.solids_to_execute,
+                op_selection=dagster_run.resolved_op_selection,
                 asset_selection=dagster_run.asset_selection,
             )
         )
 
         execution_plan = create_execution_plan(
             recon_job,
             run_config=dagster_run.run_config,
@@ -546,23 +548,14 @@
     help=(
         "Indicates that the working directory should be empty and should not set to the current "
         "directory as a default"
     ),
     envvar="DAGSTER_EMPTY_WORKING_DIRECTORY",
 )
 @click.option(
-    "--ipc-output-file",
-    type=click.Path(),
-    help=(
-        "[INTERNAL] This option should generally not be used by users. Internal param used by"
-        " dagster when it automatically spawns gRPC servers to communicate the success or failure"
-        " of the server launching."
-    ),
-)
-@click.option(
     "--fixed-server-id",
     type=click.STRING,
     required=False,
     help=(
         "[INTERNAL] This option should generally not be used by users. Internal param used by "
         "dagster to spawn a gRPC server with the specified server id."
     ),
@@ -626,28 +619,37 @@
     port=None,
     socket=None,
     host=None,
     max_workers=None,
     heartbeat=False,
     heartbeat_timeout=30,
     lazy_load_user_code=False,
-    ipc_output_file=None,
     fixed_server_id=None,
     override_system_timezone=None,
     log_level="INFO",
     use_python_environment_entry_point=False,
     container_image=None,
     container_context=None,
     location_name=None,
     instance_ref=None,
     inject_env_vars_from_instance=False,
     **kwargs,
 ):
     from dagster._core.test_utils import mock_system_timezone
 
+    check.invariant(heartbeat_timeout > 0, "heartbeat_timeout must be greater than 0")
+
+    check.invariant(
+        max_workers is None or max_workers > 1 if heartbeat else True,
+        (
+            "max_workers must be greater than 1 or set to None if heartbeat is True. "
+            "If set to None, the server will use the gRPC default."
+        ),
+    )
+
     if seven.IS_WINDOWS and port is None:
         raise click.UsageError(
             "You must pass a valid --port/-p on Windows: --socket/-s not supported."
         )
     if not (port or socket and not (port and socket)):
         raise click.UsageError("You must pass one and only one of --port/-p or --socket/-s.")
 
@@ -685,39 +687,45 @@
             package_name=kwargs["package_name"],
         )
 
     with ExitStack() as exit_stack:
         if override_system_timezone:
             exit_stack.enter_context(mock_system_timezone(override_system_timezone))
 
-        server = DagsterGrpcServer(
-            port=port,
-            socket=socket,
-            host=host,
+        server_termination_event = threading.Event()
+        api_servicer = DagsterApiServer(
+            server_termination_event=server_termination_event,
             loadable_target_origin=loadable_target_origin,
-            max_workers=max_workers,
             heartbeat=heartbeat,
             heartbeat_timeout=heartbeat_timeout,
             lazy_load_user_code=lazy_load_user_code,
-            ipc_output_file=ipc_output_file,
             fixed_server_id=fixed_server_id,
             entry_point=(
                 get_python_environment_entry_point(sys.executable)
                 if use_python_environment_entry_point
                 else DEFAULT_DAGSTER_ENTRY_POINT
             ),
             container_image=container_image,
-            container_context=json.loads(container_context)
-            if container_context is not None
-            else None,
+            container_context=(
+                json.loads(container_context) if container_context is not None else None
+            ),
             inject_env_vars_from_instance=inject_env_vars_from_instance,
             instance_ref=deserialize_value(instance_ref, InstanceRef) if instance_ref else None,
             location_name=location_name,
         )
 
+        server = DagsterGrpcServer(
+            server_termination_event=server_termination_event,
+            dagster_api_servicer=api_servicer,
+            port=port,
+            socket=socket,
+            host=host,
+            max_workers=max_workers,
+        )
+
         code_desc = " "
         if loadable_target_origin:
             if loadable_target_origin.python_file:
                 code_desc = f" for file {loadable_target_origin.python_file} "
             elif loadable_target_origin.package_name:
                 code_desc = f" for package {loadable_target_origin.package_name} "
             elif loadable_target_origin.module_name:
```

### Comparing `dagster-1.3.4/dagster/_cli/asset.py` & `dagster-1.3.5/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/config_scaffolder.py` & `dagster-1.3.5/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/debug.py` & `dagster-1.3.5/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/dev.py` & `dagster-1.3.5/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/instance.py` & `dagster-1.3.5/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/job.py` & `dagster-1.3.5/dagster/_cli/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,63 +459,63 @@
         )
 
         if preset and config:
             raise click.UsageError("Can not use --preset with -c / --config / --config-json.")
 
         run_tags = get_tags_from_args(kwargs)
 
-        solid_selection = get_op_selection_from_args(kwargs)
+        op_selection = get_op_selection_from_args(kwargs)
 
         dagster_run = _create_external_run(
             instance=instance,
             code_location=code_location,
             external_repo=external_repo,
             external_job=external_job,
             run_config=config,
             tags=run_tags,
-            solid_selection=solid_selection,
+            op_selection=op_selection,
             run_id=cast(Optional[str], kwargs.get("run_id")),
         )
 
         return instance.submit_run(dagster_run.run_id, workspace)
 
 
 def _create_external_run(
     instance: DagsterInstance,
     code_location: CodeLocation,
     external_repo: ExternalRepository,
     external_job: ExternalJob,
     run_config: Mapping[str, object],
     tags: Optional[Mapping[str, str]],
-    solid_selection: Optional[Sequence[str]],
+    op_selection: Optional[Sequence[str]],
     run_id: Optional[str],
 ) -> DagsterRun:
     check.inst_param(instance, "instance", DagsterInstance)
     check.inst_param(code_location, "code_location", CodeLocation)
     check.inst_param(external_repo, "external_repo", ExternalRepository)
     check.inst_param(external_job, "external_job", ExternalJob)
     check.opt_mapping_param(run_config, "run_config", key_type=str)
 
     check.opt_mapping_param(tags, "tags", key_type=str)
-    check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
+    check.opt_sequence_param(op_selection, "op_selection", of_type=str)
     check.opt_str_param(run_id, "run_id")
 
-    run_config, tags, solid_selection = _check_execute_external_job_args(
+    run_config, tags, op_selection = _check_execute_external_job_args(
         external_job,
         run_config,
         tags,
-        solid_selection,
+        op_selection,
     )
 
     job_name = external_job.name
     job_subset_selector = JobSubsetSelector(
         location_name=code_location.name,
         repository_name=external_repo.name,
         job_name=job_name,
-        solid_selection=solid_selection,
+        op_selection=op_selection,
     )
 
     external_job = code_location.get_external_job(job_subset_selector)
 
     external_execution_plan = code_location.get_external_execution_plan(
         external_job,
         run_config,
@@ -525,17 +525,17 @@
     )
     execution_plan_snapshot = external_execution_plan.execution_plan_snapshot
 
     return instance.create_run(
         job_name=job_name,
         run_id=run_id,
         run_config=run_config,
-        solids_to_execute=external_job.solids_to_execute,
+        resolved_op_selection=external_job.resolved_op_selection,
         step_keys_to_execute=execution_plan_snapshot.step_keys_to_execute,
-        solid_selection=solid_selection,
+        op_selection=op_selection,
         status=None,
         root_run_id=None,
         parent_run_id=None,
         tags=tags,
         job_snapshot=external_job.job_snapshot,
         execution_plan_snapshot=execution_plan_snapshot,
         parent_job_snapshot=external_job.parent_job_snapshot,
@@ -545,27 +545,27 @@
     )
 
 
 def _check_execute_external_job_args(
     external_job: ExternalJob,
     run_config: Mapping[str, object],
     tags: Optional[Mapping[str, str]],
-    solid_selection: Optional[Sequence[str]],
+    op_selection: Optional[Sequence[str]],
 ) -> Tuple[Mapping[str, object], Mapping[str, str], Optional[Sequence[str]]]:
     check.inst_param(external_job, "external_job", ExternalJob)
     run_config = check.opt_mapping_param(run_config, "run_config")
 
     tags = check.opt_mapping_param(tags, "tags", key_type=str)
-    check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
+    check.opt_sequence_param(op_selection, "op_selection", of_type=str)
     tags = merge_dicts(external_job.tags, tags)
 
     return (
         run_config,
         validate_tags(tags),
-        solid_selection,
+        op_selection,
     )
 
 
 @job_cli.command(
     name="scaffold_config",
     help="Scaffold the config for a job.\n\n{instructions}".format(
         instructions=get_job_in_same_python_env_instructions("scaffold_config")
```

### Comparing `dagster-1.3.4/dagster/_cli/load_handle.py` & `dagster-1.3.5/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/project.py` & `dagster-1.3.5/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/run.py` & `dagster-1.3.5/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/schedule.py` & `dagster-1.3.5/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/sensor.py` & `dagster-1.3.5/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/utils.py` & `dagster-1.3.5/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.5/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/__init__.py` & `dagster-1.3.5/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/config_schema.py` & `dagster-1.3.5/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/config_type.py` & `dagster-1.3.5/dagster/_config/config_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -339,20 +339,50 @@
                 GREEN = enum.auto()
                 BLUE = enum.auto()
 
             @op(
                 config_schema={"color": Field(Enum.from_python_enum(Color))}
             )
             def select_color(context):
-                # ...
+                assert context.op_config["color"] == Color.RED
         """
         if name is None:
             name = enum.__name__
         return cls(name, [EnumValue(v.name, python_value=v) for v in enum])
 
+    @classmethod
+    def from_python_enum_direct_values(cls, enum, name=None):
+        """Create a Dagster enum corresponding to an existing Python enum, where the direct values are passed instead of symbolic values (IE, enum.symbol.value as opposed to enum.symbol).
+
+        This is necessary for internal usage, as the symbolic values are not serializable.
+
+        Args:
+            enum (enum.EnumMeta):
+                The class representing the enum.
+            name (Optional[str]):
+                The name for the enum. If not present, `enum.__name__` will be used.
+
+        Example:
+        .. code-block:: python
+
+            class Color(enum.Enum):
+                RED = enum.auto()
+                GREEN = enum.auto()
+                BLUE = enum.auto()
+
+            @op(
+                config_schema={"color": Field(Enum.from_python_enum(Color))}
+            )
+            def select_color(context):
+                assert context.op_config["color"] == Color.RED.value
+        """
+        if name is None:
+            name = enum.__name__
+        return cls(name, [EnumValue(v.name, python_value=v.value) for v in enum])
+
 
 class ScalarUnion(ConfigType):
     """Defines a configuration type that accepts a scalar value OR a non-scalar value like a
     :py:class:`~dagster.List`, :py:class:`~dagster.Dict`, or :py:class:`~dagster.Selector`.
 
     This allows runtime scalars to be configured without a dictionary with the key ``value`` and
     instead just use the scalar value directly. However this still leaves the option to
```

### Comparing `dagster-1.3.4/dagster/_config/errors.py` & `dagster-1.3.5/dagster/_config/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,14 +374,30 @@
                 type=type(config_value),
             )
         ),
         error_data=RuntimeMismatchErrorData(context.config_type_snap, repr(config_value)),
     )
 
 
+def create_pydantic_env_var_error(context: ContextData, config_value: object) -> EvaluationError:
+    correct_env_var = str({"env": config_value})
+    return EvaluationError(
+        stack=context.stack,
+        reason=DagsterEvaluationErrorReason.RUNTIME_TYPE_MISMATCH,
+        message=(
+            f'Invalid use of environment variable wrapper. Value "{config_value}" is wrapped with'
+            " EnvVar(), which is reserved for passing to structured pydantic config objects only."
+            " To provide an environment variable to a run config dictionary, replace"
+            f' EnvVar("{config_value}") with {correct_env_var}, or pass a structured RunConfig'
+            " object."
+        ),
+        error_data=RuntimeMismatchErrorData(context.config_type_snap, repr(config_value)),
+    )
+
+
 def create_selector_multiple_fields_error(
     context: ContextData, config_value: Mapping[str, object]
 ) -> EvaluationError:
     check.inst_param(context, "context", ContextData)
 
     defined_fields = sorted(context.config_type_snap.field_names)
     incoming_fields = sorted(list(config_value.keys()))
```

### Comparing `dagster-1.3.4/dagster/_config/evaluate_value_result.py` & `dagster-1.3.5/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/field.py` & `dagster-1.3.5/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/field_utils.py` & `dagster-1.3.5/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/post_process.py` & `dagster-1.3.5/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/primitive_mapping.py` & `dagster-1.3.5/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.5/dagster/_config/pythonic_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import (
     AbstractSet,
     Any,
     Callable,
     Dict,
     Generator,
     Generic,
-    Iterable,
     Mapping,
     NamedTuple,
     Optional,
     Set,
     Type,
     TypeVar,
     Union,
@@ -27,24 +26,23 @@
     Enum as DagsterEnum,
     Field as DagsterField,
 )
 from dagster._config.config_type import (
     Array,
     ConfigFloatInstance,
     ConfigType,
-    EnumValue,
     Noneable,
 )
 from dagster._config.field_utils import config_dictionary_from_values
 from dagster._config.post_process import resolve_defaults
 from dagster._config.pythonic_config.typing_utils import (
     TypecheckAllowPartialResourceInitParams,
 )
 from dagster._config.source import BoolSource, IntSource, StringSource
-from dagster._config.validate import process_config, validate_config
+from dagster._config.validate import validate_config
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.definition_config_schema import (
     CoercableToConfigSchema,
     ConfiguredDefinitionConfigSchema,
     DefinitionConfigSchema,
 )
 from dagster._core.errors import (
@@ -414,32 +412,14 @@
         config=old_field.config_type,
         default_value=new_config_value,
         is_required=False,
         description=old_field.description,
     )
 
 
-def _process_config_values(
-    schema_field: Field, data: Mapping[str, Any], config_obj_name: str
-) -> Mapping[str, Any]:
-    post_processed_config = process_config(
-        schema_field.config_type, config_dictionary_from_values(data, schema_field)
-    )
-
-    if not post_processed_config.success:
-        raise DagsterInvalidConfigError(
-            f"Error while processing {config_obj_name} config ",
-            post_processed_config.errors,
-            data,
-        )
-    assert post_processed_config.value is not None
-
-    return post_processed_config.value or {}
-
-
 def _curry_config_schema(schema_field: Field, data: Any) -> DefinitionConfigSchema:
     """Return a new config schema configured with the passed in data."""
     return DefinitionConfigSchema(_apply_defaults_to_schema_field(schema_field, data))
 
 
 TResValue = TypeVar("TResValue")
 TIOManagerValue = TypeVar("TIOManagerValue", bound=IOManager)
@@ -873,40 +853,29 @@
     def configure_at_launch(cls: "Type[Self]", **kwargs) -> "PartialResource[Self]":
         """Returns a partially initialized copy of the resource, with remaining config fields
         set at runtime.
         """
         return PartialResource(cls, data=kwargs)
 
     def _with_updated_values(
-        self, values: Mapping[str, Any]
+        self, values: Optional[Mapping[str, Any]]
     ) -> "ConfigurableResourceFactory[TResValue]":
         """Returns a new instance of the resource with the given values.
         Used when initializing a resource at runtime.
         """
+        values = check.opt_mapping_param(values, "values", key_type=str)
         # Since Resource extends BaseModel and is a dataclass, we know that the
         # signature of any __init__ method will always consist of the fields
         # of this class. We can therefore safely pass in the values as kwargs.
         out = self.__class__(**{**self._get_non_none_public_field_values(), **values})
         out._state__internal__ = out._state__internal__._replace(  # noqa: SLF001
             resource_context=self._state__internal__.resource_context
         )
         return out
 
-    def _resolve_and_update_env_vars(self) -> "ConfigurableResourceFactory[TResValue]":
-        """Processes the config dictionary to resolve any EnvVar values. This is called at runtime
-        when the resource is initialized, so the user is only shown the error if they attempt to
-        kick off a run relying on this resource.
-
-        Returns a new instance of the resource.
-        """
-        post_processed_data = _process_config_values(
-            self._schema, self._resolved_config_dict, self.__class__.__name__
-        )
-        return self._with_updated_values(post_processed_data)
-
     @contextlib.contextmanager
     def _resolve_and_update_nested_resources(
         self, context: InitResourceContext
     ) -> Generator["ConfigurableResourceFactory[TResValue]", None, None]:
         """Updates any nested resources with the resource values from the context.
         In this case, populating partially configured resources or
         resources that return plain Python types.
@@ -958,27 +927,27 @@
         )
         return copy
 
     def _initialize_and_run(self, context: InitResourceContext) -> TResValue:
         with self._resolve_and_update_nested_resources(context) as has_nested_resource:
             updated_resource = has_nested_resource.with_resource_context(  # noqa: SLF001
                 context
-            )._resolve_and_update_env_vars()
+            )._with_updated_values(context.resource_config)
 
             updated_resource.setup_for_execution(context)
             return updated_resource.create_resource(context)
 
     @contextlib.contextmanager
     def _initialize_and_run_cm(
         self, context: InitResourceContext
     ) -> Generator[TResValue, None, None]:
         with self._resolve_and_update_nested_resources(context) as has_nested_resource:
             updated_resource = has_nested_resource.with_resource_context(  # noqa: SLF001
                 context
-            )._resolve_and_update_env_vars()
+            )._with_updated_values(context.resource_config)
 
             with updated_resource.yield_for_execution(context) as value:
                 yield value
 
     def setup_for_execution(self, context: InitResourceContext) -> None:
         """Optionally override this method to perform any pre-execution steps
         needed before the resource is used in execution.
@@ -1147,15 +1116,17 @@
         data: Dict[str, Any],
     ):
         resource_pointers, _data_without_resources = separate_resource_params(data)
 
         MakeConfigCacheable.__init__(self, data=data, resource_cls=resource_cls)  # type: ignore  # extends BaseModel, takes kwargs
 
         def resource_fn(context: InitResourceContext):
-            instantiated = resource_cls(**context.resource_config, **data)
+            instantiated = resource_cls(
+                **{**data, **context.resource_config}
+            )  # So that collisions are resolved in favor of the latest provided run config
             return instantiated._get_initialize_and_run_fn()(context)  # noqa: SLF001
 
         self._state__internal__ = PartialResourceState(
             # We keep track of any resources we depend on which are not fully configured
             # so that we can retrieve them at runtime
             nested_partial_resources={
                 k: v for k, v in resource_pointers.items() if (not _is_fully_configured(v))
@@ -1560,21 +1531,15 @@
     # no FloatSource, so we just return float
     elif safe_is_subclass(potential_dagster_type, ConstrainedFloat):
         potential_dagster_type = float
     elif safe_is_subclass(potential_dagster_type, ConstrainedInt):
         return IntSource
 
     if safe_is_subclass(potential_dagster_type, Enum):
-        return DagsterEnum(
-            potential_dagster_type.__name__,
-            [
-                EnumValue(v.name, python_value=v.value)
-                for v in cast(Iterable[Enum], potential_dagster_type)
-            ],
-        )
+        return DagsterEnum.from_python_enum_direct_values(potential_dagster_type)
 
     # special case raw python literals to their source equivalents
     if potential_dagster_type is str:
         return StringSource
     elif potential_dagster_type is int:
         return IntSource
     elif potential_dagster_type is bool:
@@ -1780,19 +1745,35 @@
         non_resources={k: v for k, v in data.items() if not is_coercible_to_resource(v)},
     )
 
 
 def _call_resource_fn_with_default(
     stack: contextlib.ExitStack, obj: ResourceDefinition, context: InitResourceContext
 ) -> Any:
+    from dagster._config.validate import process_config
+
     if isinstance(obj.config_schema, ConfiguredDefinitionConfigSchema):
         value = cast(Dict[str, Any], obj.config_schema.resolve_config({}).value)
         context = context.replace_config(value["config"])
     elif obj.config_schema.default_provided:
-        context = context.replace_config(obj.config_schema.default_value)
+        # To explain why we need to process config here;
+        # - The resource available on the init context (context.resource_config) has already been processed
+        # - The nested resource's config has also already been processed, but is only available in the broader run config dictionary.
+        # - The only information we have access to here is the unprocessed default value, so we need to process it a second time.
+        unprocessed_config = obj.config_schema.default_value
+        evr = process_config(
+            {"config": obj.config_schema.config_type}, {"config": unprocessed_config}
+        )
+        if not evr.success:
+            raise DagsterInvalidConfigError(
+                "Error in config for nested resource ",
+                evr.errors,
+                unprocessed_config,
+            )
+        context = context.replace_config(cast(dict, evr.value)["config"])
 
     is_fn_generator = inspect.isgenerator(obj.resource_fn) or isinstance(
         obj.resource_fn, contextlib.ContextDecorator
     )
     if has_at_least_one_parameter(obj.resource_fn):  # type: ignore[unreachable]
         result = cast(ResourceFunctionWithContext, obj.resource_fn)(context)
     else:
```

### Comparing `dagster-1.3.4/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.5/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.5/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.5/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/snap.py` & `dagster-1.3.5/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/source.py` & `dagster-1.3.5/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/stack.py` & `dagster-1.3.5/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/traversal_context.py` & `dagster-1.3.5/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/type_printer.py` & `dagster-1.3.5/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_config/validate.py` & `dagster-1.3.5/dagster/_config/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     create_field_not_defined_error,
     create_field_substitution_collision_error,
     create_fields_not_defined_error,
     create_map_error,
     create_missing_required_field_error,
     create_missing_required_fields_error,
     create_none_not_allowed_error,
+    create_pydantic_env_var_error,
     create_scalar_error,
     create_selector_multiple_fields_error,
     create_selector_multiple_fields_no_field_selected_error,
     create_selector_type_error,
     create_selector_unspecified_value_error,
 )
 from .evaluate_value_result import EvaluateValueResult
@@ -76,14 +77,16 @@
             stack=EvaluationStack(entries=[]),
         ),
         config_value,
     )
 
 
 def _validate_config(context: ValidationContext, config_value: object) -> EvaluateValueResult[Any]:
+    from dagster._config.field_utils import EnvVar, IntEnvVar
+
     check.inst_param(context, "context", ValidationContext)
 
     kind = context.config_type_snap.kind
 
     if kind == ConfigTypeKind.NONEABLE:
         return (
             EvaluateValueResult.for_value(config_value)
@@ -96,14 +99,21 @@
 
     if config_value is None:
         return EvaluateValueResult.for_error(create_none_not_allowed_error(context))
 
     if kind == ConfigTypeKind.SCALAR:
         if not is_config_scalar_valid(context.config_type_snap, config_value):
             return EvaluateValueResult.for_error(create_scalar_error(context, config_value))
+        # If user passes an EnvVar or IntEnvVar to a non-structured run config dictionary, throw explicit error
+        if context.config_type_snap.scalar_kind == ConfigScalarKind.STRING and isinstance(
+            config_value, (EnvVar, IntEnvVar)
+        ):
+            return EvaluateValueResult.for_error(
+                create_pydantic_env_var_error(context, config_value)
+            )
         return EvaluateValueResult.for_value(config_value)
     elif kind == ConfigTypeKind.SELECTOR:
         return validate_selector_config(context, config_value)
     elif kind == ConfigTypeKind.STRICT_SHAPE:
         return validate_shape_config(context, config_value)
     elif kind == ConfigTypeKind.PERMISSIVE_SHAPE:
         return validate_permissive_shape_config(context, config_value)
```

### Comparing `dagster-1.3.4/dagster/_core/assets.py` & `dagster-1.3.5/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/code_pointer.py` & `dagster-1.3.5/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/container_context/config.py` & `dagster-1.3.5/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/debug.py` & `dagster-1.3.5/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/decorator_utils.py` & `dagster-1.3.5/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/__init__.py` & `dagster-1.3.5/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.5/dagster/_core/definitions/asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Optional,
     Sequence,
     Set,
     Union,
     cast,
 )
 
+import pendulum
 import toposort
 
 import dagster._check as check
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.errors import DagsterInvalidInvocationError, DagsterInvariantViolationError
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.selector.subset_selector import DependencyGraph, generate_asset_dep_graph
@@ -651,27 +652,41 @@
         required_multi_asset_keys = self._asset_graph.get_required_multi_asset_keys(asset_key) | {
             asset_key
         }
         level = max(
             self._toposort_level_by_asset_key[required_asset_key]
             for required_asset_key in required_multi_asset_keys
         )
+
+        def _sort_key_for_time_window_partition(
+            partitions_def: TimeWindowPartitionsDefinition,
+        ) -> float:
+            # A sort key such that time window partitions are sorted from oldest to newest
+            return pendulum.instance(
+                datetime.strptime(cast(str, asset_partition.partition_key), partitions_def.fmt),
+                tz=partitions_def.timezone,
+            ).timestamp()
+
+        partitions_def = self._asset_graph.get_partitions_def(asset_key)
         if self._asset_graph.has_self_dependency(asset_key):
-            partitions_def = self._asset_graph.get_partitions_def(asset_key)
             if partitions_def is not None and isinstance(
                 partitions_def, TimeWindowPartitionsDefinition
             ):
-                partition_sort_key = partitions_def.time_window_for_partition_key(
-                    cast(str, asset_partition.partition_key)
-                ).start.timestamp()
+                # sort self dependencies from oldest to newest, as older partitions must exist before
+                # new ones can execute
+                partition_sort_key = _sort_key_for_time_window_partition(partitions_def)
             else:
                 check.failed(
                     "Assets with self-dependencies must have time-window partitions, but"
                     f" {asset_key} does not."
                 )
+        elif isinstance(partitions_def, TimeWindowPartitionsDefinition):
+            # sort non-self dependencies from newest to oldest, as newer partitions are more relevant
+            # than older ones
+            partition_sort_key = -1 * _sort_key_for_time_window_partition(partitions_def)
         else:
             partition_sort_key = None
 
         return ToposortedPriorityQueue.QueueItem(
             level,
             partition_sort_key,
             [
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.5/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_in.py` & `dagster-1.3.5/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.5/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_out.py` & `dagster-1.3.5/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.5/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,42 +29,127 @@
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
     has_one_dimension_time_window_partitioning,
 )
+from dagster._serdes.serdes import whitelist_for_serdes
 from dagster._utils.backcompat import deprecation_warning
 from dagster._utils.schedules import cron_string_iterator
 
 from .asset_selection import AssetGraph, AssetSelection
+from .auto_materialize_condition import (
+    AutoMaterializeCondition,
+    AutoMaterializeDecisionType,
+    DownstreamFreshnessAutoMaterializeCondition,
+    FreshnessAutoMaterializeCondition,
+    MaxMaterializationsExceededAutoMaterializeCondition,
+    MissingAutoMaterializeCondition,
+    ParentMaterializedAutoMaterializeCondition,
+    ParentOutdatedAutoMaterializeCondition,
+)
 from .decorators.sensor_decorator import sensor
 from .partition import PartitionsDefinition, PartitionsSubset
 from .run_request import RunRequest
 from .sensor_definition import DefaultSensorStatus, SensorDefinition
 from .utils import check_valid_name
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
 
+@whitelist_for_serdes
+class AutoMaterializeAssetEvaluation(NamedTuple):
+    """Represents the results of the auto-materialize logic for a single asset.
+
+    Properties:
+        asset_key (AssetKey): The asset key that was evaluated.
+        conditions: The conditions that impact if the asset should be materialized, skipped, or
+            discarded. If the asset is partitioned, this will be a list of tuples, where the first
+            element is the condition and the second element is the set of partitions that the
+            condition applies to.
+    """
+
+    asset_key: AssetKey
+    conditions: Union[
+        Sequence[AutoMaterializeCondition],
+        Sequence[Tuple[AutoMaterializeCondition, PartitionsSubset]],
+    ]
+    num_requested: int
+    num_skipped: int
+    num_discarded: int
+
+    @staticmethod
+    def from_conditions(
+        asset_graph: AssetGraph,
+        asset_key: AssetKey,
+        conditions_by_asset_partition: Mapping[
+            AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]
+        ],
+    ) -> "AutoMaterializeAssetEvaluation":
+        num_requested = 0
+        num_skipped = 0
+        num_discarded = 0
+
+        for conditions in conditions_by_asset_partition.values():
+            decision_types = {condition.decision_type for condition in conditions}
+            if AutoMaterializeDecisionType.DISCARD in decision_types:
+                num_discarded += 1
+            elif AutoMaterializeDecisionType.SKIP in decision_types:
+                num_skipped += 1
+            else:
+                check.invariant(AutoMaterializeDecisionType.MATERIALIZE in decision_types)
+                num_requested += 1
+
+        partitions_def = asset_graph.get_partitions_def(asset_key)
+        if partitions_def is None:
+            return AutoMaterializeAssetEvaluation(
+                asset_key=asset_key,
+                conditions=list(set().union(*conditions_by_asset_partition.values())),
+                num_requested=num_requested,
+                num_skipped=num_skipped,
+                num_discarded=num_discarded,
+            )
+        else:
+            partition_keys_by_condition = defaultdict(set)
+
+            for asset_partition, conditions in conditions_by_asset_partition.items():
+                for condition in conditions:
+                    partition_keys_by_condition[condition].add(
+                        check.not_none(asset_partition.partition_key)
+                    )
+
+            return AutoMaterializeAssetEvaluation(
+                asset_key=asset_key,
+                conditions=[
+                    (condition, partitions_def.empty_subset().with_partition_keys(partition_keys))
+                    for condition, partition_keys in partition_keys_by_condition.items()
+                ],
+                num_requested=num_requested,
+                num_skipped=num_skipped,
+                num_discarded=num_discarded,
+            )
+
+
 def get_implicit_auto_materialize_policy(
     asset_graph: AssetGraph, asset_key: AssetKey
 ) -> Optional[AutoMaterializePolicy]:
     """For backcompat with pre-auto materialize policy graphs, assume a default scope of 1 day."""
     auto_materialize_policy = asset_graph.get_auto_materialize_policy(asset_key)
     if auto_materialize_policy is None:
         return AutoMaterializePolicy(
             on_missing=True,
             on_new_parent_data=not bool(
                 asset_graph.get_downstream_freshness_policies(asset_key=asset_key)
             ),
             for_freshness=True,
             time_window_partition_scope_minutes=24 * 60,
+            max_materializations_per_minute=None,
         )
     return auto_materialize_policy
 
 
 def reconciliation_window_for_time_window_partitions(
     partitions_def: Union[TimeWindowPartitionsDefinition, MultiPartitionsDefinition],
     time_window_partition_scope: Optional[datetime.timedelta],
@@ -355,25 +440,34 @@
             the same events the next time this function is called.
     """
     result_asset_partitions: Set[AssetKeyPartitionKey] = set()
     result_latest_storage_id = latest_storage_id
 
     for asset_key in target_asset_keys_and_parents:
         if asset_graph.is_source(asset_key):
-            if asset_graph.is_observable(asset_key) and instance_queryer.new_version_exists(
-                observable_source_asset_key=asset_key, after_cursor=latest_storage_id
-            ):
-                for child in asset_graph.get_children_partitions(
-                    dynamic_partitions_store=instance_queryer,
-                    current_time=instance_queryer.evaluation_time,
-                    asset_key=asset_key,
-                    partition_key=None,
-                ):
-                    if child.asset_key in target_asset_keys:
-                        result_asset_partitions.add(child)
+            if asset_graph.is_observable(asset_key):
+                # for observable sources, find the storage id of the latest version record that differs
+                # from the previous version (if any)
+                new_version_storage_id = instance_queryer.new_version_storage_id(
+                    observable_source_asset_key=asset_key, after_cursor=latest_storage_id
+                )
+                if new_version_storage_id is not None:
+                    if (
+                        result_latest_storage_id is None
+                        or new_version_storage_id > result_latest_storage_id
+                    ):
+                        result_latest_storage_id = new_version_storage_id
+                    for child in asset_graph.get_children_partitions(
+                        dynamic_partitions_store=instance_queryer,
+                        current_time=instance_queryer.evaluation_time,
+                        asset_key=asset_key,
+                        partition_key=None,
+                    ):
+                        if child.asset_key in target_asset_keys:
+                            result_asset_partitions.add(child)
 
             continue
 
         partitions_def = asset_graph.get_partitions_def(asset_key)
         latest_record = instance_queryer.get_latest_materialization_record(
             asset_key, after_cursor=latest_storage_id
         )
@@ -506,39 +600,49 @@
     return (
         never_materialized_or_requested,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     )
 
 
-def determine_asset_partitions_to_reconcile(
+def determine_asset_partitions_to_auto_materialize(
     instance_queryer: "CachingInstanceQueryer",
     cursor: AssetReconciliationCursor,
     target_asset_keys: AbstractSet[AssetKey],
     target_asset_keys_and_parents: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
+    current_time: datetime.datetime,
+    conditions_by_asset_partition_for_freshness: Mapping[
+        AssetKeyPartitionKey, Set[AutoMaterializeCondition]
+    ],
 ) -> Tuple[
-    AbstractSet[AssetKeyPartitionKey],
+    Mapping[AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]],
     AbstractSet[AssetKey],
     Mapping[AssetKey, AbstractSet[str]],
     Optional[int],
 ]:
+    materialization_counts_by_asset_key: Dict[AssetKey, int] = defaultdict(int)
     evaluation_time = instance_queryer.evaluation_time
 
     (
         never_materialized_or_requested_roots,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     ) = find_never_materialized_or_requested_root_asset_partitions(
         instance_queryer=instance_queryer,
         cursor=cursor,
         target_asset_keys=target_asset_keys,
         asset_graph=asset_graph,
     )
 
+    # initialize conditions with the conditions_for_freshness
+    conditions_by_asset_partition: Dict[
+        AssetKeyPartitionKey, Set[AutoMaterializeCondition]
+    ] = defaultdict(set, conditions_by_asset_partition_for_freshness)
+
     # a filter for eliminating candidates
     def can_reconcile_candidate(candidate: AssetKeyPartitionKey) -> bool:
         auto_materialize_policy = get_implicit_auto_materialize_policy(
             asset_graph=asset_graph, asset_key=candidate.asset_key
         )
         partitions_def = asset_graph.get_partitions_def(candidate.asset_key)
 
@@ -580,26 +684,31 @@
         asset_graph=asset_graph,
         instance=instance_queryer.instance,
     )
 
     def parents_will_be_reconciled(
         asset_graph: AssetGraph,
         candidate: AssetKeyPartitionKey,
-        to_reconcile: AbstractSet[AssetKeyPartitionKey],
     ) -> bool:
         from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 
         for parent in asset_graph.get_parents_partitions(
             instance_queryer, evaluation_time, candidate.asset_key, candidate.partition_key
         ):
             if instance_queryer.is_reconciled(asset_partition=parent, asset_graph=asset_graph):
                 continue
 
             if not (
-                parent in to_reconcile
+                (
+                    parent in conditions_by_asset_partition
+                    and all(
+                        condition.decision_type == AutoMaterializeDecisionType.MATERIALIZE
+                        for condition in conditions_by_asset_partition[parent]
+                    )
+                )
                 # if they don't have the same partitioning, then we can't launch a run that
                 # targets both, so we need to wait until the parent is reconciled before
                 # launching a run for the child
                 and asset_graph.have_same_partitioning(parent.asset_key, candidate.asset_key)
                 and parent.partition_key == candidate.partition_key
             ):
                 return False
@@ -610,30 +719,45 @@
                 if asset_graph.get_repository_handle(
                     candidate.asset_key
                 ) is not asset_graph.get_repository_handle(parent.asset_key):
                     return False
 
         return True
 
-    def should_reconcile_candidate(candidate: AssetKeyPartitionKey) -> bool:
+    def conditions_for_candidate(
+        candidate: AssetKeyPartitionKey,
+    ) -> AbstractSet[AutoMaterializeCondition]:
         auto_materialize_policy = get_implicit_auto_materialize_policy(
             asset_graph=asset_graph, asset_key=candidate.asset_key
         )
+        conditions = set()
         if auto_materialize_policy is None:
-            return False
+            return conditions
+        elif auto_materialize_policy.on_missing and not instance_queryer.materialization_exists(
+            asset_partition=candidate
+        ):
+            conditions.add(MissingAutoMaterializeCondition())
+        elif auto_materialize_policy.on_new_parent_data and not instance_queryer.is_reconciled(
+            asset_partition=candidate, asset_graph=asset_graph
+        ):
+            conditions.add(ParentMaterializedAutoMaterializeCondition())
 
-        return (
-            auto_materialize_policy.on_missing
-            and not instance_queryer.materialization_exists(asset_partition=candidate)
-        ) or (
-            auto_materialize_policy.on_new_parent_data
-            and not instance_queryer.is_reconciled(
-                asset_partition=candidate, asset_graph=asset_graph
-            )
-        )
+        # if there are any conditions that would cause us to materialize this candidate unit, we
+        # need to ensure they would not cause us to exceed the rate limit
+        if conditions:
+            if (
+                auto_materialize_policy.max_materializations_per_minute is not None
+                and materialization_counts_by_asset_key[candidate.asset_key]
+                >= auto_materialize_policy.max_materializations_per_minute
+            ):
+                conditions.add(MaxMaterializationsExceededAutoMaterializeCondition())
+            else:
+                materialization_counts_by_asset_key[candidate.asset_key] += 1
+
+        return conditions
 
     def should_reconcile(
         asset_graph: AssetGraph,
         candidates_unit: Iterable[AssetKeyPartitionKey],
         to_reconcile: AbstractSet[AssetKeyPartitionKey],
     ) -> bool:
         if any(
@@ -643,30 +767,47 @@
             or candidate in backfill_target_asset_graph_subset
             # do not reconcile assets if they are not in the target selection
             or candidate.asset_key not in target_asset_keys
             for candidate in candidates_unit
         ):
             return False
 
-        return all(
-            parents_will_be_reconciled(asset_graph, candidate, to_reconcile)
-            for candidate in candidates_unit
-        ) and any(should_reconcile_candidate(candidate) for candidate in candidates_unit)
+        if all(parents_will_be_reconciled(asset_graph, candidate) for candidate in candidates_unit):
+            unit_conditions = set().union(
+                *(conditions_for_candidate(candidate) for candidate in candidates_unit)
+            )
+            # all candidates in the unit share the same conditions
+            if unit_conditions:
+                for candidate in candidates_unit:
+                    conditions_by_asset_partition[candidate].update(unit_conditions)
+                # all conditions be of type MATERIALIZE for an asset partition to be materialized
+                return all(
+                    condition.decision_type == AutoMaterializeDecisionType.MATERIALIZE
+                    for condition in unit_conditions
+                )
+            return False
+        else:
+            for candidate in candidates_unit:
+                conditions_by_asset_partition[candidate].add(
+                    ParentOutdatedAutoMaterializeCondition()
+                )
+        return False
 
-    to_reconcile = asset_graph.bfs_filter_asset_partitions(
+    # will update conditions
+    asset_graph.bfs_filter_asset_partitions(
         instance_queryer,
         lambda candidates_unit, to_reconcile: should_reconcile(
             asset_graph, candidates_unit, to_reconcile
         ),
         set(itertools.chain(never_materialized_or_requested_roots, stale_candidates)),
         evaluation_time,
     )
 
     return (
-        to_reconcile,
+        conditions_by_asset_partition,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
         latest_storage_id,
     )
 
 
 def get_execution_period_for_policy(
@@ -696,61 +837,70 @@
         return pendulum.Period(
             # we don't want to execute this too frequently
             start=effective_data_time + 0.9 * freshness_policy.maximum_lag_delta,
             end=max(effective_data_time + freshness_policy.maximum_lag_delta, current_time),
         )
 
 
-def get_execution_period_for_policies(
+def get_execution_period_and_conditions_for_policies(
+    local_policy: Optional[FreshnessPolicy],
     policies: AbstractSet[FreshnessPolicy],
     effective_data_time: Optional[datetime.datetime],
     current_time: datetime.datetime,
-) -> Optional[pendulum.Period]:
+) -> Tuple[Optional[pendulum.Period], AbstractSet[AutoMaterializeCondition]]:
     """Determines a range of times for which you can kick off an execution of this asset to solve
     the most pressing constraint, alongside a maximum number of additional constraints.
     """
     merged_period = None
-    for period in sorted(
+    conditions = set()
+    for period, policy in sorted(
         (
-            get_execution_period_for_policy(policy, effective_data_time, current_time)
+            (get_execution_period_for_policy(policy, effective_data_time, current_time), policy)
             for policy in policies
         ),
         # sort execution periods by most pressing
-        key=lambda period: period.end,
+        key=lambda pp: pp[0].end,
     ):
         if merged_period is None:
             merged_period = period
         elif period.start <= merged_period.end:
             merged_period = pendulum.Period(
                 start=max(period.start, merged_period.start),
                 end=period.end,
             )
         else:
             break
 
-    return merged_period
+        if policy == local_policy:
+            conditions.add(FreshnessAutoMaterializeCondition())
+        else:
+            conditions.add(DownstreamFreshnessAutoMaterializeCondition())
 
+    return merged_period, conditions
 
-def determine_asset_partitions_to_reconcile_for_freshness(
+
+def determine_asset_partitions_to_auto_materialize_for_freshness(
     data_time_resolver: "CachingDataTimeResolver",
     asset_graph: AssetGraph,
     target_asset_keys: AbstractSet[AssetKey],
     target_asset_keys_and_parents: AbstractSet[AssetKey],
     current_time: datetime.datetime,
-) -> AbstractSet[AssetKeyPartitionKey]:
+) -> Mapping[AssetKeyPartitionKey, Set[AutoMaterializeCondition]]:
     """Returns a set of AssetKeyPartitionKeys to materialize in order to abide by the given
     FreshnessPolicies, as well as a set of AssetKeyPartitionKeys which will be materialized at
     some point within the plan window.
 
     Attempts to minimize the total number of asset executions.
     """
     from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 
     # now we have a full set of constraints, we can find solutions for them as we move down
-    to_materialize: Set[AssetKeyPartitionKey] = set()
+    conditions_by_asset_partition: Mapping[
+        AssetKeyPartitionKey, Set[AutoMaterializeCondition]
+    ] = defaultdict(set)
     waiting_to_materialize: Set[AssetKey] = set()
     expected_data_time_by_key: Dict[AssetKey, Optional[datetime.datetime]] = {}
 
     for level in asset_graph.toposort_asset_keys():
         for key in level:
             if (
                 key not in target_asset_keys_and_parents
@@ -767,35 +917,42 @@
                 continue
 
             # if we're going to materialize a parent of this asset that's in a different repository,
             # then we need to wait
             if isinstance(asset_graph, ExternalAssetGraph):
                 repo = asset_graph.get_repository_handle(key)
                 if any(
-                    AssetKeyPartitionKey(p, None) in to_materialize
+                    AssetKeyPartitionKey(p, None) in conditions_by_asset_partition
                     and asset_graph.get_repository_handle(p) is not repo
                     for p in parents
                 ):
                     waiting_to_materialize.add(key)
                     continue
 
             # figure out the current contents of this asset with respect to its constraints
             current_data_time = data_time_resolver.get_current_data_time(key, current_time)
 
             # figure out the expected data time of this asset if it were to be executed on this tick
-            expected_data_time = min(
-                (
-                    cast(datetime.datetime, expected_data_time_by_key[k])
-                    for k in parents
-                    if k in expected_data_time_by_key and expected_data_time_by_key[k] is not None
-                ),
-                default=current_time,
+            # for root assets, this would just be the current time
+            expected_data_time = (
+                min(
+                    (
+                        cast(datetime.datetime, expected_data_time_by_key[k])
+                        for k in parents
+                        if k in expected_data_time_by_key
+                        and expected_data_time_by_key[k] is not None
+                    ),
+                    default=None,
+                )
+                if asset_graph.has_non_source_parents(key)
+                else current_time
             )
 
-            if key in target_asset_keys:
+            # currently, freshness logic has no effect on partitioned assets
+            if key in target_asset_keys and not asset_graph.is_partitioned(key):
                 # calculate the data times you would expect after all currently-executing runs
                 # were to successfully complete
                 in_progress_data_time = data_time_resolver.get_in_progress_data_time(
                     key, current_time
                 )
 
                 # calculate the data times you would have expected if the most recent run succeeded
@@ -806,53 +963,70 @@
                 effective_data_time = max(
                     filter(None, (current_data_time, in_progress_data_time, failed_data_time)),
                     default=None,
                 )
 
                 # figure out a time period that you can execute this asset within to solve a maximum
                 # number of constraints
-                execution_period = get_execution_period_for_policies(
+                (
+                    execution_period,
+                    execution_conditions,
+                ) = get_execution_period_and_conditions_for_policies(
+                    local_policy=asset_graph.freshness_policies_by_key.get(key),
                     policies=asset_graph.get_downstream_freshness_policies(asset_key=key),
                     effective_data_time=effective_data_time,
                     current_time=current_time,
                 )
             else:
-                execution_period = None
+                execution_period, execution_conditions = None, set()
 
-            # a key may already be in to_materialize by the time we get here if a required
+            # a key may already be in conditions by the time we get here if a required
             # neighbor was selected to be updated
-            asset_key_partition_key = AssetKeyPartitionKey(key, None)
-            if asset_key_partition_key in to_materialize:
+            asset_partition = AssetKeyPartitionKey(key, None)
+            if asset_partition in conditions_by_asset_partition and all(
+                condition.decision_type == AutoMaterializeDecisionType.MATERIALIZE
+                for condition in conditions_by_asset_partition[asset_partition]
+            ):
                 expected_data_time_by_key[key] = expected_data_time
             elif (
                 execution_period is not None
                 and execution_period.start <= current_time
                 and expected_data_time is not None
                 and expected_data_time >= execution_period.start
+                and all(
+                    condition.decision_type == AutoMaterializeDecisionType.MATERIALIZE
+                    for condition in execution_conditions
+                )
             ):
-                to_materialize.add(asset_key_partition_key)
                 expected_data_time_by_key[key] = expected_data_time
+                conditions_by_asset_partition[asset_partition].update(execution_conditions)
                 # all required neighbors will be updated on the same tick
                 for required_key in asset_graph.get_required_multi_asset_keys(key):
-                    to_materialize.add(AssetKeyPartitionKey(required_key, None))
+                    conditions_by_asset_partition[
+                        (AssetKeyPartitionKey(required_key, None))
+                    ].update(execution_conditions)
             else:
                 # if downstream assets consume this, they should expect data time equal to the
                 # current time for this asset, as it's not going to be updated
                 expected_data_time_by_key[key] = current_data_time
 
-    return to_materialize
+    return conditions_by_asset_partition
 
 
 def reconcile(
     asset_graph: AssetGraph,
     target_asset_keys: AbstractSet[AssetKey],
     instance: "DagsterInstance",
     cursor: AssetReconciliationCursor,
     run_tags: Optional[Mapping[str, str]],
-):
+) -> Tuple[
+    Sequence[RunRequest],
+    AssetReconciliationCursor,
+    Sequence[AutoMaterializeAssetEvaluation],
+]:
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
     current_time = pendulum.now("UTC")
 
     instance_queryer = CachingInstanceQueryer(instance=instance, evaluation_time=current_time)
 
     target_parent_asset_keys = {
@@ -865,51 +1039,64 @@
     # fetch some data in advance to batch some queries
     target_asset_keys_and_parents_list = list(target_asset_keys_and_parents)
     instance_queryer.prefetch_asset_records(target_asset_keys_and_parents_list)
     instance_queryer.prefetch_asset_partition_counts(
         target_asset_keys_and_parents_list, after_cursor=cursor.latest_storage_id
     )
 
-    asset_partitions_to_reconcile_for_freshness = (
-        determine_asset_partitions_to_reconcile_for_freshness(
+    conditions_by_asset_partition_for_freshness = (
+        determine_asset_partitions_to_auto_materialize_for_freshness(
             data_time_resolver=CachingDataTimeResolver(
                 instance_queryer=instance_queryer, asset_graph=asset_graph
             ),
             asset_graph=asset_graph,
             target_asset_keys=target_asset_keys,
             target_asset_keys_and_parents=target_asset_keys_and_parents,
             current_time=current_time,
         )
     )
 
     (
-        asset_partitions_to_reconcile,
+        conditions_by_asset_partition,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
         latest_storage_id,
-    ) = determine_asset_partitions_to_reconcile(
+    ) = determine_asset_partitions_to_auto_materialize(
         instance_queryer=instance_queryer,
         asset_graph=asset_graph,
         cursor=cursor,
         target_asset_keys=target_asset_keys,
         target_asset_keys_and_parents=target_asset_keys_and_parents,
+        current_time=current_time,
+        conditions_by_asset_partition_for_freshness=conditions_by_asset_partition_for_freshness,
     )
 
     run_requests = build_run_requests(
-        asset_partitions_to_reconcile | asset_partitions_to_reconcile_for_freshness,
-        asset_graph,
-        run_tags,
+        asset_partitions={
+            asset_partition
+            for asset_partition, conditions in conditions_by_asset_partition.items()
+            if all(
+                condition.decision_type == AutoMaterializeDecisionType.MATERIALIZE
+                for condition in conditions
+            )
+        },
+        asset_graph=asset_graph,
+        run_tags=run_tags,
     )
 
-    return run_requests, cursor.with_updates(
-        latest_storage_id=latest_storage_id,
-        run_requests=run_requests,
-        asset_graph=asset_graph,
-        newly_materialized_root_asset_keys=newly_materialized_root_asset_keys,
-        newly_materialized_root_partitions_by_asset_key=newly_materialized_root_partitions_by_asset_key,
+    return (
+        run_requests,
+        cursor.with_updates(
+            latest_storage_id=latest_storage_id,
+            run_requests=run_requests,
+            asset_graph=asset_graph,
+            newly_materialized_root_asset_keys=newly_materialized_root_asset_keys,
+            newly_materialized_root_partitions_by_asset_key=newly_materialized_root_partitions_by_asset_key,
+        ),
+        build_auto_materialize_asset_evaluations(asset_graph, conditions_by_asset_partition),
     )
 
 
 def build_run_requests(
     asset_partitions: Iterable[AssetKeyPartitionKey],
     asset_graph: AssetGraph,
     run_tags: Optional[Mapping[str, str]],
@@ -947,14 +1134,35 @@
                     tags=tags,
                 )
             )
 
     return run_requests
 
 
+def build_auto_materialize_asset_evaluations(
+    asset_graph: AssetGraph,
+    conditions_by_asset_partition: Mapping[
+        AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]
+    ],
+) -> Sequence[AutoMaterializeAssetEvaluation]:
+    """Bundles up the conditions into AutoMaterializeAssetEvaluations."""
+    conditions_by_asset_key: Dict[
+        AssetKey, Dict[AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]]
+    ] = defaultdict(dict)
+
+    # split into sub-dictionaries that hold only the conditions specific to each asset
+    for asset_partition, conditions in conditions_by_asset_partition.items():
+        conditions_by_asset_key[asset_partition.asset_key][asset_partition] = conditions
+
+    return [
+        AutoMaterializeAssetEvaluation.from_conditions(asset_graph, asset_key, conditions)
+        for asset_key, conditions in conditions_by_asset_key.items()
+    ]
+
+
 @experimental
 def build_asset_reconciliation_sensor(
     asset_selection: AssetSelection,
     name: str = "asset_reconciliation_sensor",
     minimum_interval_seconds: Optional[int] = None,
     description: Optional[str] = None,
     default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
@@ -1091,15 +1299,15 @@
                     " an AutoMaterializePolicy set. This asset will be automatically materialized"
                     " by the AssetDaemon, and should not be passed to this sensor. It's"
                     " recommended to remove this sensor once you have migrated to the"
                     " AutoMaterializePolicy api."
                 ),
             )
 
-        run_requests, updated_cursor = reconcile(
+        run_requests, updated_cursor, _ = reconcile(
             asset_graph=asset_graph,
             target_asset_keys=target_asset_keys,
             instance=context.instance,
             cursor=cursor,
             run_tags=run_tags,
         )
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.5/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.5/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/assets.py` & `dagster-1.3.5/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/assets_job.py` & `dagster-1.3.5/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.5/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/composition.py` & `dagster-1.3.5/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/config.py` & `dagster-1.3.5/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/configurable.py` & `dagster-1.3.5/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/data_time.py` & `dagster-1.3.5/dagster/_core/definitions/data_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dagster._core.definitions.time_window_partitions import (
     TimeWindowPartitionsDefinition,
     TimeWindowPartitionsSubset,
 )
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.event_api import EventLogRecord
 from dagster._core.storage.dagster_run import FINISHED_STATUSES, DagsterRunStatus, RunsFilter
-from dagster._utils import make_hashable
+from dagster._utils import datetime_as_float, make_hashable
 from dagster._utils.cached_method import cached_method
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
 
 class CachingDataTimeResolver:
     _instance_queryer: CachingInstanceQueryer
     _asset_graph: AssetGraph
@@ -425,15 +425,15 @@
         if (
             latest_materialization is not None
             and latest_materialization.run_id == latest_run_record.dagster_run.run_id
         ):
             return current_data_time
 
         run_failure_time = datetime.datetime.utcfromtimestamp(
-            latest_run_record.end_time or latest_run_record.create_timestamp.timestamp()
+            latest_run_record.end_time or datetime_as_float(latest_run_record.create_timestamp)
         ).replace(tzinfo=datetime.timezone.utc)
         return self._get_in_progress_data_time_in_run(
             run_id=run_id, asset_key=asset_key, current_time=run_failure_time
         )
 
     ####################
     # MAIN METHODS
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/data_version.py` & `dagster-1.3.5/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.5/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.5/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.5/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/dependency.py` & `dagster-1.3.5/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/events.py` & `dagster-1.3.5/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.5/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.5/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.5/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.5/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.5/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.5/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.5/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/inference.py` & `dagster-1.3.5/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/input.py` & `dagster-1.3.5/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.5/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/job_base.py` & `dagster-1.3.5/dagster/_core/definitions/job_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     @property
     @abstractmethod
     def asset_selection(self) -> Optional[AbstractSet[AssetKey]]:
         pass
 
     @property
-    def solids_to_execute(self) -> Optional[AbstractSet[str]]:
+    def resolved_op_selection(self) -> Optional[AbstractSet[str]]:
         return set(self.op_selection) if self.op_selection else None
 
 
 class InMemoryJob(IJob):
     def __init__(
         self,
         job_def: "JobDefinition",
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/job_definition.py` & `dagster-1.3.5/dagster/_core/definitions/job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -961,14 +961,18 @@
     def op_selection(self) -> Optional[AbstractSet[str]]:
         return set(self.op_selection_data.op_selection) if self.op_selection_data else None
 
     @property
     def asset_selection(self) -> Optional[AbstractSet[AssetKey]]:
         return self.asset_selection_data.asset_selection if self.asset_selection_data else None
 
+    @property
+    def resolved_op_selection(self) -> Optional[AbstractSet[str]]:
+        return self.op_selection_data.resolved_op_selection if self.op_selection_data else None
+
 
 def _swap_default_io_man(resources: Mapping[str, ResourceDefinition], job: JobDefinition):
     """Used to create the user facing experience of the default io_manager
     switching to in-memory when using execute_in_process.
     """
     from dagster._core.storage.mem_io_manager import mem_io_manager
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.5/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.5/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.5/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/materialize.py` & `dagster-1.3.5/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.5/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.5/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.5/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.5/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/node_container.py` & `dagster-1.3.5/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/node_definition.py` & `dagster-1.3.5/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/observe.py` & `dagster-1.3.5/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/op_definition.py` & `dagster-1.3.5/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.5/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/op_selection.py` & `dagster-1.3.5/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/output.py` & `dagster-1.3.5/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/partition.py` & `dagster-1.3.5/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.5/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.5/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/policy.py` & `dagster-1.3.5/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.5/dagster/_core/definitions/reconstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,29 +254,28 @@
     # This allows repeated calls to get_definition in execution paths to not reload the job
     @lru_cache(maxsize=1)
     def get_definition(self) -> JobDefinition:
         return self.repository.get_definition().get_maybe_subset_job_def(
             self.job_name,
             self.op_selection,
             self.asset_selection,
-            self.solids_to_execute,
         )
 
     def get_reconstructable_repository(self) -> ReconstructableRepository:
         return self.repository
 
     def get_subset(
         self,
         *,
         op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ) -> Self:
         if op_selection and asset_selection:
             check.failed(
-                "solid_selection and asset_selection cannot both be provided as arguments",
+                "op_selection and asset_selection cannot both be provided as arguments",
             )
         op_selection = set(op_selection) if op_selection else None
         return ReconstructableJob(
             repository=self.repository,
             job_name=self.job_name,
             op_selection=op_selection,
             asset_selection=asset_selection,
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.5/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.5/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,14 @@
         return None
 
     def get_maybe_subset_job_def(
         self,
         job_name: str,
         op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
-        solids_to_execute: Optional[AbstractSet[str]] = None,
     ):
         defn = self.get_job(job_name)
         return defn.get_subset(op_selection=op_selection, asset_selection=asset_selection)
 
     @public
     def load_asset_value(
         self,
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.5/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.5/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.5/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.5/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.5/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.5/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/run_config.py` & `dagster-1.3.5/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.5/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/run_request.py` & `dagster-1.3.5/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.5/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.5/dagster/_core/definitions/schedule_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
             )
 
         if job is not None:
             self._target: Union[DirectTarget, RepoRelativeTarget] = DirectTarget(job)
         else:
             self._target = RepoRelativeTarget(
                 job_name=check.str_param(job_name, "job_name"),
-                solid_selection=None,
+                op_selection=None,
             )
 
         if name:
             self._name = check_valid_name(name)
         elif job_name:
             self._name = job_name + "_schedule"
         elif job:
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.5/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/selector.py` & `dagster-1.3.5/dagster/_core/definitions/selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,69 @@
-from typing import NamedTuple, Optional, Sequence
+from typing import AbstractSet, Iterable, NamedTuple, Optional, Sequence
+
+from typing_extensions import Self
 
 import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.repository_definition import SINGLETON_REPOSITORY_NAME
 from dagster._serdes import create_snapshot_id, whitelist_for_serdes
 
 
 class JobSubsetSelector(
     NamedTuple(
         "_JobSubsetSelector",
         [
             ("location_name", str),
             ("repository_name", str),
             ("job_name", str),
-            ("solid_selection", Optional[Sequence[str]]),
-            ("asset_selection", Optional[Sequence[AssetKey]]),
+            ("op_selection", Optional[Sequence[str]]),
+            ("asset_selection", Optional[AbstractSet[AssetKey]]),
         ],
     )
 ):
     """The information needed to resolve a job within a host process."""
 
     def __new__(
         cls,
         location_name: str,
         repository_name: str,
         job_name: str,
-        solid_selection: Optional[Sequence[str]],
-        asset_selection: Optional[Sequence[AssetKey]] = None,
+        op_selection: Optional[Sequence[str]],
+        asset_selection: Optional[Iterable[AssetKey]] = None,
     ):
+        asset_selection = set(asset_selection) if asset_selection else None
         return super(JobSubsetSelector, cls).__new__(
             cls,
             location_name=check.str_param(location_name, "location_name"),
             repository_name=check.str_param(repository_name, "repository_name"),
             job_name=check.str_param(job_name, "job_name"),
-            solid_selection=check.opt_nullable_sequence_param(
-                solid_selection, "solid_selection", str
-            ),
-            asset_selection=check.opt_nullable_sequence_param(
+            op_selection=check.opt_nullable_sequence_param(op_selection, "op_selection", str),
+            asset_selection=check.opt_nullable_set_param(
                 asset_selection, "asset_selection", AssetKey
             ),
         )
 
     def to_graphql_input(self):
         return {
             "repositoryLocationName": self.location_name,
             "repositoryName": self.repository_name,
             "pipelineName": self.job_name,
-            "solidSelection": self.solid_selection,
+            "solidSelection": self.op_selection,
         }
 
-    def with_solid_selection(self, solid_selection):
+    def with_op_selection(self, op_selection: Optional[Sequence[str]]) -> Self:
         check.invariant(
-            self.solid_selection is None,
-            "Can not invoke with_solid_selection when solid_selection={} is already set".format(
-                solid_selection
+            self.op_selection is None,
+            (
+                f"Can not invoke with_op_selection when op_selection={self.op_selection} is"
+                " already set"
             ),
         )
         return JobSubsetSelector(
-            self.location_name, self.repository_name, self.job_name, solid_selection
+            self.location_name, self.repository_name, self.job_name, op_selection
         )
 
 
 @whitelist_for_serdes
 class JobSelector(
     NamedTuple(
         "_JobSelector", [("location_name", str), ("repository_name", str), ("job_name", str)]
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.5/dagster/_core/definitions/sensor_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
         jobs = jobs if jobs else [job] if job else None
 
         targets: Optional[List[Union[RepoRelativeTarget, DirectTarget]]] = None
         if job_name:
             targets = [
                 RepoRelativeTarget(
                     job_name=check.str_param(job_name, "job_name"),
-                    solid_selection=None,
+                    op_selection=None,
                 )
             ]
         elif job:
             targets = [DirectTarget(job)]
         elif jobs:
             targets = [DirectTarget(job) for job in jobs]
         elif asset_selection:
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/source_asset.py` & `dagster-1.3.5/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.5/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/target.py` & `dagster-1.3.5/dagster/_core/definitions/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class RepoRelativeTarget(NamedTuple):
     """The thing to be executed by a schedule or sensor, selecting by name a job in the same repository.
     """
 
     job_name: str
-    solid_selection: Optional[Sequence[str]]
+    op_selection: Optional[Sequence[str]]
 
 
 class DirectTarget(
     NamedTuple(
         "_DirectTarget",
         [("target", ExecutableDefinition)],
     )
@@ -49,13 +49,13 @@
         )
 
     @property
     def job_name(self) -> str:
         return self.target.name
 
     @property
-    def solid_selection(self):
+    def op_selection(self):
         # open question on how to direct target subset job
         return None
 
     def load(self) -> ExecutableDefinition:
         return self.target
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.5/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,16 @@
         if (start_offset != 0 or end_offset != 0) and (
             from_partitions_def.cron_schedule != to_partitions_def.cron_schedule
         ):
             raise DagsterInvalidDefinitionError(
                 "Can't use the start_offset or end_offset parameters of"
                 " TimeWindowPartitionMapping when the cron schedule of the upstream"
                 " PartitionsDefinition is different than the cron schedule of the downstream"
-                " one."
+                f" one. Attempted to map from cron schedule '{from_partitions_def.cron_schedule}' "
+                f"to cron schedule '{to_partitions_def.cron_schedule}'."
             )
 
         if to_partitions_def.timezone != from_partitions_def.timezone:
             raise DagsterInvalidDefinitionError("Timezones don't match")
 
         # skip fancy mapping logic in the simple case
         if from_partitions_def == to_partitions_def and start_offset == 0 and end_offset == 0:
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.5/dagster/_core/definitions/time_window_partitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 class TimeWindowPartitionsDefinition(
     PartitionsDefinition,
     NamedTuple(
         "_TimeWindowPartitionsDefinition",
         [
             ("start", PublicAttr[datetime]),
             ("timezone", PublicAttr[str]),
+            ("end", PublicAttr[Optional[datetime]]),
             ("fmt", PublicAttr[str]),
             ("end_offset", PublicAttr[int]),
             ("cron_schedule", PublicAttr[str]),
         ],
     ),
 ):
     r"""A set of partitions where each partitions corresponds to a time window.
@@ -88,25 +89,27 @@
     Args:
         cron_schedule (str): Determines the bounds of the time windows.
         start (datetime): The first partition in the set will start on at the first cron_schedule
             tick that is equal to or after this value.
         timezone (Optional[str]): The timezone in which each time should exist.
             Supported strings for timezones are the ones provided by the
             `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
+        end (datetime): The last partition (excluding) in the set.
         fmt (str): The date format to use for partition_keys.
         end_offset (int): Extends the partition set by a number of partitions equal to the value
             passed. If end_offset is 0 (the default), the last partition ends before the current
             time. If end_offset is 1, the second-to-last partition ends before the current time,
             and so on.
     """
 
     def __new__(
         cls,
         start: Union[datetime, str],
         fmt: str,
+        end: Union[datetime, str, None] = None,
         schedule_type: Optional[ScheduleType] = None,
         timezone: Optional[str] = None,
         end_offset: int = 0,
         minute_offset: Optional[int] = None,
         hour_offset: Optional[int] = None,
         day_offset: Optional[int] = None,
         cron_schedule: Optional[str] = None,
@@ -115,14 +118,21 @@
         timezone = timezone or "UTC"
 
         if isinstance(start, datetime):
             start_dt = pendulum.instance(start, tz=timezone)
         else:
             start_dt = pendulum.instance(datetime.strptime(start, fmt), tz=timezone)
 
+        if not end:
+            end_dt = None
+        elif isinstance(end, datetime):
+            end_dt = pendulum.instance(end, tz=timezone)
+        else:
+            end_dt = pendulum.instance(datetime.strptime(end, fmt), tz=timezone)
+
         if cron_schedule is not None:
             check.invariant(
                 schedule_type is None and not minute_offset and not hour_offset and not day_offset,
                 (
                     "If cron_schedule argument is provided, then schedule_type, minute_offset, "
                     "hour_offset, and day_offset can't also be provided"
                 ),
@@ -141,15 +151,15 @@
         if not is_valid_cron_schedule(cron_schedule):
             raise DagsterInvalidDefinitionError(
                 f"Found invalid cron schedule '{cron_schedule}' for a"
                 " TimeWindowPartitionsDefinition."
             )
 
         return super(TimeWindowPartitionsDefinition, cls).__new__(
-            cls, start_dt, timezone, fmt, end_offset, cron_schedule
+            cls, start_dt, timezone, end_dt, fmt, end_offset, cron_schedule
         )
 
     def get_current_timestamp(self, current_time: Optional[datetime] = None) -> float:
         return (
             pendulum.instance(current_time, tz=self.timezone)
             if current_time
             else pendulum.now(self.timezone)
@@ -165,14 +175,16 @@
         # string format datetimes.
         current_timestamp = self.get_current_timestamp(current_time=current_time)
 
         partitions_past_current_time = 0
 
         num_partitions = 0
         for time_window in self._iterate_time_windows(self.start):
+            if self.end and time_window.end.timestamp() > self.end.timestamp():
+                break
             if (
                 time_window.end.timestamp() <= current_timestamp
                 or partitions_past_current_time < self.end_offset
             ):
                 num_partitions += 1
 
                 if time_window.end.timestamp() > current_timestamp:
@@ -197,14 +209,16 @@
         partitions_past_current_time = 0
         partition_keys = []
         reached_end = False
 
         for idx, time_window in enumerate(self._iterate_time_windows(self.start)):
             if time_window.end.timestamp() >= current_timestamp:
                 reached_end = True
+            if self.end and time_window.end.timestamp() > self.end.timestamp():
+                reached_end = True
             if (
                 time_window.end.timestamp() <= current_timestamp
                 or partitions_past_current_time < self.end_offset
             ):
                 if idx >= start_idx and idx < end_idx:
                     partition_keys.append(time_window.start.strftime(self.fmt))
                 if time_window.end.timestamp() > current_timestamp:
@@ -225,14 +239,16 @@
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> Sequence[str]:
         current_timestamp = self.get_current_timestamp(current_time=current_time)
 
         partitions_past_current_time = 0
         partition_keys: List[str] = []
         for time_window in self._iterate_time_windows(self.start):
+            if self.end and time_window.end.timestamp() > self.end.timestamp():
+                break
             if (
                 time_window.end.timestamp() <= current_timestamp
                 or partitions_past_current_time < self.end_offset
             ):
                 partition_keys.append(time_window.start.strftime(self.fmt))
 
                 if time_window.end.timestamp() > current_timestamp:
@@ -459,14 +475,17 @@
 
         current_time = (
             pendulum.instance(current_time, tz=self.timezone)
             if current_time
             else pendulum.now(self.timezone)
         )
 
+        if self.end and self.end < current_time:
+            current_time = self.end
+
         if self.end_offset == 0:
             return next(iter(self._reverse_iterate_time_windows(current_time)))
         else:
             # TODO: make this efficient
             last_partition_key = super().get_last_partition_key(current_time)
             return (
                 self.time_window_for_partition_key(last_partition_key)
@@ -747,14 +766,16 @@
     in the set will end before the current time, unless the end_offset argument is set to a
     positive number. If minute_offset and/or hour_offset are used, the start and end times of
     each partition will be hour_offset:minute_offset of each day.
 
     Args:
         start_date (Union[datetime.datetime, str]): The first date in the set of partitions. Can
             provide in either a datetime or string format.
+        end_date (Union[datetime.datetime, str, None]): The last date(excluding) in the set of partitions.
+            Default is None. Can provide in either a datetime or string format.
         minute_offset (int): Number of minutes past the hour to "split" the partition. Defaults
             to 0.
         hour_offset (int): Number of hours past 00:00 to "split" the partition. Defaults to 0.
         timezone (Optional[str]): The timezone in which each date should exist.
             Supported strings for timezones are the ones provided by the
             `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
         fmt (Optional[str]): The date format to use. Defaults to `%Y-%m-%d`.
@@ -771,26 +792,28 @@
         DailyPartitionsDefinition(start_date="2022-03-12", minute_offset=15, hour_offset=16)
         # creates partitions (2022-03-12-16:15, 2022-03-13-16:15), (2022-03-13-16:15, 2022-03-14-16:15), ...
     """
 
     def __new__(
         cls,
         start_date: Union[datetime, str],
+        end_date: Union[datetime, str, None] = None,
         minute_offset: int = 0,
         hour_offset: int = 0,
         timezone: Optional[str] = None,
         fmt: Optional[str] = None,
         end_offset: int = 0,
     ):
         _fmt = fmt or DEFAULT_DATE_FORMAT
 
         return super(DailyPartitionsDefinition, cls).__new__(
             cls,
             schedule_type=ScheduleType.DAILY,
             start=start_date,
+            end=end_date,
             minute_offset=minute_offset,
             hour_offset=hour_offset,
             timezone=timezone,
             fmt=_fmt,
             end_offset=end_offset,
         )
 
@@ -906,14 +929,16 @@
     in the set will end before the current time, unless the end_offset argument is set to a
     positive number. If minute_offset is provided, the start and end times of each partition
     will be minute_offset past the hour.
 
     Args:
         start_date (Union[datetime.datetime, str]): The first date in the set of partitions. Can
             provide in either a datetime or string format.
+        end_date (Union[datetime.datetime, str, None]): The last date(excluding) in the set of partitions.
+            Default is None. Can provide in either a datetime or string format.
         minute_offset (int): Number of minutes past the hour to "split" the partition. Defaults
             to 0.
         fmt (Optional[str]): The date format to use. Defaults to `%Y-%m-%d`.
         timezone (Optional[str]): The timezone in which each date should exist.
             Supported strings for timezones are the ones provided by the
             `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
         end_offset (int): Extends the partition set by a number of partitions equal to the value
@@ -929,25 +954,27 @@
         HourlyPartitionsDefinition(start_date=datetime(2022, 03, 12), minute_offset=15)
         # creates partitions (2022-03-12-00:15, 2022-03-12-01:15), (2022-03-12-01:15, 2022-03-12-02:15), ...
     """
 
     def __new__(
         cls,
         start_date: Union[datetime, str],
+        end_date: Union[datetime, str, None] = None,
         minute_offset: int = 0,
         timezone: Optional[str] = None,
         fmt: Optional[str] = None,
         end_offset: int = 0,
     ):
         _fmt = fmt or DEFAULT_HOURLY_FORMAT_WITHOUT_TIMEZONE
 
         return super(HourlyPartitionsDefinition, cls).__new__(
             cls,
             schedule_type=ScheduleType.HOURLY,
             start=start_date,
+            end=end_date,
             minute_offset=minute_offset,
             timezone=timezone,
             fmt=_fmt,
             end_offset=end_offset,
         )
 
 
@@ -1034,14 +1061,16 @@
     end date of each partition will be day_offset. If minute_offset and/or hour_offset are used,
     the start and end times of each partition will be hour_offset:minute_offset of each day.
 
     Args:
         start_date (Union[datetime.datetime, str]): The first date in the set of partitions will be
             midnight the sonnest first of the month following start_date. Can provide in either a
             datetime or string format.
+        end_date (Union[datetime.datetime, str, None]): The last date(excluding) in the set of partitions.
+            Default is None. Can provide in either a datetime or string format.
         minute_offset (int): Number of minutes past the hour to "split" the partition. Defaults
             to 0.
         hour_offset (int): Number of hours past 00:00 to "split" the partition. Defaults to 0.
         day_offset (int): Day of the month to "split" the partition. Defaults to 1.
         timezone (Optional[str]): The timezone in which each date should exist.
             Supported strings for timezones are the ones provided by the
             `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
@@ -1059,27 +1088,29 @@
         MonthlyPartitionsDefinition(start_date="2022-03-12", minute_offset=15, hour_offset=3, day_offset=5)
         # creates partitions (2022-04-05-03:15, 2022-05-05-03:15), (2022-05-05-03:15, 2022-06-05-03:15), ...
     """
 
     def __new__(
         cls,
         start_date: Union[datetime, str],
+        end_date: Union[datetime, str, None] = None,
         minute_offset: int = 0,
         hour_offset: int = 0,
         day_offset: int = 1,
         timezone: Optional[str] = None,
         fmt: Optional[str] = None,
         end_offset: int = 0,
     ):
         _fmt = fmt or DEFAULT_DATE_FORMAT
 
         return super(MonthlyPartitionsDefinition, cls).__new__(
             cls,
             schedule_type=ScheduleType.MONTHLY,
             start=start_date,
+            end=end_date,
             minute_offset=minute_offset,
             hour_offset=hour_offset,
             day_offset=day_offset,
             timezone=timezone,
             fmt=_fmt,
             end_offset=end_offset,
         )
@@ -1178,14 +1209,16 @@
     minute_offset and/or hour_offset are used, the start and end times of each partition will be
     hour_offset:minute_offset of each day.
 
     Args:
         start_date (Union[datetime.datetime, str]): The first date in the set of partitions will
             Sunday at midnight following start_date. Can provide in either a datetime or string
             format.
+        end_date (Union[datetime.datetime, str, None]): The last date(excluding) in the set of partitions.
+            Default is None. Can provide in either a datetime or string format.
         minute_offset (int): Number of minutes past the hour to "split" the partition. Defaults
             to 0.
         hour_offset (int): Number of hours past 00:00 to "split" the partition. Defaults to 0.
         day_offset (int): Day of the week to "split" the partition. Defaults to 0 (Sunday).
         timezone (Optional[str]): The timezone in which each date should exist.
             Supported strings for timezones are the ones provided by the
             `IANA time zone database <https://www.iana.org/time-zones>` - e.g. "America/Los_Angeles".
@@ -1203,27 +1236,29 @@
         WeeklyPartitionsDefinition(start_date="2022-03-12", minute_offset=15, hour_offset=3, day_offset=6)
         # creates partitions (2022-03-12-03:15, 2022-03-19-03:15), (2022-03-19-03:15, 2022-03-26-03:15), ...
     """
 
     def __new__(
         cls,
         start_date: Union[datetime, str],
+        end_date: Union[datetime, str, None] = None,
         minute_offset: int = 0,
         hour_offset: int = 0,
         day_offset: int = 0,
         timezone: Optional[str] = None,
         fmt: Optional[str] = None,
         end_offset: int = 0,
     ):
         _fmt = fmt or DEFAULT_DATE_FORMAT
 
         return super(WeeklyPartitionsDefinition, cls).__new__(
             cls,
             schedule_type=ScheduleType.WEEKLY,
             start=start_date,
+            end=end_date,
             minute_offset=minute_offset,
             hour_offset=hour_offset,
             day_offset=day_offset,
             timezone=timezone,
             fmt=_fmt,
             end_offset=end_offset,
         )
```

### Comparing `dagster-1.3.4/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.5/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/utils.py` & `dagster-1.3.5/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.5/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/errors.py` & `dagster-1.3.5/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/event_api.py` & `dagster-1.3.5/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/events/__init__.py` & `dagster-1.3.5/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/events/log.py` & `dagster-1.3.5/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/events/utils.py` & `dagster-1.3.5/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/api.py` & `dagster-1.3.5/dagster/_core/execution/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # | execute_run_iterator        | DagsterRun         | async | (1)         | no                      |
 # | execute_run                 | DagsterRun         | sync  | (1)         | no                      |
 # | execute_plan_iterator       | ExecutionPlan      | async | (2)         | no                      |
 # | execute_plan                | ExecutionPlan      | sync  | (2)         | no                      |
 #
 # Notes on reexecution support:
 # (1) The appropriate bits must be set on the DagsterRun passed to this function. Specifically,
-#     parent_run_id and root_run_id must be set and consistent, and if a solids_to_execute or
+#     parent_run_id and root_run_id must be set and consistent, and if a resolved_op_selection or
 #     step_keys_to_execute are set they must be consistent with the parent and root runs.
 # (2) As for (1), but the ExecutionPlan passed must also agree in all relevant bits.
 
 
 def execute_run_iterator(
     job: IJob,
     dagster_run: DagsterRun,
@@ -132,21 +132,21 @@
                 "Run of {} ({}) in state {}, expected STARTED or STARTING because it's "
                 "resuming from a run worker failure".format(
                     dagster_run.job_name, dagster_run.run_id, dagster_run.status
                 )
             ),
         )
 
-    if dagster_run.solids_to_execute or dagster_run.asset_selection:
+    if dagster_run.resolved_op_selection or dagster_run.asset_selection:
         # when `execute_run_iterator` is directly called, the sub pipeline hasn't been created
         # note that when we receive the solids to execute via DagsterRun, it won't support
         # solid selection query syntax
         job = job.get_subset(
-            op_selection=list(dagster_run.solids_to_execute)
-            if dagster_run.solids_to_execute
+            op_selection=list(dagster_run.resolved_op_selection)
+            if dagster_run.resolved_op_selection
             else None,
             asset_selection=dagster_run.asset_selection,
         )
 
     execution_plan = _get_execution_plan_from_run(job, dagster_run, instance)
     if isinstance(job, ReconstructableJob):
         job = job.with_repository_load_data(execution_plan.repository_load_data)
@@ -214,21 +214,21 @@
     check.invariant(
         dagster_run.status == DagsterRunStatus.NOT_STARTED
         or dagster_run.status == DagsterRunStatus.STARTING,
         desc="Run {} ({}) in state {}, expected NOT_STARTED or STARTING".format(
             dagster_run.job_name, dagster_run.run_id, dagster_run.status
         ),
     )
-    if dagster_run.solids_to_execute or dagster_run.asset_selection:
+    if dagster_run.resolved_op_selection or dagster_run.asset_selection:
         # when `execute_run` is directly called, the sub job hasn't been created
         # note that when we receive the solids to execute via DagsterRun, it won't support
         # solid selection query syntax
         job = job.get_subset(
-            op_selection=list(dagster_run.solids_to_execute)
-            if dagster_run.solids_to_execute
+            op_selection=list(dagster_run.resolved_op_selection)
+            if dagster_run.resolved_op_selection
             else None,
             asset_selection=dagster_run.asset_selection,
         )
 
     execution_plan = _get_execution_plan_from_run(job, dagster_run, instance)
     if isinstance(job, ReconstructableJob):
         job = job.with_repository_load_data(execution_plan.repository_load_data)
@@ -479,30 +479,30 @@
 
     job_arg, repository_load_data = _job_with_repository_load_data(job_arg)
 
     (
         job_arg,
         run_config,
         tags,
-        solids_to_execute,
+        resolved_op_selection,
         op_selection,
     ) = _check_execute_job_args(
         job_arg=job_arg,
         run_config=run_config,
         tags=tags,
         op_selection=op_selection,
     )
 
     log_repo_stats(instance=instance, job=job_arg, source="execute_pipeline")
 
     dagster_run = instance.create_run_for_job(
         job_def=job_arg.get_definition(),
         run_config=run_config,
-        solid_selection=op_selection,
-        solids_to_execute=solids_to_execute,
+        op_selection=op_selection,
+        resolved_op_selection=resolved_op_selection,
         tags=tags,
         job_code_origin=(
             job_arg.get_python_origin() if isinstance(job_arg, ReconstructableJob) else None
         ),
         repository_load_data=repository_load_data,
         asset_selection=frozenset(asset_selection) if asset_selection else None,
     )
@@ -563,17 +563,17 @@
             )
 
         dagster_run = execute_instance.create_run_for_job(
             job_def=job_arg.get_definition(),
             execution_plan=execution_plan,
             run_config=run_config,
             tags=tags,
-            solid_selection=parent_dagster_run.solid_selection,
+            op_selection=parent_dagster_run.op_selection,
             asset_selection=parent_dagster_run.asset_selection,
-            solids_to_execute=parent_dagster_run.solids_to_execute,
+            resolved_op_selection=parent_dagster_run.resolved_op_selection,
             root_run_id=parent_dagster_run.root_run_id or parent_dagster_run.run_id,
             parent_run_id=parent_dagster_run.run_id,
             job_code_origin=(
                 job_arg.get_python_origin() if isinstance(job_arg, ReconstructableJob) else None
             ),
             repository_load_data=repository_load_data,
         )
@@ -647,23 +647,14 @@
             dagster_run=dagster_run,
             instance=instance,
             retry_mode=retry_mode,
         )
     )
 
 
-def _check_job(job_arg: Union[JobDefinition, IJob]) -> IJob:
-    # backcompat
-    if isinstance(job_arg, JobDefinition):
-        job_arg = InMemoryJob(job_arg)
-
-    check.inst_param(job_arg, "job_arg", IJob)
-    return job_arg
-
-
 def _get_execution_plan_from_run(
     job: IJob,
     dagster_run: DagsterRun,
     instance: DagsterInstance,
 ) -> ExecutionPlan:
     execution_plan_snapshot = (
         instance.get_execution_plan_snapshot(dagster_run.execution_plan_snapshot_id)
@@ -671,15 +662,15 @@
         else None
     )
 
     # Rebuild from snapshot if able and selection has not changed
     if (
         execution_plan_snapshot is not None
         and execution_plan_snapshot.can_reconstruct_plan
-        and job.solids_to_execute == dagster_run.solids_to_execute
+        and job.resolved_op_selection == dagster_run.resolved_op_selection
         and job.asset_selection == dagster_run.asset_selection
     ):
         return ExecutionPlan.rebuild_from_snapshot(
             dagster_run.job_name,
             execution_plan_snapshot,
         )
 
@@ -702,22 +693,22 @@
     run_config: Optional[Mapping[str, object]] = None,
     step_keys_to_execute: Optional[Sequence[str]] = None,
     known_state: Optional[KnownExecutionState] = None,
     instance_ref: Optional[InstanceRef] = None,
     tags: Optional[Mapping[str, str]] = None,
     repository_load_data: Optional[RepositoryLoadData] = None,
 ) -> ExecutionPlan:
-    job = _check_job(job)
-
-    # If you have repository_load_data, make sure to use it when building plan
-    if isinstance(job, ReconstructableJob) and repository_load_data is not None:
-        job = job.with_repository_load_data(repository_load_data)
+    if isinstance(job, IJob):
+        # If you have repository_load_data, make sure to use it when building plan
+        if isinstance(job, ReconstructableJob) and repository_load_data is not None:
+            job = job.with_repository_load_data(repository_load_data)
+        job_def = job.get_definition()
+    else:
+        job_def = job
 
-    job_def = job.get_definition()
-    check.inst_param(job_def, "job_def", JobDefinition)
     run_config = check.opt_mapping_param(run_config, "run_config", key_type=str)
     check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
     check.opt_inst_param(instance_ref, "instance_ref", InstanceRef)
     tags = check.opt_mapping_param(tags, "tags", key_type=str, value_type=str)
     known_state = check.opt_inst_param(
         known_state,
         "known_state",
@@ -727,15 +718,15 @@
     repository_load_data = check.opt_inst_param(
         repository_load_data, "repository_load_data", RepositoryLoadData
     )
 
     resolved_run_config = ResolvedRunConfig.build(job_def, run_config)
 
     return ExecutionPlan.build(
-        job,
+        job_def,
         resolved_run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
         instance_ref=instance_ref,
         tags=tags,
         repository_load_data=repository_load_data,
     )
@@ -900,47 +891,46 @@
 ) -> Tuple[
     IJob,
     Optional[Mapping],
     Mapping[str, str],
     Optional[AbstractSet[str]],
     Optional[Sequence[str]],
 ]:
-    job_arg = _check_job(job_arg)
-    job_def = job_arg.get_definition()
-    check.inst_param(job_def, "job_def", JobDefinition)
+    ijob = InMemoryJob(job_arg) if isinstance(job_arg, JobDefinition) else job_arg
+    job_def = job_arg if isinstance(job_arg, JobDefinition) else job_arg.get_definition()
 
     run_config = check.opt_mapping_param(run_config, "run_config")
 
     tags = check.opt_mapping_param(tags, "tags", key_type=str)
-    check.opt_sequence_param(op_selection, "solid_selection", of_type=str)
+    check.opt_sequence_param(op_selection, "op_selection", of_type=str)
 
     tags = merge_dicts(job_def.tags, tags)
 
-    # generate job subset from the given solid_selection
+    # generate job subset from the given op_selection
     if op_selection:
-        job_arg = job_arg.get_subset(op_selection=op_selection)
+        ijob = ijob.get_subset(op_selection=op_selection)
 
     return (
-        job_arg,
+        ijob,
         run_config,
         tags,
-        job_arg.solids_to_execute,
+        ijob.resolved_op_selection,
         op_selection,
     )
 
 
 def _resolve_reexecute_step_selection(
     instance: DagsterInstance,
     job: IJob,
     run_config: Optional[Mapping],
     parent_dagster_run: DagsterRun,
     step_selection: Sequence[str],
 ) -> ExecutionPlan:
-    if parent_dagster_run.solid_selection:
-        job = job.get_subset(op_selection=parent_dagster_run.solid_selection)
+    if parent_dagster_run.op_selection:
+        job = job.get_subset(op_selection=parent_dagster_run.op_selection)
 
     state = KnownExecutionState.build_for_reexecution(instance, parent_dagster_run)
 
     parent_plan = create_execution_plan(
         job,
         parent_dagster_run.run_config,
         known_state=state,
```

### Comparing `dagster-1.3.4/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.5/dagster/_core/execution/asset_backfill.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
         check.failed("Expected RunRequest to have an asset selection")
 
     pipeline_selector = JobSubsetSelector(
         location_name=location_name,
         repository_name=repo_handle.repository_name,
         job_name=job_name,
         asset_selection=run_request.asset_selection,
-        solid_selection=None,
+        op_selection=None,
     )
 
     selector_id = hash_collection(pipeline_selector)
 
     if selector_id not in pipeline_and_execution_plan_cache:
         code_location = workspace.get_code_location(repo_handle.code_location_origin.location_name)
 
@@ -514,16 +514,16 @@
 
     run = instance.create_run(
         job_snapshot=external_job.job_snapshot,
         execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
         parent_job_snapshot=external_job.parent_job_snapshot,
         job_name=external_job.name,
         run_id=None,
-        solids_to_execute=None,
-        solid_selection=None,
+        resolved_op_selection=None,
+        op_selection=None,
         run_config={},
         step_keys_to_execute=None,
         tags=run_request.tags,
         root_run_id=None,
         parent_run_id=None,
         status=DagsterRunStatus.NOT_STARTED,
         external_job_origin=external_job.get_external_origin(),
```

### Comparing `dagster-1.3.4/dagster/_core/execution/backfill.py` & `dagster-1.3.5/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/build_resources.py` & `dagster-1.3.5/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/compute_logs.py` & `dagster-1.3.5/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/compute.py` & `dagster-1.3.5/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/hook.py` & `dagster-1.3.5/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/init.py` & `dagster-1.3.5/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/input.py` & `dagster-1.3.5/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/invocation.py` & `dagster-1.3.5/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/logger.py` & `dagster-1.3.5/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/output.py` & `dagster-1.3.5/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context/system.py` & `dagster-1.3.5/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/context_creation_job.py` & `dagster-1.3.5/dagster/_core/execution/context_creation_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,15 @@
 
     return ContextCreationData(
         job=job,
         resolved_run_config=resolved_run_config,
         dagster_run=dagster_run,
         executor_def=executor_def,
         instance=instance,
-        resource_keys_to_init=get_required_resource_keys_to_init(
-            execution_plan, job_def, resolved_run_config
-        ),
+        resource_keys_to_init=get_required_resource_keys_to_init(execution_plan, job_def),
         execution_plan=execution_plan,
     )
 
 
 def create_plan_data(
     context_creation_data: "ContextCreationData", raise_on_error: bool, retry_mode: RetryMode
 ) -> PlanData:
```

### Comparing `dagster-1.3.4/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.5/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.5/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/execution_result.py` & `dagster-1.3.5/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/host_mode.py` & `dagster-1.3.5/dagster/_core/execution/host_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         or dagster_run.status == DagsterRunStatus.STARTING,
         desc="Pipeline run {} ({}) in state {}, expected NOT_STARTED or STARTING".format(
             dagster_run.job_name, dagster_run.run_id, dagster_run.status
         ),
     )
 
     recon_job = recon_job.get_subset(
-        op_selection=dagster_run.solids_to_execute,
+        op_selection=dagster_run.resolved_op_selection,
         asset_selection=dagster_run.asset_selection,
     )
 
     execution_plan_snapshot = instance.get_execution_plan_snapshot(
         check.not_none(dagster_run.execution_plan_snapshot_id)
     )
     execution_plan = ExecutionPlan.rebuild_from_snapshot(
```

### Comparing `dagster-1.3.4/dagster/_core/execution/job_backfill.py` & `dagster-1.3.5/dagster/_core/execution/job_backfill.py`

 * *Files 8% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     if backfill_job.asset_selection:
         # need to make another call to the user code location to properly subset
         # for an asset selection
         pipeline_selector = JobSubsetSelector(
             location_name=code_location.name,
             repository_name=repo_name,
             job_name=external_partition_set.job_name,
-            solid_selection=None,
+            op_selection=None,
             asset_selection=backfill_job.asset_selection,
         )
         external_job = code_location.get_external_job(pipeline_selector)
     else:
         external_job = external_repo.get_full_external_job(external_partition_set.job_name)
     for partition_data in result.partition_data:
         # Refresh the code location in case the workspace has reloaded mid-backfill
@@ -257,24 +257,24 @@
     tags = merge_dicts(
         external_pipeline.tags,
         partition_data.tags,
         DagsterRun.tags_for_backfill_id(backfill_job.backfill_id),
         backfill_job.tags,
     )
 
-    solids_to_execute = None
-    solid_selection = None
+    resolved_op_selection = None
+    op_selection = None
     if not backfill_job.from_failure and not backfill_job.reexecution_steps:
         step_keys_to_execute = None
         parent_run_id = None
         root_run_id = None
         known_state = None
-        if external_partition_set.solid_selection:
-            solids_to_execute = frozenset(external_partition_set.solid_selection)
-            solid_selection = external_partition_set.solid_selection
+        if external_partition_set.op_selection:
+            resolved_op_selection = frozenset(external_partition_set.op_selection)
+            op_selection = external_partition_set.op_selection
 
     elif backfill_job.from_failure:
         last_run = _fetch_last_run(instance, external_partition_set, partition_data.name)
         if not last_run or last_run.status != DagsterRunStatus.FAILURE:
             return None
         return instance.create_reexecuted_run(
             parent_run=last_run,
@@ -299,17 +299,17 @@
             known_state = KnownExecutionState.build_for_reexecution(
                 instance,
                 last_run,
             ).update_for_step_selection(step_keys_to_execute)
         else:
             known_state = None
 
-        if external_partition_set.solid_selection:
-            solids_to_execute = frozenset(external_partition_set.solid_selection)
-            solid_selection = external_partition_set.solid_selection
+        if external_partition_set.op_selection:
+            resolved_op_selection = frozenset(external_partition_set.op_selection)
+            op_selection = external_partition_set.op_selection
 
     external_execution_plan = code_location.get_external_execution_plan(
         external_pipeline,
         partition_data.run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
         instance=instance,
@@ -317,24 +317,24 @@
 
     return instance.create_run(
         job_snapshot=external_pipeline.job_snapshot,
         execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
         parent_job_snapshot=external_pipeline.parent_job_snapshot,
         job_name=external_pipeline.name,
         run_id=make_new_run_id(),
-        solids_to_execute=solids_to_execute,
+        resolved_op_selection=resolved_op_selection,
         run_config=partition_data.run_config,
         step_keys_to_execute=step_keys_to_execute,
         tags=tags,
         root_run_id=root_run_id,
         parent_run_id=parent_run_id,
         status=DagsterRunStatus.NOT_STARTED,
         external_job_origin=external_pipeline.get_external_origin(),
         job_code_origin=external_pipeline.get_python_origin(),
-        solid_selection=solid_selection,
+        op_selection=op_selection,
         asset_selection=frozenset(backfill_job.asset_selection)
         if backfill_job.asset_selection
         else None,
     )
 
 
 def _fetch_last_run(
```

### Comparing `dagster-1.3.4/dagster/_core/execution/job_execution_result.py` & `dagster-1.3.5/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/memoization.py` & `dagster-1.3.5/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/active.py` & `dagster-1.3.5/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/compute.py` & `dagster-1.3.5/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.5/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.5/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.5/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.5/dagster/_core/execution/plan/external_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,18 +182,18 @@
 def step_run_ref_to_step_context(
     step_run_ref: StepRunRef, instance: DagsterInstance
 ) -> StepExecutionContext:
     check.inst_param(instance, "instance", DagsterInstance)
 
     job = step_run_ref.recon_job
 
-    solids_to_execute = step_run_ref.dagster_run.solids_to_execute
-    if solids_to_execute or step_run_ref.dagster_run.asset_selection:
+    resolved_op_selection = step_run_ref.dagster_run.resolved_op_selection
+    if resolved_op_selection or step_run_ref.dagster_run.asset_selection:
         job = step_run_ref.recon_job.get_subset(
-            op_selection=solids_to_execute,
+            op_selection=resolved_op_selection,
             asset_selection=step_run_ref.dagster_run.asset_selection,
         )
 
     execution_plan = create_execution_plan(
         job,
         step_run_ref.run_config,
         step_keys_to_execute=[step_run_ref.step_key],
```

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/handle.py` & `dagster-1.3.5/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.5/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.5/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/objects.py` & `dagster-1.3.5/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.5/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/plan.py` & `dagster-1.3.5/dagster/_core/execution/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._core.definitions import (
     GraphDefinition,
-    IJob,
     InputDefinition,
     Node,
     NodeHandle,
     NodeOutput,
     OpDefinition,
 )
 from dagster._core.definitions.composition import MappedInputPlaceholder
 from dagster._core.definitions.dependency import DependencyStructure
 from dagster._core.definitions.executor_definition import ExecutorRequirement
 from dagster._core.definitions.job_definition import JobDefinition
-from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.definitions.repository_definition import RepositoryLoadData
 from dagster._core.errors import (
     DagsterExecutionStepNotFoundError,
     DagsterInvariantViolationError,
     DagsterUnmetExecutorRequirementsError,
 )
 from dagster._core.execution.plan.handle import (
@@ -96,87 +94,70 @@
 
 
 class _PlanBuilder:
     """This is the state that is built up during the execution plan build process."""
 
     def __init__(
         self,
-        job: IJob,
+        job_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
         step_keys_to_execute: Optional[Sequence[str]],
         known_state: KnownExecutionState,
         instance_ref: Optional[InstanceRef],
         tags: Mapping[str, str],
         repository_load_data: Optional[RepositoryLoadData],
     ):
-        if isinstance(job, ReconstructableJob) and repository_load_data is not None:
-            check.invariant(
-                job.repository.repository_load_data == repository_load_data,
-                (
-                    "When building an ExecutionPlan with explicit repository_load_data and a"
-                    " ReconstructableJob, the repository_load_data on the job must be"
-                    " identical to passed-in repository_load_data."
-                ),
-            )
-        self.job = check.inst_param(job, "job", IJob)
+        self.job_def = check.inst_param(job_def, "job", JobDefinition)
         self.resolved_run_config = check.inst_param(
             resolved_run_config, "resolved_run_config", ResolvedRunConfig
         )
-        check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", str)
-        self.step_keys_to_execute = step_keys_to_execute
-        self._steps: Dict[str, IExecutionStep] = {}
-        self.step_output_map: Dict[
-            NodeOutput, Union[StepOutputHandle, UnresolvedStepOutputHandle]
-        ] = {}
+        self.step_keys_to_execute = check.opt_nullable_sequence_param(
+            step_keys_to_execute, "step_keys_to_execute", str
+        )
         self.known_state = check.inst_param(known_state, "known_state", KnownExecutionState)
         self._instance_ref = instance_ref
-        self._seen_handles: Set[StepHandleUnion] = set()
         self._tags = check.mapping_param(tags, "tags", key_type=str, value_type=str)
         self.repository_load_data = check.opt_inst_param(
             repository_load_data, "repository_load_data", RepositoryLoadData
         )
 
-    @property
-    def job_name(self) -> str:
-        return self.job.get_definition().name
+        self._steps: Dict[str, IExecutionStep] = {}
+        self.step_output_map: Dict[
+            NodeOutput, Union[StepOutputHandle, UnresolvedStepOutputHandle]
+        ] = {}
+        self._seen_handles: Set[StepHandleUnion] = set()
 
     def add_step(self, step: IExecutionStep) -> None:
         # Keep track of the step keys we've seen so far to ensure we don't add duplicates
         if step.handle in self._seen_handles:
             keys = list(self._steps.keys())
-            check.failed(
-                "Duplicated key {key}. Full list seen so far: {key_list}.".format(
-                    key=step.key, key_list=keys
-                )
-            )
+            check.failed(f"Duplicated key {step.key}. Full list seen so far: {keys}.")
         self._seen_handles.add(step.handle)
         self._steps[step.node_handle.to_string()] = step
 
     def get_step_by_node_handle(self, handle: NodeHandle) -> IExecutionStep:
         check.inst_param(handle, "handle", NodeHandle)
         return self._steps[handle.to_string()]
 
     def build(self) -> "ExecutionPlan":
         """Builds the execution plan."""
         _check_persistent_storage_requirement(
-            self.job,
+            self.job_def,
             self.resolved_run_config,
         )
 
-        job_def = self.job.get_definition()
         root_inputs: List[
             Union[StepInput, UnresolvedMappedStepInput, UnresolvedCollectStepInput]
         ] = []
-        # Recursively build the execution plan starting at the root pipeline
-        for input_def in job_def.graph.input_defs:
+        # Recursively bjob_defd the execution plan starting at the root pipeline
+        for input_def in self.job_def.graph.input_defs:
             input_name = input_def.name
 
-            input_source = get_root_graph_input_source(
-                plan_builder=self,
-                job_def=job_def,
+            input_source = self.get_root_graph_input_source(
+                job_def=self.job_def,
                 input_name=input_name,
                 input_def=input_def,
             )
 
             # If an input with dagster_type "Nothing" doesn't have a value
             # we don't create a StepInput
             if input_source is None:
@@ -187,16 +168,16 @@
                     name=input_name,
                     dagster_type_key=input_def.dagster_type.key,
                     source=input_source,
                 )
             )
 
         self._build_from_sorted_nodes(
-            job_def.nodes_in_topological_order,
-            job_def.dependency_structure,
+            self.job_def.nodes_in_topological_order,
+            self.job_def.dependency_structure,
             parent_step_inputs=root_inputs,
         )
 
         step_dict = {step.handle: step for step in self._steps.values()}
         step_dict_by_key = {step.key: step for step in self._steps.values()}
         step_handles_to_execute = [step.handle for step in self._steps.values()]
 
@@ -216,62 +197,62 @@
             resolvable_map,
             step_handles_to_execute,
             self.known_state,
             _compute_artifacts_persisted(
                 step_dict,
                 step_dict_by_key,
                 step_handles_to_execute,
-                job_def,
+                self.job_def,
                 self.resolved_run_config,
                 executable_map,
             ),
             executor_name=executor_name,
             repository_load_data=self.repository_load_data,
         )
 
         if self.step_keys_to_execute is not None:
             plan = plan.build_subset_plan(
-                self.step_keys_to_execute, job_def, self.resolved_run_config
+                self.step_keys_to_execute, self.job_def, self.resolved_run_config
             )
 
         # Expects that if step_keys_to_execute was set, that the `plan` variable will have the
         # reflected step_keys_to_execute
-        if job_def.is_using_memoization(self._tags) and len(step_output_versions) == 0:
+        if self.job_def.is_using_memoization(self._tags) and len(step_output_versions) == 0:
             if self._instance_ref is None:
                 raise DagsterInvariantViolationError(
                     "Attempted to build memoized execution plan without providing a persistent "
                     "DagsterInstance to create_execution_plan."
                 )
             instance = DagsterInstance.from_ref(self._instance_ref)
             plan = plan.build_memoized_plan(
-                job_def, self.resolved_run_config, instance, self.step_keys_to_execute
+                self.job_def, self.resolved_run_config, instance, self.step_keys_to_execute
             )
 
         return plan
 
     def _build_from_sorted_nodes(
         self,
         nodes: Sequence[Node],
         dependency_structure: DependencyStructure,
         parent_handle: Optional[NodeHandle] = None,
         parent_step_inputs: Optional[Sequence[StepInputUnion]] = None,
     ) -> None:
-        asset_layer = self.job.get_definition().asset_layer
+        asset_layer = self.job_def.asset_layer
         step_output_map: Dict[NodeOutput, Union[StepOutputHandle, UnresolvedStepOutputHandle]] = {}
         for node in nodes:
             handle = NodeHandle(node.name, parent_handle)
 
             ### 1. INPUTS
             # Create and add execution plan steps for node inputs
             has_unresolved_input = False
             has_pending_input = False
             step_inputs: List[StepInputUnion] = []
             for input_name, input_def in node.definition.input_dict.items():
                 step_input_source = get_step_input_source(
-                    self.job.get_definition(),
+                    self.job_def,
                     node,
                     input_name,
                     input_def,
                     dependency_structure,
                     handle,
                     self.resolved_run_config.ops.get(str(handle)),
                     step_output_map,
@@ -327,35 +308,35 @@
 
                 if has_pending_input and has_unresolved_input:
                     check.failed("Can not have pending and unresolved step inputs")
 
                 elif has_unresolved_input:
                     new_step = UnresolvedMappedExecutionStep(
                         handle=UnresolvedStepHandle(node_handle=handle),
-                        job_name=self.job_name,
+                        job_name=self.job_def.name,
                         step_inputs=cast(
                             List[Union[StepInput, UnresolvedMappedStepInput]], step_inputs
                         ),
                         step_outputs=step_outputs,
                         tags=node.tags,
                     )
                 elif has_pending_input:
                     new_step = UnresolvedCollectExecutionStep(
                         handle=StepHandle(node_handle=handle),
-                        job_name=self.job_name,
+                        job_name=self.job_def.name,
                         step_inputs=cast(
                             List[Union[StepInput, UnresolvedCollectStepInput]], step_inputs
                         ),
                         step_outputs=step_outputs,
                         tags=node.tags,
                     )
                 else:
                     new_step = ExecutionStep(
                         handle=StepHandle(node_handle=handle),
-                        job_name=self.job_name,
+                        job_name=self.job_def.name,
                         step_inputs=cast(List[StepInput], step_inputs),
                         step_outputs=step_outputs,
                         tags=node.tags,
                     )
 
                 self.add_step(new_step)
 
@@ -401,43 +382,42 @@
                         step.resolved_by_output_name,
                     )
                 else:
                     check.failed(f"Unexpected step type {step}")
 
                 step_output_map[node_output] = step_output_handle
 
+    def get_root_graph_input_source(
+        self,
+        input_name: str,
+        input_def: InputDefinition,
+        job_def: JobDefinition,
+    ) -> Optional[Union[FromConfig, FromDirectInputValue]]:
+        input_values = job_def.input_values
+        if input_values and input_name in input_values:
+            return FromDirectInputValue(input_name=input_name)
 
-def get_root_graph_input_source(
-    plan_builder: _PlanBuilder,
-    input_name: str,
-    input_def: InputDefinition,
-    job_def: JobDefinition,
-) -> Optional[Union[FromConfig, FromDirectInputValue]]:
-    input_values = job_def.input_values
-    if input_values and input_name in input_values:
-        return FromDirectInputValue(input_name=input_name)
-
-    input_config = plan_builder.resolved_run_config.inputs
+        input_config = self.resolved_run_config.inputs
 
-    if input_config and input_name in input_config:
-        return FromConfig(input_name=input_name, node_handle=None)
+        if input_config and input_name in input_config:
+            return FromConfig(input_name=input_name, node_handle=None)
 
-    if input_def.dagster_type.is_nothing:
-        return None
+        if input_def.dagster_type.is_nothing:
+            return None
 
-    # Otherwise we throw an error.
-    raise DagsterInvariantViolationError(
-        (
-            "In top-level graph of {described_target}, input {input_name} "
-            "must get a value from the inputs section of its configuration."
-        ).format(
-            described_target=plan_builder.job.get_definition().describe_target(),
-            input_name=input_name,
+        # Otherwise we throw an error.
+        raise DagsterInvariantViolationError(
+            (
+                "In top-level graph of {described_target}, input {input_name} "
+                "must get a value from the inputs section of its configuration."
+            ).format(
+                described_target=self.job_def.describe_target(),
+                input_name=input_name,
+            )
         )
-    )
 
 
 def get_step_input_source(
     job_def: JobDefinition,
     node: Node,
     input_name: str,
     input_def: InputDefinition,
@@ -965,15 +945,15 @@
 
             return cast(ExecutionStep, only_step).handle
 
         return None
 
     @staticmethod
     def build(
-        job: IJob,
+        job_def: JobDefinition,
         resolved_run_config: ResolvedRunConfig,
         step_keys_to_execute: Optional[Sequence[str]] = None,
         known_state: Optional[KnownExecutionState] = None,
         instance_ref: Optional[InstanceRef] = None,
         tags: Optional[Mapping[str, str]] = None,
         repository_load_data: Optional[RepositoryLoadData] = None,
     ) -> "ExecutionPlan":
@@ -981,41 +961,23 @@
 
         To do this, we iterate through the job's nodes in topological order, and hand off the
         execution steps for each node to a companion _PlanBuilder object.
 
         Once we've processed the entire job, we invoke _PlanBuilder.build() to construct the
         ExecutionPlan object.
         """
-        check.inst_param(job, "job", IJob)
-        check.inst_param(resolved_run_config, "resolved_run_config", ResolvedRunConfig)
-        check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
-        known_state = check.opt_inst_param(
-            known_state,
-            "known_state",
-            KnownExecutionState,
-            # may be good to force call sites to specify instead of defaulting to unknown
-            default=KnownExecutionState(),
-        )
-        tags = check.opt_mapping_param(tags, "tags", key_type=str, value_type=str)
-        repository_load_data = check.opt_inst_param(
-            repository_load_data, "repository_load_data", RepositoryLoadData
-        )
-
-        plan_builder = _PlanBuilder(
-            job,
+        return _PlanBuilder(
+            job_def,
             resolved_run_config=resolved_run_config,
             step_keys_to_execute=step_keys_to_execute,
-            known_state=known_state,
+            known_state=known_state or KnownExecutionState(),
             instance_ref=instance_ref,
-            tags=tags,
+            tags=tags or {},
             repository_load_data=repository_load_data,
-        )
-
-        # Finally, we build and return the execution plan
-        return plan_builder.build()
+        ).build()
 
     @staticmethod
     def rebuild_step_input(
         step_input_snap: "ExecutionStepInputSnap",
     ) -> Union["StepInput", "UnresolvedMappedStepInput", "UnresolvedCollectStepInput"]:
         from dagster._core.snap.execution_plan_snapshot import ExecutionStepInputSnap
 
@@ -1195,18 +1157,17 @@
         if job_def.resource_defs[output_def.io_manager_key] == mem_io_manager:
             return False
 
     return True
 
 
 def _check_persistent_storage_requirement(
-    pipeline: IJob,
+    job_def: JobDefinition,
     resolved_run_config: ResolvedRunConfig,
 ) -> None:
-    job_def = pipeline.get_definition()
     executor_def = job_def.executor_def
     requirements_lst = executor_def.get_requirements(
         resolved_run_config.execution.execution_engine_config
     )
     if ExecutorRequirement.PERSISTENT_OUTPUTS not in requirements_lst:
         return
 
@@ -1275,15 +1236,15 @@
     return False
 
 
 def _compute_artifacts_persisted(
     step_dict: Dict[StepHandleUnion, IExecutionStep],
     step_dict_by_key: Dict[str, IExecutionStep],
     step_handles_to_execute: Sequence[StepHandleUnion],
-    pipeline_def: JobDefinition,
+    job_def: JobDefinition,
     resolved_run_config: ResolvedRunConfig,
     executable_map: Mapping[str, Union[StepHandle, ResolvedFromDynamicStepHandle]],
 ) -> bool:
     """Check if all the border steps of the current run have non-in-memory IO managers for reexecution.
 
     Border steps: all the steps that don't have upstream steps to execute, i.e. indegree is 0).
     """
@@ -1297,18 +1258,16 @@
     if len(steps_by_level) == 0:
         return False
 
     for step in steps_by_level[0]:
         # check if all its inputs' upstream step outputs have non-in-memory IO manager configured
         for step_input in step.step_inputs:
             for step_output_handle in step_input.get_step_output_handle_dependencies():
-                io_manager_key = _get_manager_key(
-                    step_dict_by_key, step_output_handle, pipeline_def
-                )
-                manager_def = pipeline_def.resource_defs.get(io_manager_key)
+                io_manager_key = _get_manager_key(step_dict_by_key, step_output_handle, job_def)
+                manager_def = job_def.resource_defs.get(io_manager_key)
                 if (
                     # no IO manager is configured
                     not manager_def
                     # IO manager is non persistent
                     or manager_def == mem_io_manager
                 ):
                     return False
```

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/state.py` & `dagster-1.3.5/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/step.py` & `dagster-1.3.5/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/plan/utils.py` & `dagster-1.3.5/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.5/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.5/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/resources_init.py` & `dagster-1.3.5/dagster/_core/execution/resources_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     UnresolvedMappedStepInput,
 )
 from dagster._core.execution.plan.plan import ExecutionPlan, StepHandleUnion
 from dagster._core.execution.plan.step import ExecutionStep, IExecutionStep
 from dagster._core.instance import DagsterInstance
 from dagster._core.log_manager import DagsterLogManager
 from dagster._core.storage.dagster_run import DagsterRun
-from dagster._core.system_config.objects import ResolvedRunConfig, ResourceConfig
+from dagster._core.system_config.objects import ResourceConfig
 from dagster._core.utils import toposort
 from dagster._utils import EventGenerationManager, ensure_gen
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.timing import format_duration, time_execution_scope
 
 from .context.init import InitResourceContext
 
@@ -355,34 +355,31 @@
             pass
         else:
             check.failed(f"Resource generator {resource_name} yielded more than one item.")
 
 
 def get_required_resource_keys_to_init(
     execution_plan: ExecutionPlan,
-    pipeline_def: JobDefinition,
-    resolved_run_config: ResolvedRunConfig,
+    job_def: JobDefinition,
 ) -> AbstractSet[str]:
     resource_keys: Set[str] = set()
 
     for step_handle, step in execution_plan.step_dict.items():
         if step_handle not in execution_plan.step_handles_to_execute:
             continue
 
-        hook_defs = pipeline_def.get_all_hooks_for_handle(step.node_handle)
+        hook_defs = job_def.get_all_hooks_for_handle(step.node_handle)
         for hook_def in hook_defs:
             resource_keys = resource_keys.union(hook_def.required_resource_keys)
 
         resource_keys = resource_keys.union(
-            get_required_resource_keys_for_step(pipeline_def, step, execution_plan)
+            get_required_resource_keys_for_step(job_def, step, execution_plan)
         )
 
-    return frozenset(
-        get_transitive_required_resource_keys(resource_keys, pipeline_def.resource_defs)
-    )
+    return frozenset(get_transitive_required_resource_keys(resource_keys, job_def.resource_defs))
 
 
 def get_transitive_required_resource_keys(
     required_resource_keys: AbstractSet[str], resource_defs: Mapping[str, ResourceDefinition]
 ) -> AbstractSet[str]:
     resource_dependencies = resolve_resource_dependencies(resource_defs)
     ensure_resource_deps_satisfiable(resource_dependencies)
```

### Comparing `dagster-1.3.4/dagster/_core/execution/retries.py` & `dagster-1.3.5/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.5/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/stats.py` & `dagster-1.3.5/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/tags.py` & `dagster-1.3.5/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.5/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.5/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/execution/with_resources.py` & `dagster-1.3.5/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/base.py` & `dagster-1.3.5/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.5/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/in_process.py` & `dagster-1.3.5/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/init.py` & `dagster-1.3.5/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/multiprocess.py` & `dagster-1.3.5/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.5/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/__init__.py` & `dagster-1.3.5/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/code_location.py` & `dagster-1.3.5/dagster/_core/host_representation/code_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     def get_external_job(self, selector: JobSubsetSelector) -> ExternalJob:
         """Return the ExternalPipeline for a specific pipeline. Subclasses only
         need to implement get_subset_external_pipeline_result to handle the case where
         an op selection is specified, which requires access to the underlying JobDefinition
         to generate the subsetted pipeline snapshot.
         """
-        if not selector.solid_selection and not selector.asset_selection:
+        if not selector.op_selection and not selector.asset_selection:
             return self.get_repository(selector.repository_name).get_full_external_job(
                 selector.job_name
             )
 
         repo_handle = self.get_repository(selector.repository_name).handle
 
         subset_result = self.get_subset_external_job_result(selector)
@@ -363,15 +363,15 @@
         )
 
         from dagster._grpc.impl import get_external_pipeline_subset_result
 
         return get_external_pipeline_subset_result(
             self._get_repo_def(selector.repository_name),
             selector.job_name,
-            selector.solid_selection,
+            selector.op_selection,
             selector.asset_selection,
         )
 
     def get_external_execution_plan(
         self,
         external_job: ExternalJob,
         run_config: Mapping[str, object],
@@ -387,15 +387,15 @@
         check.opt_inst_param(known_state, "known_state", KnownExecutionState)
         check.opt_inst_param(instance, "instance", DagsterInstance)
 
         execution_plan = create_execution_plan(
             job=self.get_reconstructable_job(
                 external_job.repository_handle.repository_name, external_job.name
             ).get_subset(
-                op_selection=external_job.solids_to_execute,
+                op_selection=external_job.resolved_op_selection,
                 asset_selection=external_job.asset_selection,
             ),
             run_config=run_config,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
         )
@@ -734,15 +734,15 @@
 
         execution_plan_snapshot_or_error = sync_get_external_execution_plan_grpc(
             api_client=self.client,
             job_origin=external_job.get_external_origin(),
             run_config=run_config,
             job_snapshot_id=external_job.identifying_job_snapshot_id,
             asset_selection=asset_selection,
-            solid_selection=external_job.solid_selection,
+            op_selection=external_job.op_selection,
             step_keys_to_execute=step_keys_to_execute,
             known_state=known_state,
             instance=instance,
         )
 
         return ExternalExecutionPlan(execution_plan_snapshot=execution_plan_snapshot_or_error)
 
@@ -757,15 +757,15 @@
         )
 
         external_repository = self.get_repository(selector.repository_name)
         job_handle = JobHandle(selector.job_name, external_repository.handle)
         return sync_get_external_job_subset_grpc(
             self.client,
             job_handle.get_external_origin(),
-            selector.solid_selection,
+            selector.op_selection,
             selector.asset_selection,
         )
 
     def get_external_partition_config(
         self,
         repository_handle: RepositoryHandle,
         partition_set_name: str,
```

### Comparing `dagster-1.3.4/dagster/_core/host_representation/external.py` & `dagster-1.3.5/dagster/_core/host_representation/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,25 +360,25 @@
             return self._data
 
     @property
     def repository_handle(self) -> RepositoryHandle:
         return self._repository_handle
 
     @property
-    def solid_selection(self) -> Optional[Sequence[str]]:
+    def op_selection(self) -> Optional[Sequence[str]]:
         return (
-            self._job_index.job_snapshot.lineage_snapshot.node_selection
+            self._job_index.job_snapshot.lineage_snapshot.op_selection
             if self._job_index.job_snapshot.lineage_snapshot
             else None
         )
 
     @property
-    def solids_to_execute(self) -> Optional[AbstractSet[str]]:
+    def resolved_op_selection(self) -> Optional[AbstractSet[str]]:
         return (
-            self._job_index.job_snapshot.lineage_snapshot.nodes_to_execute
+            self._job_index.job_snapshot.lineage_snapshot.resolved_op_selection
             if self._job_index.job_snapshot.lineage_snapshot
             else None
         )
 
     @property
     def asset_selection(self) -> Optional[AbstractSet[AssetKey]]:
         return (
@@ -604,16 +604,16 @@
         return self._external_schedule_data.cron_schedule
 
     @property
     def execution_timezone(self) -> Optional[str]:
         return self._external_schedule_data.execution_timezone
 
     @property
-    def solid_selection(self) -> Optional[Sequence[str]]:
-        return self._external_schedule_data.solid_selection
+    def op_selection(self) -> Optional[Sequence[str]]:
+        return self._external_schedule_data.op_selection
 
     @property
     def job_name(self) -> str:
         return self._external_schedule_data.job_name
 
     @property
     def mode(self) -> Optional[str]:
@@ -735,17 +735,17 @@
 
     @property
     def mode(self) -> Optional[str]:
         target = self._get_single_target()
         return target.mode if target else None
 
     @property
-    def solid_selection(self) -> Optional[Sequence[str]]:
+    def op_selection(self) -> Optional[Sequence[str]]:
         target = self._get_single_target()
-        return target.solid_selection if target else None
+        return target.op_selection if target else None
 
     def _get_single_target(self) -> Optional[ExternalTargetData]:
         if self._external_sensor_data.target_dict:
             return list(self._external_sensor_data.target_dict.values())[0]
         else:
             return None
 
@@ -860,16 +860,16 @@
         )
 
     @property
     def name(self) -> str:
         return self._external_partition_set_data.name
 
     @property
-    def solid_selection(self) -> Optional[Sequence[str]]:
-        return self._external_partition_set_data.solid_selection
+    def op_selection(self) -> Optional[Sequence[str]]:
+        return self._external_partition_set_data.op_selection
 
     @property
     def mode(self) -> Optional[str]:
         return self._external_partition_set_data.mode
 
     @property
     def job_name(self) -> str:
```

### Comparing `dagster-1.3.4/dagster/_core/host_representation/external_data.py` & `dagster-1.3.5/dagster/_core/host_representation/external_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains data objects meant to be serialized between
 host processes and user processes. They should contain no
 business logic or clever indexing. Use the classes in external.py
 for that.
 """
+import inspect
 import json
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from enum import Enum
 from typing import (
     Any,
     Dict,
@@ -85,14 +86,15 @@
     SensorType,
 )
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.definitions.utils import DEFAULT_GROUP_NAME
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.snap import JobSnapshot
 from dagster._core.snap.mode import ResourceDefSnap, build_resource_def_snap
+from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 
 DEFAULT_MODE_NAME = "default"
 DEFAULT_PRESET_NAME = "default"
 
 
@@ -346,73 +348,74 @@
             active_presets=check.sequence_param(
                 active_presets, "active_presets", of_type=ExternalPresetData
             ),
             parent_snapshot_id=check.opt_str_param(parent_snapshot_id, "parent_snapshot_id"),
         )
 
 
-@whitelist_for_serdes
+@whitelist_for_serdes(storage_field_names={"op_selection": "solid_selection"})
 class ExternalPresetData(
     NamedTuple(
         "_ExternalPresetData",
         [
             ("name", str),
             ("run_config", Mapping[str, object]),
-            ("solid_selection", Optional[Sequence[str]]),
+            ("op_selection", Optional[Sequence[str]]),
             ("mode", str),
             ("tags", Mapping[str, str]),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         run_config: Optional[Mapping[str, object]],
-        solid_selection: Optional[Sequence[str]],
+        op_selection: Optional[Sequence[str]],
         mode: str,
         tags: Mapping[str, str],
     ):
         return super(ExternalPresetData, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             run_config=check.opt_mapping_param(run_config, "run_config", key_type=str),
-            solid_selection=check.opt_nullable_sequence_param(
-                solid_selection, "solid_selection", of_type=str
+            op_selection=check.opt_nullable_sequence_param(
+                op_selection, "op_selection", of_type=str
             ),
             mode=check.str_param(mode, "mode"),
             tags=check.opt_mapping_param(tags, "tags", key_type=str, value_type=str),
         )
 
 
 @whitelist_for_serdes(
-    storage_field_names={"job_name": "pipeline_name"}, skip_when_empty_fields={"default_status"}
+    storage_field_names={"job_name": "pipeline_name", "op_selection": "solid_selection"},
+    skip_when_empty_fields={"default_status"},
 )
 class ExternalScheduleData(
     NamedTuple(
         "_ExternalScheduleData",
         [
             ("name", str),
             ("cron_schedule", Union[str, Sequence[str]]),
             ("job_name", str),
-            ("solid_selection", Optional[Sequence[str]]),
+            ("op_selection", Optional[Sequence[str]]),
             ("mode", Optional[str]),
             ("environment_vars", Optional[Mapping[str, str]]),
             ("partition_set_name", Optional[str]),
             ("execution_timezone", Optional[str]),
             ("description", Optional[str]),
             ("default_status", Optional[DefaultScheduleStatus]),
         ],
     )
 ):
     def __new__(
         cls,
         name,
         cron_schedule,
         job_name,
-        solid_selection,
+        op_selection,
         mode,
         environment_vars,
         partition_set_name,
         execution_timezone,
         description=None,
         default_status=None,
     ):
@@ -421,15 +424,15 @@
             cron_schedule = check.sequence_param(cron_schedule, "cron_schedule", of_type=str)
 
         return super(ExternalScheduleData, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             cron_schedule=cron_schedule,
             job_name=check.str_param(job_name, "job_name"),
-            solid_selection=check.opt_nullable_list_param(solid_selection, "solid_selection", str),
+            op_selection=check.opt_nullable_list_param(op_selection, "op_selection", str),
             mode=check.opt_str_param(mode, "mode"),
             environment_vars=check.opt_dict_param(environment_vars, "environment_vars"),
             partition_set_name=check.opt_str_param(partition_set_name, "partition_set_name"),
             execution_timezone=check.opt_str_param(execution_timezone, "execution_timezone"),
             description=check.opt_str_param(description, "description"),
             # Leave default_status as None if it's STOPPED to maintain stable back-compat IDs
             default_status=DefaultScheduleStatus.RUNNING
@@ -445,29 +448,29 @@
     def __new__(cls, error: Optional[SerializableErrorInfo]):
         return super(ExternalScheduleExecutionErrorData, cls).__new__(
             cls,
             error=check.opt_inst_param(error, "error", SerializableErrorInfo),
         )
 
 
-@whitelist_for_serdes(storage_field_names={"job_name": "pipeline_name"})
+@whitelist_for_serdes(
+    storage_field_names={"job_name": "pipeline_name", "op_selection": "solid_selection"}
+)
 class ExternalTargetData(
     NamedTuple(
         "_ExternalTargetData",
-        [("job_name", str), ("mode", str), ("solid_selection", Optional[Sequence[str]])],
+        [("job_name", str), ("mode", str), ("op_selection", Optional[Sequence[str]])],
     )
 ):
-    def __new__(cls, job_name: str, mode: str, solid_selection: Optional[Sequence[str]]):
+    def __new__(cls, job_name: str, mode: str, op_selection: Optional[Sequence[str]]):
         return super(ExternalTargetData, cls).__new__(
             cls,
             job_name=check.str_param(job_name, "job_name"),
             mode=mode,
-            solid_selection=check.opt_nullable_sequence_param(
-                solid_selection, "solid_selection", str
-            ),
+            op_selection=check.opt_nullable_sequence_param(op_selection, "op_selection", str),
         )
 
 
 @whitelist_for_serdes
 class ExternalSensorMetadata(
     NamedTuple("_ExternalSensorMetadata", [("asset_keys", Optional[Sequence[AssetKey]])])
 ):
@@ -479,39 +482,39 @@
             asset_keys=check.opt_nullable_sequence_param(
                 asset_keys, "asset_keys", of_type=AssetKey
             ),
         )
 
 
 @whitelist_for_serdes(
-    storage_field_names={"job_name": "pipeline_name"},
+    storage_field_names={"job_name": "pipeline_name", "op_selection": "solid_selection"},
     skip_when_empty_fields={"default_status", "sensor_type"},
 )
 class ExternalSensorData(
     NamedTuple(
         "_ExternalSensorData",
         [
             ("name", str),
             ("job_name", Optional[str]),
-            ("solid_selection", Optional[Sequence[str]]),
+            ("op_selection", Optional[Sequence[str]]),
             ("mode", Optional[str]),
             ("min_interval", Optional[int]),
             ("description", Optional[str]),
             ("target_dict", Mapping[str, ExternalTargetData]),
             ("metadata", Optional[ExternalSensorMetadata]),
             ("default_status", Optional[DefaultSensorStatus]),
             ("sensor_type", Optional[SensorType]),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         job_name: Optional[str] = None,
-        solid_selection: Optional[Sequence[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
         mode: Optional[str] = None,
         min_interval: Optional[int] = None,
         description: Optional[str] = None,
         target_dict: Optional[Mapping[str, ExternalTargetData]] = None,
         metadata: Optional[ExternalSensorMetadata] = None,
         default_status: Optional[DefaultSensorStatus] = None,
         sensor_type: Optional[SensorType] = None,
@@ -519,26 +522,26 @@
         if job_name and not target_dict:
             # handle the legacy case where the ExternalSensorData was constructed from an earlier
             # version of dagster
             target_dict = {
                 job_name: ExternalTargetData(
                     job_name=check.str_param(job_name, "job_name"),
                     mode=check.opt_str_param(mode, "mode", DEFAULT_MODE_NAME),
-                    solid_selection=check.opt_nullable_sequence_param(
-                        solid_selection, "solid_selection", str
+                    op_selection=check.opt_nullable_sequence_param(
+                        op_selection, "op_selection", str
                     ),
                 )
             }
 
         return super(ExternalSensorData, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             job_name=check.opt_str_param(job_name, "job_name"),  # keep legacy field populated
-            solid_selection=check.opt_nullable_sequence_param(
-                solid_selection, "solid_selection", str
+            op_selection=check.opt_nullable_sequence_param(
+                op_selection, "op_selection", str
             ),  # keep legacy field populated
             mode=check.opt_str_param(mode, "mode"),  # keep legacy field populated
             min_interval=check.opt_int_param(min_interval, "min_interval"),
             description=check.opt_str_param(description, "description"),
             target_dict=check.opt_mapping_param(
                 target_dict, "target_dict", str, ExternalTargetData
             ),
@@ -614,14 +617,15 @@
     NamedTuple(
         "_ExternalTimeWindowPartitionsDefinitionData",
         [
             ("start", float),
             ("timezone", Optional[str]),
             ("fmt", str),
             ("end_offset", int),
+            ("end", Optional[float]),
             ("cron_schedule", Optional[str]),
             # superseded by cron_schedule, but kept around for backcompat
             ("schedule_type", Optional[ScheduleType]),
             # superseded by cron_schedule, but kept around for backcompat
             ("minute_offset", Optional[int]),
             # superseded by cron_schedule, but kept around for backcompat
             ("hour_offset", Optional[int]),
@@ -632,50 +636,54 @@
 ):
     def __new__(
         cls,
         start: float,
         timezone: Optional[str],
         fmt: str,
         end_offset: int,
+        end: Optional[float] = None,
         cron_schedule: Optional[str] = None,
         schedule_type: Optional[ScheduleType] = None,
         minute_offset: Optional[int] = None,
         hour_offset: Optional[int] = None,
         day_offset: Optional[int] = None,
     ):
         return super(ExternalTimeWindowPartitionsDefinitionData, cls).__new__(
             cls,
             schedule_type=check.opt_inst_param(schedule_type, "schedule_type", ScheduleType),
             start=check.float_param(start, "start"),
             timezone=check.opt_str_param(timezone, "timezone"),
             fmt=check.str_param(fmt, "fmt"),
             end_offset=check.int_param(end_offset, "end_offset"),
+            end=check.opt_float_param(end, "end"),
             minute_offset=check.opt_int_param(minute_offset, "minute_offset"),
             hour_offset=check.opt_int_param(hour_offset, "hour_offset"),
             day_offset=check.opt_int_param(day_offset, "day_offset"),
             cron_schedule=check.opt_str_param(cron_schedule, "cron_schedule"),
         )
 
     def get_partitions_definition(self):
         if self.cron_schedule is not None:
             return TimeWindowPartitionsDefinition(
                 cron_schedule=self.cron_schedule,
                 start=pendulum.from_timestamp(self.start, tz=self.timezone),
                 timezone=self.timezone,
                 fmt=self.fmt,
                 end_offset=self.end_offset,
+                end=pendulum.from_timestamp(self.end, tz=self.timezone) if self.end else None,
             )
         else:
             # backcompat case
             return TimeWindowPartitionsDefinition(
                 schedule_type=self.schedule_type,
                 start=pendulum.from_timestamp(self.start, tz=self.timezone),
                 timezone=self.timezone,
                 fmt=self.fmt,
                 end_offset=self.end_offset,
+                end=pendulum.from_timestamp(self.end, tz=self.timezone) if self.end else None,
                 minute_offset=self.minute_offset,
                 hour_offset=self.hour_offset,
                 day_offset=self.day_offset,
             )
 
 
 @whitelist_for_serdes
@@ -745,42 +753,42 @@
     ExternalPartitionsDefinitionData,
     NamedTuple("_ExternalDynamicPartitionsDefinitionData", [("name", str)]),
 ):
     def get_partitions_definition(self):
         return DynamicPartitionsDefinition(name=self.name)
 
 
-@whitelist_for_serdes(storage_field_names={"job_name": "pipeline_name"})
+@whitelist_for_serdes(
+    storage_field_names={"job_name": "pipeline_name", "op_selection": "solid_selection"}
+)
 class ExternalPartitionSetData(
     NamedTuple(
         "_ExternalPartitionSetData",
         [
             ("name", str),
             ("job_name", str),
-            ("solid_selection", Optional[Sequence[str]]),
+            ("op_selection", Optional[Sequence[str]]),
             ("mode", Optional[str]),
             ("external_partitions_data", Optional[ExternalPartitionsDefinitionData]),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         job_name: str,
-        solid_selection: Optional[Sequence[str]],
+        op_selection: Optional[Sequence[str]],
         mode: Optional[str],
         external_partitions_data: Optional[ExternalPartitionsDefinitionData] = None,
     ):
         return super(ExternalPartitionSetData, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             job_name=check.str_param(job_name, "job_name"),
-            solid_selection=check.opt_nullable_sequence_param(
-                solid_selection, "solid_selection", str
-            ),
+            op_selection=check.opt_nullable_sequence_param(op_selection, "op_selection", str),
             mode=check.opt_str_param(mode, "mode"),
             external_partitions_data=check.opt_inst_param(
                 external_partitions_data,
                 "external_partitions_data",
                 ExternalPartitionsDefinitionData,
             ),
         )
@@ -1607,24 +1615,30 @@
         k: external_resource_value_from_raw(v) for k, v in config_schema_default.items()
     }
 
     resource_type_def = resource_def
     if isinstance(resource_type_def, ResourceWithKeyMapping):
         resource_type_def = resource_type_def.wrapped_resource
 
-    resource_type = _get_class_name(type(resource_type_def))
-
-    if isinstance(
+    # use the resource function name as the resource type if it's a function resource
+    # (ie direct instantiation of ResourceDefinition or IOManagerDefinition)
+    if type(resource_type_def) in (ResourceDefinition, IOManagerDefinition):
+        module_name = check.not_none(inspect.getmodule(resource_type_def.resource_fn)).__name__
+        resource_type = f"{module_name}.{resource_type_def.resource_fn.__name__}"
+    # if it's a Pythonic resource, get the underlying Pythonic class name
+    elif isinstance(
         resource_type_def,
         (
             ConfigurableResourceFactoryResourceDefinition,
             ConfigurableIOManagerFactoryResourceDefinition,
         ),
     ):
         resource_type = _get_class_name(resource_type_def.configurable_resource_cls)
+    else:
+        resource_type = _get_class_name(type(resource_type_def))
 
     return ExternalResourceData(
         name=name,
         resource_snapshot=build_resource_def_snap(name, resource_def),
         configured_values=configured_values,
         config_field_snaps=unconfigured_config_type_snap.fields or [],
         config_schema_snap=config_type.get_schema_snapshot(),
@@ -1639,15 +1653,15 @@
 
 def external_schedule_data_from_def(schedule_def: ScheduleDefinition) -> ExternalScheduleData:
     check.inst_param(schedule_def, "schedule_def", ScheduleDefinition)
     return ExternalScheduleData(
         name=schedule_def.name,
         cron_schedule=schedule_def.cron_schedule,
         job_name=schedule_def.job_name,
-        solid_selection=schedule_def._target.solid_selection,  # noqa: SLF001
+        op_selection=schedule_def._target.op_selection,  # noqa: SLF001
         mode=DEFAULT_MODE_NAME,
         environment_vars=schedule_def.environment_vars,
         partition_set_name=None,
         execution_timezone=schedule_def.execution_timezone,
         description=schedule_def.description,
         default_status=schedule_def.default_status,
     )
@@ -1674,14 +1688,19 @@
 def external_time_window_partitions_definition_from_def(
     partitions_def: TimeWindowPartitionsDefinition,
 ) -> ExternalTimeWindowPartitionsDefinitionData:
     check.inst_param(partitions_def, "partitions_def", TimeWindowPartitionsDefinition)
     return ExternalTimeWindowPartitionsDefinitionData(
         cron_schedule=partitions_def.cron_schedule,
         start=pendulum.instance(partitions_def.start, tz=partitions_def.timezone).timestamp(),
+        end=(
+            pendulum.instance(partitions_def.end, tz=partitions_def.timezone).timestamp()
+            if partitions_def.end
+            else None
+        ),
         timezone=partitions_def.timezone,
         fmt=partitions_def.fmt,
         end_offset=partitions_def.end_offset,
     )
 
 
 def external_static_partitions_definition_from_def(
@@ -1742,15 +1761,15 @@
         partitions_def_data = external_multi_partitions_definition_from_def(partitions_def)
     else:
         partitions_def_data = None
 
     return ExternalPartitionSetData(
         name=external_partition_set_name_for_job_name(job_def.name),
         job_name=job_def.name,
-        solid_selection=None,
+        op_selection=None,
         mode=DEFAULT_MODE_NAME,
         external_partitions_data=partitions_def_data,
     )
 
 
 EXTERNAL_PARTITION_SET_NAME_SUFFIX: Final = "_partition_set"
 
@@ -1772,33 +1791,33 @@
     asset_keys = None
     if isinstance(sensor_def, AssetSensorDefinition):
         asset_keys = [sensor_def.asset_key]
 
     if sensor_def.asset_selection is not None:
         target_dict = {
             base_asset_job_name: ExternalTargetData(
-                job_name=base_asset_job_name, mode=DEFAULT_MODE_NAME, solid_selection=None
+                job_name=base_asset_job_name, mode=DEFAULT_MODE_NAME, op_selection=None
             )
             for base_asset_job_name in repository_def.get_implicit_asset_job_names()
         }
     else:
         target_dict = {
             target.job_name: ExternalTargetData(
                 job_name=target.job_name,
                 mode=DEFAULT_MODE_NAME,
-                solid_selection=target.solid_selection,
+                op_selection=target.op_selection,
             )
             for target in sensor_def.targets
         }
 
     return ExternalSensorData(
         name=sensor_def.name,
         job_name=first_target.job_name if first_target else None,
         mode=None,
-        solid_selection=first_target.solid_selection if first_target else None,
+        op_selection=first_target.op_selection if first_target else None,
         target_dict=target_dict,
         min_interval=sensor_def.minimum_interval_seconds,
         description=sensor_def.description,
         metadata=ExternalSensorMetadata(asset_keys=asset_keys),
         default_status=sensor_def.default_status,
         sensor_type=sensor_def.sensor_type,
     )
@@ -1809,12 +1828,12 @@
     if job_def.run_config is None:
         return []
     else:
         return [
             ExternalPresetData(
                 name=DEFAULT_PRESET_NAME,
                 run_config=job_def.run_config,
-                solid_selection=None,
+                op_selection=None,
                 mode=DEFAULT_MODE_NAME,
                 tags={},
             )
         ]
```

### Comparing `dagster-1.3.4/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.5/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.5/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/handle.py` & `dagster-1.3.5/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/historical.py` & `dagster-1.3.5/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/job_index.py` & `dagster-1.3.5/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/origin.py` & `dagster-1.3.5/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/host_representation/represented.py` & `dagster-1.3.5/dagster/_core/host_representation/represented.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,25 +50,25 @@
         return self._job_index.job_snapshot
 
     @property
     def parent_job_snapshot(self) -> Optional[JobSnapshot]:
         return self._job_index.parent_job_snapshot
 
     @property
-    def solid_selection(self) -> Optional[Sequence[str]]:
+    def op_selection(self) -> Optional[Sequence[str]]:
         return (
-            self._job_index.job_snapshot.lineage_snapshot.node_selection
+            self._job_index.job_snapshot.lineage_snapshot.op_selection
             if self._job_index.job_snapshot.lineage_snapshot
             else None
         )
 
     @property
-    def solids_to_execute(self) -> Optional[AbstractSet[str]]:
+    def resolved_op_selection(self) -> Optional[AbstractSet[str]]:
         return (
-            self._job_index.job_snapshot.lineage_snapshot.nodes_to_execute
+            self._job_index.job_snapshot.lineage_snapshot.resolved_op_selection
             if self._job_index.job_snapshot.lineage_snapshot
             else None
         )
 
     # Config
 
     @property
```

### Comparing `dagster-1.3.4/dagster/_core/instance/__init__.py` & `dagster-1.3.5/dagster/_core/instance/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 import yaml
 from typing_extensions import Protocol, Self, TypeAlias, TypeVar, runtime_checkable
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.events import AssetKey
-from dagster._core.definitions.job_base import InMemoryJob
 from dagster._core.errors import (
     DagsterHomeNotSetError,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
     DagsterRunAlreadyExists,
     DagsterRunConflict,
 )
@@ -997,70 +996,70 @@
 
     def create_run_for_job(
         self,
         job_def: "JobDefinition",
         execution_plan: Optional["ExecutionPlan"] = None,
         run_id: Optional[str] = None,
         run_config: Optional[Mapping[str, object]] = None,
-        solids_to_execute: Optional[AbstractSet[str]] = None,
+        resolved_op_selection: Optional[AbstractSet[str]] = None,
         status: Optional[Union[DagsterRunStatus, str]] = None,
         tags: Optional[Mapping[str, str]] = None,
         root_run_id: Optional[str] = None,
         parent_run_id: Optional[str] = None,
-        solid_selection: Optional[Sequence[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         external_job_origin: Optional["ExternalJobOrigin"] = None,
         job_code_origin: Optional[JobPythonOrigin] = None,
         repository_load_data: Optional["RepositoryLoadData"] = None,
     ) -> DagsterRun:
         from dagster._core.definitions.job_definition import JobDefinition
         from dagster._core.execution.api import create_execution_plan
         from dagster._core.execution.plan.plan import ExecutionPlan
         from dagster._core.snap import snapshot_from_execution_plan
 
         check.inst_param(job_def, "pipeline_def", JobDefinition)
         check.opt_inst_param(execution_plan, "execution_plan", ExecutionPlan)
 
-        # note that solids_to_execute is required to execute the solid subset, which is the
+        # note that op_selection is required to execute the solid subset, which is the
         # frozenset version of the previous solid_subset.
-        # solid_selection is not required and will not be converted to solids_to_execute here.
+        # op_selection is not required and will not be converted to op_selection here.
         # i.e. this function doesn't handle solid queries.
-        # solid_selection is only used to pass the user queries further down.
-        check.opt_set_param(solids_to_execute, "solids_to_execute", of_type=str)
-        check.opt_list_param(solid_selection, "solid_selection", of_type=str)
+        # op_selection is only used to pass the user queries further down.
+        check.opt_set_param(resolved_op_selection, "resolved_op_selection", of_type=str)
+        check.opt_list_param(op_selection, "op_selection", of_type=str)
         check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
 
-        # solids_to_execute never provided
-        if asset_selection or solid_selection:
+        # op_selection never provided
+        if asset_selection or op_selection:
             # for cases when `create_run_for_pipeline` is directly called
             job_def = job_def.get_subset(
                 asset_selection=asset_selection,
-                op_selection=solid_selection,
+                op_selection=op_selection,
             )
         step_keys_to_execute = None
 
         if execution_plan:
             step_keys_to_execute = execution_plan.step_keys_to_execute
 
         else:
             execution_plan = create_execution_plan(
-                job=InMemoryJob(job_def),
+                job=job_def,
                 run_config=run_config,
                 instance_ref=self.get_ref() if self.is_persistent else None,
                 tags=tags,
                 repository_load_data=repository_load_data,
             )
 
         return self.create_run(
             job_name=job_def.name,
             run_id=run_id,
             run_config=run_config,
-            solid_selection=solid_selection,
+            op_selection=op_selection,
             asset_selection=asset_selection,
-            solids_to_execute=solids_to_execute,
+            resolved_op_selection=resolved_op_selection,
             step_keys_to_execute=step_keys_to_execute,
             status=DagsterRunStatus(status) if status else None,
             tags=tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
             job_snapshot=job_def.get_job_snapshot(),
             execution_plan_snapshot=snapshot_from_execution_plan(
@@ -1073,25 +1072,25 @@
         )
 
     def _construct_run_with_snapshots(
         self,
         job_name: str,
         run_id: str,
         run_config: Optional[Mapping[str, object]],
-        solids_to_execute: Optional[AbstractSet[str]],
+        resolved_op_selection: Optional[AbstractSet[str]],
         step_keys_to_execute: Optional[Sequence[str]],
         status: Optional[DagsterRunStatus],
         tags: Mapping[str, str],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         job_snapshot: Optional[JobSnapshot],
         execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
         parent_job_snapshot: Optional[JobSnapshot],
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
-        solid_selection: Optional[Sequence[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
         external_job_origin: Optional["ExternalJobOrigin"] = None,
         job_code_origin: Optional[JobPythonOrigin] = None,
     ) -> DagsterRun:
         # https://github.com/dagster-io/dagster/issues/2403
         if tags and IS_AIRFLOW_INGEST_PIPELINE_STR in tags:
             if AIRFLOW_EXECUTION_DATE_STR not in tags:
                 tags = {
@@ -1123,16 +1122,16 @@
         )
 
         return DagsterRun(
             job_name=job_name,
             run_id=run_id,
             run_config=run_config,
             asset_selection=asset_selection,
-            solid_selection=solid_selection,
-            solids_to_execute=solids_to_execute,
+            op_selection=op_selection,
+            resolved_op_selection=resolved_op_selection,
             step_keys_to_execute=step_keys_to_execute,
             status=status,
             tags=tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
             job_snapshot_id=job_snapshot_id,
             execution_plan_snapshot_id=execution_plan_snapshot_id,
@@ -1281,16 +1280,16 @@
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         step_keys_to_execute: Optional[Sequence[str]],
         execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
         job_snapshot: Optional[JobSnapshot],
         parent_job_snapshot: Optional[JobSnapshot],
         asset_selection: Optional[AbstractSet[AssetKey]],
-        solids_to_execute: Optional[AbstractSet[str]],
-        solid_selection: Optional[Sequence[str]],
+        resolved_op_selection: Optional[AbstractSet[str]],
+        op_selection: Optional[Sequence[str]],
         external_job_origin: Optional["ExternalJobOrigin"],
         job_code_origin: Optional[JobPythonOrigin],
     ) -> DagsterRun:
         from dagster._core.definitions.utils import validate_tags
         from dagster._core.host_representation.origin import ExternalJobOrigin
         from dagster._core.snap import ExecutionPlanSnapshot, JobSnapshot
 
@@ -1334,48 +1333,48 @@
 
         if parent_job_snapshot:
             check.invariant(
                 job_snapshot,
                 "If parent_job_snapshot is set, job_snapshot should also be.",
             )
 
-        # solid_selection is a sequence of selection queries assigned by the user.
-        # *Most* callers expand the solid_selection into an explicit set of
-        # solids_to_execute via accessing external_job.solids_to_execute
+        # op_selection is a sequence of selection queries assigned by the user.
+        # *Most* callers expand the op_selection into an explicit set of
+        # resolved_op_selection via accessing external_job.resolved_op_selection
         # but not all do. Some (launch execution mutation in graphql and backfill run
         # creation, for example) actually pass the solid *selection* into the
-        # solids_to_execute parameter, but just as a frozen set, rather than
+        # resolved_op_selection parameter, but just as a frozen set, rather than
         # fully resolving the selection, as the daemon launchers do. Given the
         # state of callers we just check to ensure that the arguments are well-formed.
         #
-        # asset_selection adds another dimension to this lovely dance. solid_selection
+        # asset_selection adds another dimension to this lovely dance. op_selection
         # and asset_selection are mutually exclusive and should never both be set.
         # This is invariant is checked in a sporadic fashion around
         # the codebase, but is never enforced in a typed fashion.
         #
         # Additionally, the way that callsites currently behave *if* asset selection
-        # is set (i.e., not None) then *neither* solid_selection *nor*
-        # solids_to_execute is passed. In the asset selection case resolving
-        # the set of assets into the canonical solids_to_execute is done in
+        # is set (i.e., not None) then *neither* op_selection *nor*
+        # resolved_op_selection is passed. In the asset selection case resolving
+        # the set of assets into the canonical resolved_op_selection is done in
         # the user process, and the exact resolution is never persisted in the run.
         # We are asserting that invariant here to maintain that behavior.
 
-        check.opt_set_param(solids_to_execute, "solids_to_execute", of_type=str)
-        check.opt_sequence_param(solid_selection, "solid_selection", of_type=str)
+        check.opt_set_param(resolved_op_selection, "resolved_op_selection", of_type=str)
+        check.opt_sequence_param(op_selection, "op_selection", of_type=str)
         check.opt_set_param(asset_selection, "asset_selection", of_type=AssetKey)
 
         if asset_selection is not None:
             check.invariant(
-                solid_selection is None,
-                "Cannot pass both asset_selection and solid_selection",
+                op_selection is None,
+                "Cannot pass both asset_selection and op_selection",
             )
 
             check.invariant(
-                solids_to_execute is None,
-                "Cannot pass both asset_selection and solids_to_execute",
+                resolved_op_selection is None,
+                "Cannot pass both asset_selection and resolved_op_selection",
             )
 
         # The "python origin" arguments exist so a job can be reconstructed in memory
         # after a DagsterRun has been fetched from the database.
         #
         # There are cases (notably in _logged_execute_job with Reconstructable jobs)
         # where job_code_origin and is not. In some cloud test cases only
@@ -1387,16 +1386,16 @@
         check.opt_inst_param(job_code_origin, "job_code_origin", JobPythonOrigin)
 
         dagster_run = self._construct_run_with_snapshots(
             job_name=job_name,
             run_id=run_id,  # type: ignore  # (possible none)
             run_config=run_config,
             asset_selection=asset_selection,
-            solid_selection=solid_selection,
-            solids_to_execute=solids_to_execute,
+            op_selection=op_selection,
+            resolved_op_selection=resolved_op_selection,
             step_keys_to_execute=step_keys_to_execute,
             status=status,
             tags=validated_tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
             job_snapshot=job_snapshot,
             execution_plan_snapshot=execution_plan_snapshot,
@@ -1482,43 +1481,43 @@
             instance=self,
         )
 
         return self.create_run(
             job_name=parent_run.job_name,
             run_id=None,
             run_config=run_config,
-            solids_to_execute=parent_run.solids_to_execute,
+            resolved_op_selection=parent_run.resolved_op_selection,
             step_keys_to_execute=step_keys_to_execute,
             status=DagsterRunStatus.NOT_STARTED,
             tags=tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
             job_snapshot=external_job.job_snapshot,
             execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
             parent_job_snapshot=external_job.parent_job_snapshot,
-            solid_selection=parent_run.solid_selection,
+            op_selection=parent_run.op_selection,
             asset_selection=parent_run.asset_selection,
             external_job_origin=external_job.get_external_origin(),
             job_code_origin=external_job.get_python_origin(),
         )
 
     def register_managed_run(
         self,
         job_name: str,
         run_id: str,
         run_config: Optional[Mapping[str, object]],
-        solids_to_execute: Optional[AbstractSet[str]],
+        resolved_op_selection: Optional[AbstractSet[str]],
         step_keys_to_execute: Optional[Sequence[str]],
         tags: Mapping[str, str],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         job_snapshot: Optional[JobSnapshot],
         execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
         parent_job_snapshot: Optional[JobSnapshot],
-        solid_selection: Optional[Sequence[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
         job_code_origin: Optional[JobPythonOrigin] = None,
     ) -> DagsterRun:
         # The usage of this method is limited to dagster-airflow, specifically in Dagster
         # Operators that are executed in Airflow. Because a common workflow in Airflow is to
         # retry dags from arbitrary tasks, we need any node to be capable of creating a
         # DagsterRun.
         #
@@ -1528,16 +1527,16 @@
         # error; at this point, the failed tasks try again to fetch the existing run.
         # https://github.com/dagster-io/dagster/issues/2412
 
         dagster_run = self._construct_run_with_snapshots(
             job_name=job_name,
             run_id=run_id,
             run_config=run_config,
-            solid_selection=solid_selection,
-            solids_to_execute=solids_to_execute,
+            op_selection=op_selection,
+            resolved_op_selection=resolved_op_selection,
             step_keys_to_execute=step_keys_to_execute,
             status=DagsterRunStatus.MANAGED,
             tags=tags,
             root_run_id=root_run_id,
             parent_run_id=parent_run_id,
             job_snapshot=job_snapshot,
             execution_plan_snapshot=execution_plan_snapshot,
```

### Comparing `dagster-1.3.4/dagster/_core/instance/config.py` & `dagster-1.3.5/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/instance/ref.py` & `dagster-1.3.5/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/instance_for_test.py` & `dagster-1.3.5/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/launcher/base.py` & `dagster-1.3.5/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.5/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.5/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/log_manager.py` & `dagster-1.3.5/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/nux.py` & `dagster-1.3.5/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/origin.py` & `dagster-1.3.5/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/run_coordinator/base.py` & `dagster-1.3.5/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.5/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.5/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/scheduler/__init__.py` & `dagster-1.3.5/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/scheduler/execution.py` & `dagster-1.3.5/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/scheduler/instigation.py` & `dagster-1.3.5/dagster/_core/scheduler/instigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 from typing import List, NamedTuple, Optional, Sequence, Union
 
 from typing_extensions import TypeAlias
 
 import dagster._check as check
+from dagster._core.definitions.asset_reconciliation_sensor import AutoMaterializeAssetEvaluation
 
 # re-export
 from dagster._core.definitions.run_request import (
     InstigatorType as InstigatorType,
     SkipReason as SkipReason,
 )
 from dagster._core.definitions.selector import InstigatorSelector, RepositorySelector
@@ -584,7 +585,12 @@
         check.invariant(error is None, "Tick status was not FAILURE but error was provided")
 
     if skip_reason:
         check.invariant(
             status == TickStatus.SKIPPED,
             "Tick status was not SKIPPED but skip_reason was provided",
         )
+
+
+class AutoMaterializeAssetEvaluationRecord(NamedTuple):
+    evaluation: AutoMaterializeAssetEvaluation
+    evaluation_id: int
```

### Comparing `dagster-1.3.4/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.5/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/secrets/env_file.py` & `dagster-1.3.5/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/selector/subset_selector.py` & `dagster-1.3.5/dagster/_core/selector/subset_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,22 +370,22 @@
 
     Note:
     - If one of the query clauses is invalid, we will skip that one and continue to parse the valid
         ones.
 
     Args:
         pipeline_def (JobDefinition): the pipeline to execute.
-        solid_selection (List[str]): a list of the solid selection queries (including single solid
+        op_queries (List[str]): a list of the solid selection queries (including single solid
             names) to execute.
 
     Returns:
         FrozenSet[str]: a frozenset of qualified deduplicated solid names, empty if no qualified
             subset selected.
     """
-    check.sequence_param(op_queries, "solid_selection", of_type=str)
+    check.sequence_param(op_queries, "op_queries", of_type=str)
 
     # special case: select all
     if len(op_queries) == 1 and op_queries[0] == "*":
         return frozenset(graph_def.node_names())
 
     graph = generate_dep_graph(graph_def)
     node_names: Set[str] = set()
```

### Comparing `dagster-1.3.4/dagster/_core/snap/__init__.py` & `dagster-1.3.5/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/snap/dagster_types.py` & `dagster-1.3.5/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.5/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.5/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/snap/job_snapshot.py` & `dagster-1.3.5/dagster/_core/snap/job_snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         check.inst_param(job_def, "job_def", JobDefinition)
         lineage = None
         if job_def.op_selection_data:
             lineage = JobLineageSnapshot(
                 parent_snapshot_id=create_job_snapshot_id(
                     cls.from_job_def(job_def.op_selection_data.parent_job_def)
                 ),
-                node_selection=sorted(job_def.op_selection_data.op_selection),
-                nodes_to_execute=job_def.op_selection_data.resolved_op_selection,
+                op_selection=sorted(job_def.op_selection_data.op_selection),
+                resolved_op_selection=job_def.op_selection_data.resolved_op_selection,
             )
         if job_def.asset_selection_data:
             lineage = JobLineageSnapshot(
                 parent_snapshot_id=create_job_snapshot_id(
                     cls.from_job_def(job_def.asset_selection_data.parent_job_def)
                 ),
                 asset_selection=job_def.asset_selection_data.asset_selection,
@@ -399,37 +399,37 @@
         return _construct_noneable_from_snap(config_type_snap, config_snap_map)
     check.failed(f"Could not evaluate config type snap kind: {config_type_snap.kind}")
 
 
 @whitelist_for_serdes(
     storage_name="PipelineSnapshotLineage",
     storage_field_names={
-        "node_selection": "solid_selection",
-        "nodes_to_execute": "solids_to_execute",
+        "op_selection": "solid_selection",
+        "resolved_op_selection": "solids_to_execute",
     },
 )
 class JobLineageSnapshot(
     NamedTuple(
         "_JobLineageSnapshot",
         [
             ("parent_snapshot_id", str),
-            ("node_selection", Optional[Sequence[str]]),
-            ("nodes_to_execute", Optional[AbstractSet[str]]),
+            ("op_selection", Optional[Sequence[str]]),
+            ("resolved_op_selection", Optional[AbstractSet[str]]),
             ("asset_selection", Optional[AbstractSet[AssetKey]]),
         ],
     )
 ):
     def __new__(
         cls,
         parent_snapshot_id: str,
-        node_selection: Optional[Sequence[str]] = None,
-        nodes_to_execute: Optional[AbstractSet[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
+        resolved_op_selection: Optional[AbstractSet[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ):
-        check.opt_set_param(nodes_to_execute, "nodes_to_execute", of_type=str)
+        check.opt_set_param(resolved_op_selection, "resolved_op_selection", of_type=str)
         return super(JobLineageSnapshot, cls).__new__(
             cls,
             check.str_param(parent_snapshot_id, parent_snapshot_id),
-            node_selection,
-            nodes_to_execute,
+            op_selection,
+            resolved_op_selection,
             asset_selection,
         )
```

### Comparing `dagster-1.3.4/dagster/_core/snap/mode.py` & `dagster-1.3.5/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/snap/node.py` & `dagster-1.3.5/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.3.5/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.5/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/README.md` & `dagster-1.3.5/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/env.py` & `dagster-1.3.5/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.3.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.5/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/base_storage.py` & `dagster-1.3.5/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.5/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.5/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.5/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.5/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/config.py` & `dagster-1.3.5/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/dagster_run.py` & `dagster-1.3.5/dagster/_core/storage/dagster_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,26 +217,28 @@
     storage_name="PipelineRun",
     old_fields={"mode": None},
     storage_field_names={
         "job_name": "pipeline_name",
         "job_snapshot_id": "pipeline_snapshot_id",
         "external_job_origin": "external_pipeline_origin",
         "job_code_origin": "pipeline_code_origin",
+        "op_selection": "solid_selection",
+        "resolved_op_selection": "solids_to_execute",
     },
 )
 class DagsterRun(
     NamedTuple(
         "_DagsterRun",
         [
             ("job_name", PublicAttr[str]),
             ("run_id", str),
             ("run_config", Mapping[str, object]),
             ("asset_selection", Optional[AbstractSet[AssetKey]]),
-            ("solid_selection", Optional[Sequence[str]]),
-            ("solids_to_execute", Optional[AbstractSet[str]]),
+            ("op_selection", Optional[Sequence[str]]),
+            ("resolved_op_selection", Optional[AbstractSet[str]]),
             ("step_keys_to_execute", Optional[Sequence[str]]),
             ("status", DagsterRunStatus),
             ("tags", Mapping[str, str]),
             ("root_run_id", Optional[str]),
             ("parent_run_id", Optional[str]),
             ("job_snapshot_id", Optional[str]),
             ("execution_plan_snapshot_id", Optional[str]),
@@ -252,16 +254,16 @@
 
     def __new__(
         cls,
         job_name: str,
         run_id: Optional[str] = None,
         run_config: Optional[Mapping[str, object]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
-        solid_selection: Optional[Sequence[str]] = None,
-        solids_to_execute: Optional[AbstractSet[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
+        resolved_op_selection: Optional[AbstractSet[str]] = None,
         step_keys_to_execute: Optional[Sequence[str]] = None,
         status: Optional[DagsterRunStatus] = None,
         tags: Optional[Mapping[str, str]] = None,
         root_run_id: Optional[str] = None,
         parent_run_id: Optional[str] = None,
         job_snapshot_id: Optional[str] = None,
         execution_plan_snapshot_id: Optional[str] = None,
@@ -273,23 +275,21 @@
             (root_run_id is not None and parent_run_id is not None)
             or (root_run_id is None and parent_run_id is None),
             (
                 "Must set both root_run_id and parent_run_id when creating a PipelineRun that "
                 "belongs to a run group"
             ),
         )
-        # a frozenset which contains the names of the solids to execute
-        solids_to_execute = check.opt_nullable_set_param(
-            solids_to_execute, "solids_to_execute", of_type=str
-        )
-        # a list of solid queries provided by the user
-        # possible to be None when only solids_to_execute is set by the user directly
-        solid_selection = check.opt_nullable_sequence_param(
-            solid_selection, "solid_selection", of_type=str
+        # a set which contains the names of the ops to execute
+        resolved_op_selection = check.opt_nullable_set_param(
+            resolved_op_selection, "resolved_op_selection", of_type=str
         )
+        # a list of op queries provided by the user
+        # possible to be None when resolved_op_selection is set by the user directly
+        op_selection = check.opt_nullable_sequence_param(op_selection, "op_selection", of_type=str)
         check.opt_nullable_sequence_param(step_keys_to_execute, "step_keys_to_execute", of_type=str)
 
         asset_selection = check.opt_nullable_set_param(
             asset_selection, "asset_selection", of_type=AssetKey
         )
 
         # Placing this with the other imports causes a cyclic import
@@ -308,17 +308,17 @@
             run_id = make_new_run_id()
 
         return super(DagsterRun, cls).__new__(
             cls,
             job_name=check.str_param(job_name, "job_name"),
             run_id=check.str_param(run_id, "run_id"),
             run_config=check.opt_mapping_param(run_config, "run_config", key_type=str),
-            solid_selection=solid_selection,
+            op_selection=op_selection,
             asset_selection=asset_selection,
-            solids_to_execute=solids_to_execute,
+            resolved_op_selection=resolved_op_selection,
             step_keys_to_execute=step_keys_to_execute,
             status=check.opt_inst_param(
                 status, "status", DagsterRunStatus, DagsterRunStatus.NOT_STARTED
             ),
             tags=check.opt_mapping_param(tags, "tags", key_type=str, value_type=str),
             root_run_id=check.opt_str_param(root_run_id, "root_run_id"),
             parent_run_id=check.opt_str_param(parent_run_id, "parent_run_id"),
```

### Comparing `dagster-1.3.4/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.5/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.5/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/base.py` & `dagster-1.3.5/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.5/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.5/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.5/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.5/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.5/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/file_manager.py` & `dagster-1.3.5/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.5/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/input_manager.py` & `dagster-1.3.5/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/io_manager.py` & `dagster-1.3.5/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.5/dagster/_core/storage/legacy_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,19 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Union,
 )
 
-from dagster import _check as check
+from dagster import (
+    _check as check,
+)
 from dagster._config.config_schema import UserConfigSchema
+from dagster._core.definitions.asset_reconciliation_sensor import AutoMaterializeAssetEvaluation
 from dagster._core.event_api import EventHandlerFn
 from dagster._serdes import ConfigurableClass, ConfigurableClassData
 from dagster._utils import PrintFn
 
 from .base_storage import DagsterStorage
 from .event_log.base import (
     AssetRecord,
@@ -32,14 +35,15 @@
     from dagster._core.events import DagsterEvent, DagsterEventType
     from dagster._core.events.log import EventLogEntry
     from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
     from dagster._core.execution.stats import RunStepKeyStatsSnapshot
     from dagster._core.host_representation.origin import ExternalJobOrigin
     from dagster._core.instance import DagsterInstance
     from dagster._core.scheduler.instigation import (
+        AutoMaterializeAssetEvaluationRecord,
         InstigatorState,
         InstigatorStatus,
         InstigatorTick,
         TickData,
         TickStatus,
     )
     from dagster._core.snap.execution_plan_snapshot import ExecutionPlanSnapshot
@@ -643,14 +647,30 @@
         before: float,
         tick_statuses: Optional[Sequence["TickStatus"]] = None,
     ) -> None:
         return self._storage.schedule_storage.purge_ticks(
             origin_id, selector_id, before, tick_statuses
         )
 
+    def add_auto_materialize_asset_evaluations(
+        self,
+        evaluation_id: int,
+        asset_evaluations: Sequence[AutoMaterializeAssetEvaluation],
+    ) -> None:
+        return self._storage.schedule_storage.add_auto_materialize_asset_evaluations(
+            evaluation_id, asset_evaluations
+        )
+
+    def get_auto_materialize_asset_evaluations(
+        self, asset_key: "AssetKey", limit: int, cursor: Optional[int] = None
+    ) -> Sequence["AutoMaterializeAssetEvaluationRecord"]:
+        return self._storage.schedule_storage.get_auto_materialize_asset_evaluations(
+            asset_key, limit, cursor
+        )
+
     def upgrade(self) -> None:
         return self._storage.schedule_storage.upgrade()
 
     def migrate(self, print_fn: Optional[PrintFn] = None, force_rebuild_all: bool = False) -> None:
         return self._storage.schedule_storage.migrate(print_fn, force_rebuild_all)
 
     def optimize(self, print_fn: Optional[PrintFn] = None, force_rebuild_all: bool = False) -> None:
```

### Comparing `dagster-1.3.4/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.5/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.5/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.5/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/migration/utils.py` & `dagster-1.3.5/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.5/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/output_manager.py` & `dagster-1.3.5/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.5/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/root.py` & `dagster-1.3.5/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.5/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/base.py` & `dagster-1.3.5/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.5/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/migration.py` & `dagster-1.3.5/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/schema.py` & `dagster-1.3.5/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.5/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/schedules/base.py` & `dagster-1.3.5/dagster/_core/storage/schedules/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import abc
 from typing import Mapping, Optional, Sequence, Set
 
+from dagster import AssetKey
+from dagster._core.definitions.asset_reconciliation_sensor import AutoMaterializeAssetEvaluation
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.scheduler.instigation import (
+    AutoMaterializeAssetEvaluationRecord,
     InstigatorState,
     InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.sql import AlembicVersion
@@ -131,14 +134,34 @@
             origin_id (str): The id of the instigator target to delete
             selector_id (str): The logical instigator identifier
             before (datetime): All ticks before this datetime will get purged
             tick_statuses (Optional[List[TickStatus]]): The tick statuses to wipe
         """
 
     @abc.abstractmethod
+    def add_auto_materialize_asset_evaluations(
+        self,
+        evaluation_id: int,
+        asset_evaluations: Sequence[AutoMaterializeAssetEvaluation],
+    ) -> None:
+        """Add asset policy evaluations to storage."""
+
+    @abc.abstractmethod
+    def get_auto_materialize_asset_evaluations(
+        self, asset_key: AssetKey, limit: int, cursor: Optional[int] = None
+    ) -> Sequence[AutoMaterializeAssetEvaluationRecord]:
+        """Get the policy evaluations for a given asset.
+
+        Args:
+            asset_key (AssetKey): The asset key to query
+            limit (Optional[int]): The maximum number of evaluations to return
+            cursor (Optional[int]): The cursor to paginate from
+        """
+
+    @abc.abstractmethod
     def upgrade(self) -> None:
         """Perform any needed migrations."""
 
     def migrate(self, print_fn: Optional[PrintFn] = None, force_rebuild_all: bool = False) -> None:
         """Call this method to run any required data migrations."""
 
     def optimize(self, print_fn: Optional[PrintFn] = None, force_rebuild_all: bool = False) -> None:
```

### Comparing `dagster-1.3.4/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.5/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.5/dagster/_core/storage/schedules/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sqlalchemy as db
+from sqlalchemy.dialects import sqlite
 
 from ..sql import MySQLCompatabilityTypes, get_current_timestamp
 
 ScheduleStorageSqlMetadata = db.MetaData()
 
 JobTable = db.Table(
     "jobs",
@@ -41,14 +42,35 @@
     db.Column("type", db.String(63)),
     db.Column("timestamp", db.types.TIMESTAMP),
     db.Column("tick_body", db.Text),
     db.Column("create_timestamp", db.DateTime, server_default=get_current_timestamp()),
     db.Column("update_timestamp", db.DateTime, server_default=get_current_timestamp()),
 )
 
+AssetPolicyEvaluationsTable = db.Table(
+    "asset_daemon_asset_evaluations",
+    ScheduleStorageSqlMetadata,
+    db.Column(
+        "id",
+        db.BigInteger().with_variant(sqlite.INTEGER(), "sqlite"),
+        primary_key=True,
+        autoincrement=True,
+    ),
+    db.Column(
+        "evaluation_id", db.BigInteger().with_variant(sqlite.INTEGER(), "sqlite"), index=True
+    ),
+    db.Column("asset_key", db.Text),
+    db.Column("asset_evaluation_body", db.Text),
+    db.Column("num_requested", db.Integer),
+    db.Column("num_skipped", db.Integer),
+    db.Column("num_discarded", db.Integer),
+    db.Column("create_timestamp", db.DateTime, server_default=get_current_timestamp()),
+)
+
+
 # Secondary Index migration table, used to track data migrations, event_logs and runs.
 # This schema should match the schema in the event_log storage, run schema
 SecondaryIndexMigrationTable = db.Table(
     "secondary_indexes",
     ScheduleStorageSqlMetadata,
     db.Column("id", db.Integer, primary_key=True, autoincrement=True),
     db.Column("name", MySQLCompatabilityTypes.UniqueText, unique=True),
@@ -60,7 +82,14 @@
     "idx_job_tick_status",
     JobTickTable.c.job_origin_id,
     JobTickTable.c.status,
     mysql_length=32,
 )
 db.Index("idx_job_tick_timestamp", JobTickTable.c.job_origin_id, JobTickTable.c.timestamp)
 db.Index("idx_tick_selector_timestamp", JobTickTable.c.selector_id, JobTickTable.c.timestamp)
+
+db.Index(
+    "idx_asset_daemon_asset_evaluations_asset_key_evaluation_id",
+    AssetPolicyEvaluationsTable.c.asset_key,
+    AssetPolicyEvaluationsTable.c.evaluation_id,
+    unique=True,
+)
```

### Comparing `dagster-1.3.4/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.5/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 
 import pendulum
 import sqlalchemy as db
 import sqlalchemy.exc as db_exc
 from sqlalchemy.engine import Connection
 
 import dagster._check as check
+from dagster._core.definitions.asset_reconciliation_sensor import AutoMaterializeAssetEvaluation
+from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.scheduler.instigation import (
+    AutoMaterializeAssetEvaluationRecord,
     InstigatorState,
     InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.sql import SqlAlchemyQuery, SqlAlchemyRow
@@ -37,15 +40,21 @@
 from .base import ScheduleStorage
 from .migration import (
     OPTIONAL_SCHEDULE_DATA_MIGRATIONS,
     REQUIRED_SCHEDULE_DATA_MIGRATIONS,
     SCHEDULE_JOBS_SELECTOR_ID,
     SCHEDULE_TICKS_SELECTOR_ID,
 )
-from .schema import InstigatorsTable, JobTable, JobTickTable, SecondaryIndexMigrationTable
+from .schema import (
+    AssetPolicyEvaluationsTable,
+    InstigatorsTable,
+    JobTable,
+    JobTickTable,
+    SecondaryIndexMigrationTable,
+)
 
 T_NamedTuple = TypeVar("T_NamedTuple", bound=NamedTuple)
 
 
 class SqlScheduleStorage(ScheduleStorage):
     """Base class for SQL backed schedule storage."""
 
@@ -442,14 +451,67 @@
             )
         else:
             query = query.where(JobTickTable.c.job_origin_id == origin_id)
 
         with self.connect() as conn:
             conn.execute(query)
 
+    def add_auto_materialize_asset_evaluations(
+        self,
+        evaluation_id: int,
+        asset_evaluations: Sequence[AutoMaterializeAssetEvaluation],
+    ):
+        if not asset_evaluations:
+            return
+
+        with self.connect() as conn:
+            bulk_insert = AssetPolicyEvaluationsTable.insert().values(
+                [
+                    {
+                        "evaluation_id": evaluation_id,
+                        "asset_key": evaluation.asset_key.to_string(),
+                        "asset_evaluation_body": serialize_value(evaluation),
+                        "num_requested": evaluation.num_requested,
+                        "num_skipped": evaluation.num_skipped,
+                        "num_discarded": evaluation.num_discarded,
+                    }
+                    for evaluation in asset_evaluations
+                ]
+            )
+            conn.execute(bulk_insert)
+
+    def get_auto_materialize_asset_evaluations(
+        self, asset_key: AssetKey, limit: int, cursor: Optional[int] = None
+    ) -> Sequence[AutoMaterializeAssetEvaluationRecord]:
+        with self.connect() as conn:
+            query = (
+                db.select(
+                    [
+                        AssetPolicyEvaluationsTable.c.asset_evaluation_body,
+                        AssetPolicyEvaluationsTable.c.evaluation_id,
+                    ]
+                )
+                .where(AssetPolicyEvaluationsTable.c.asset_key == asset_key.to_string())
+                .order_by(AssetPolicyEvaluationsTable.c.evaluation_id.desc())
+            ).limit(limit)
+
+            if cursor:
+                query = query.where(AssetPolicyEvaluationsTable.c.evaluation_id < cursor)
+
+            rows = conn.execute(query)
+            return [
+                AutoMaterializeAssetEvaluationRecord(
+                    evaluation=deserialize_value(
+                        row["asset_evaluation_body"], AutoMaterializeAssetEvaluation
+                    ),
+                    evaluation_id=row["evaluation_id"],
+                )
+                for row in rows
+            ]
+
     def wipe(self) -> None:
         """Clears the schedule storage."""
         with self.connect() as conn:
             # https://stackoverflow.com/a/54386260/324449
             conn.execute(JobTable.delete())
             conn.execute(JobTickTable.delete())
             if self._has_instigators_table(conn):
```

### Comparing `dagster-1.3.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/sql.py` & `dagster-1.3.5/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/sqlite.py` & `dagster-1.3.5/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.5/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/tags.py` & `dagster-1.3.5/dagster/_core/storage/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 RESUME_RETRY_TAG = f"{SYSTEM_TAG_PREFIX}is_resume_retry"
 
 MEMOIZED_RUN_TAG = f"{SYSTEM_TAG_PREFIX}is_memoized_run"
 
 STEP_SELECTION_TAG = f"{SYSTEM_TAG_PREFIX}step_selection"
 
-SOLID_SELECTION_TAG = f"{SYSTEM_TAG_PREFIX}solid_selection"
+OP_SELECTION_TAG = f"{SYSTEM_TAG_PREFIX}solid_selection"
 
 PRESET_NAME_TAG = f"{SYSTEM_TAG_PREFIX}preset_name"
 
 GRPC_INFO_TAG = f"{HIDDEN_TAG_PREFIX}grpc_info"
 
 SCHEDULED_EXECUTION_TIME_TAG = f"{HIDDEN_TAG_PREFIX}scheduled_execution_time"
```

### Comparing `dagster-1.3.4/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.5/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.5/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.5/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/system_config/objects.py` & `dagster-1.3.5/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/telemetry.py` & `dagster-1.3.5/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/telemetry_upload.py` & `dagster-1.3.5/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/test_utils.py` & `dagster-1.3.5/dagster/_core/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,27 +96,27 @@
             yield step_event
 
 
 def nesting_graph(depth: int, num_children: int, name: Optional[str] = None) -> GraphDefinition:
     """Creates a job of nested graphs up to "depth" layers, with a fan-out of
     num_children at each layer.
 
-    Total number of solids will be num_children ^ depth
+    Total number of ops will be num_children ^ depth
     """
 
     @op
     def leaf_node(_):
         return 1
 
     def create_wrap(inner: NodeDefinition, name: str) -> GraphDefinition:
         @graph(name=name)
         def wrap():
             for i in range(num_children):
-                solid_alias = "%s_node_%d" % (name, i)
-                inner.alias(solid_alias)()
+                op_alias = "%s_node_%d" % (name, i)
+                inner.alias(op_alias)()
 
         return wrap
 
     @graph(name=name)
     def nested_graph():
         graph_def = create_wrap(leaf_node, "layer_%d" % depth)
 
@@ -132,67 +132,67 @@
 
 
 def create_run_for_test(
     instance: DagsterInstance,
     job_name: str = TEST_JOB_NAME,
     run_id=None,
     run_config=None,
-    solids_to_execute=None,
+    resolved_op_selection=None,
     step_keys_to_execute=None,
     status=None,
     tags=None,
     root_run_id=None,
     parent_run_id=None,
     job_snapshot=None,
     execution_plan_snapshot=None,
     parent_job_snapshot=None,
     external_job_origin=None,
     job_code_origin=None,
     asset_selection=None,
-    solid_selection=None,
+    op_selection=None,
 ):
     return instance.create_run(
         job_name=job_name,
         run_id=run_id,
         run_config=run_config,
-        solids_to_execute=solids_to_execute,
+        resolved_op_selection=resolved_op_selection,
         step_keys_to_execute=step_keys_to_execute,
         status=status,
         tags=tags,
         root_run_id=root_run_id,
         parent_run_id=parent_run_id,
         job_snapshot=job_snapshot,
         execution_plan_snapshot=execution_plan_snapshot,
         parent_job_snapshot=parent_job_snapshot,
         external_job_origin=external_job_origin,
         job_code_origin=job_code_origin,
         asset_selection=asset_selection,
-        solid_selection=solid_selection,
+        op_selection=op_selection,
     )
 
 
 def register_managed_run_for_test(
     instance,
     job_name=TEST_JOB_NAME,
     run_id=None,
     run_config=None,
-    solids_to_execute=None,
+    resolved_op_selection=None,
     step_keys_to_execute=None,
     tags=None,
     root_run_id=None,
     parent_run_id=None,
     job_snapshot=None,
     execution_plan_snapshot=None,
     parent_job_snapshot=None,
 ):
     return instance.register_managed_run(
         job_name,
         run_id,
         run_config,
-        solids_to_execute,
+        resolved_op_selection,
         step_keys_to_execute,
         tags,
         root_run_id,
         parent_run_id,
         job_snapshot,
         execution_plan_snapshot,
         parent_job_snapshot,
```

### Comparing `dagster-1.3.4/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.5/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/config_schema.py` & `dagster-1.3.5/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/dagster_type.py` & `dagster-1.3.5/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/decorator.py` & `dagster-1.3.5/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.5/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.5/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/python_dict.py` & `dagster-1.3.5/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/python_set.py` & `dagster-1.3.5/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/python_tuple.py` & `dagster-1.3.5/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/types/transform_typing.py` & `dagster-1.3.5/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/utility_ops.py` & `dagster-1.3.5/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/utils.py` & `dagster-1.3.5/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.5/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/config_schema.py` & `dagster-1.3.5/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/context.py` & `dagster-1.3.5/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/load.py` & `dagster-1.3.5/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/load_target.py` & `dagster-1.3.5/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/permissions.py` & `dagster-1.3.5/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_core/workspace/workspace.py` & `dagster-1.3.5/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/__init__.py` & `dagster-1.3.5/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/asset_daemon.py` & `dagster-1.3.5/dagster/_daemon/asset_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         raw_cursor = persisted_info.get(CURSOR_KEY)
         cursor = (
             AssetReconciliationCursor.from_serialized(raw_cursor, asset_graph)
             if raw_cursor
             else AssetReconciliationCursor.empty()
         )
 
-        run_requests, new_cursor = reconcile(
+        run_requests, new_cursor, _ = reconcile(
             asset_graph=asset_graph,
             target_asset_keys=target_asset_keys,
             instance=instance,
             cursor=cursor,
             run_tags=None,
         )
 
@@ -96,15 +96,15 @@
 
             code_location = workspace.get_code_location(location_name)
             external_job = code_location.get_external_job(
                 JobSubsetSelector(
                     location_name=location_name,
                     repository_name=repository_name,
                     job_name=job_name,
-                    solid_selection=None,
+                    op_selection=None,
                     asset_selection=asset_keys,
                 )
             )
 
             tags = {
                 **run_request.tags,
                 AUTO_MATERIALIZE_TAG: "true",
@@ -120,18 +120,18 @@
             )
             execution_plan_snapshot = external_execution_plan.execution_plan_snapshot
 
             run = instance.create_run(
                 job_name=external_job.name,
                 run_id=None,
                 run_config=None,
-                solids_to_execute=None,
+                resolved_op_selection=None,
                 step_keys_to_execute=None,
                 status=DagsterRunStatus.NOT_STARTED,
-                solid_selection=None,
+                op_selection=None,
                 root_run_id=None,
                 parent_run_id=None,
                 tags=tags,
                 job_snapshot=external_job.job_snapshot,
                 execution_plan_snapshot=execution_plan_snapshot,
                 parent_job_snapshot=external_job.parent_job_snapshot,
                 external_job_origin=external_job.get_external_origin(),
```

### Comparing `dagster-1.3.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         return
 
     external_job = code_location.get_external_job(
         JobSubsetSelector(
             location_name=origin.code_location_origin.location_name,
             repository_name=repo_name,
             job_name=failed_run.job_name,
-            solid_selection=failed_run.solid_selection,
+            op_selection=failed_run.op_selection,
             asset_selection=None
             if failed_run.asset_selection is None
             else list(failed_run.asset_selection),
         )
     )
 
     strategy = get_reexecution_strategy(failed_run, instance) or DEFAULT_REEXECUTION_POLICY
```

### Comparing `dagster-1.3.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/backfill.py` & `dagster-1.3.5/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/cli/__init__.py` & `dagster-1.3.5/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/controller.py` & `dagster-1.3.5/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/daemon.py` & `dagster-1.3.5/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.5/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/sensor.py` & `dagster-1.3.5/dagster/_daemon/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,15 @@
             external_sensor.get_target_data(run_request.job_name)
         )
 
         job_subset_selector = JobSubsetSelector(
             location_name=code_location.name,
             repository_name=sensor_origin.external_repository_origin.repository_name,
             job_name=target_data.job_name,
-            solid_selection=target_data.solid_selection,
+            op_selection=target_data.op_selection,
             asset_selection=run_request.asset_selection,
         )
         external_job = code_location.get_external_job(job_subset_selector)
         run = _get_or_create_sensor_run(
             context,
             instance,
             code_location,
@@ -936,18 +936,18 @@
         },
     )
 
     return instance.create_run(
         job_name=target_data.job_name,
         run_id=None,
         run_config=run_request.run_config,
-        solids_to_execute=external_job.solids_to_execute,
+        resolved_op_selection=external_job.resolved_op_selection,
         step_keys_to_execute=None,
         status=DagsterRunStatus.NOT_STARTED,
-        solid_selection=target_data.solid_selection,
+        op_selection=target_data.op_selection,
         root_run_id=None,
         parent_run_id=None,
         tags=tags,
         job_snapshot=external_job.job_snapshot,
         execution_plan_snapshot=execution_plan_snapshot,
         parent_job_snapshot=external_job.parent_job_snapshot,
         external_job_origin=external_job.get_external_origin(),
```

### Comparing `dagster-1.3.4/dagster/_daemon/types.py` & `dagster-1.3.5/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_daemon/workspace.py` & `dagster-1.3.5/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_generate/download.py` & `dagster-1.3.5/dagster/_generate/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "tutorial_notebook_assets",
     "deploy_docker",
     "deploy_ecs",
     "deploy_k8s",
     "development_to_production",
     "feature_graph_backed_assets",
     "project_fully_featured",
-    "project_pypi_github",
+    "project_analytics",
     "with_airflow",
     "with_great_expectations",
     "with_pyspark",
     "with_pyspark_emr",
     "with_wandb",
 ]
```

### Comparing `dagster-1.3.4/dagster/_generate/generate.py` & `dagster-1.3.5/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.5/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.5/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/__init__.py` & `dagster-1.3.5/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/client.py` & `dagster-1.3.5/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/compile.py` & `dagster-1.3.5/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/impl.py` & `dagster-1.3.5/dagster/_grpc/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Workhorse functions for individual API requests."""
 
 import os
 import sys
 from contextlib import contextmanager
-from typing import Any, Generator, Iterator, Optional, Sequence, Tuple, Union
+from typing import AbstractSet, Any, Generator, Iterator, Optional, Sequence, Tuple, Union
 
 import pendulum
 
 import dagster._check as check
 from dagster._core.definitions import ScheduleEvaluationContext
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.job_definition import JobDefinition
@@ -258,22 +258,22 @@
             run_event_handler=lambda x: None,
         )
 
 
 def get_external_pipeline_subset_result(
     repo_def: RepositoryDefinition,
     job_name: str,
-    solid_selection: Optional[Sequence[str]],
-    asset_selection: Optional[Sequence[AssetKey]],
+    op_selection: Optional[Sequence[str]],
+    asset_selection: Optional[AbstractSet[AssetKey]],
 ):
     try:
         definition = repo_def.get_maybe_subset_job_def(
             job_name,
-            op_selection=solid_selection,
-            asset_selection=frozenset(asset_selection) if asset_selection else None,
+            op_selection=op_selection,
+            asset_selection=asset_selection,
         )
         external_job_data = external_job_data_from_def(definition)
         return ExternalJobSubsetResult(success=True, external_job_data=external_job_data)
     except Exception:
         return ExternalJobSubsetResult(
             success=False, error=serializable_error_info_from_exc_info(sys.exc_info())
         )
@@ -487,15 +487,15 @@
     repo_def: RepositoryDefinition,
     job_name: str,
     args: ExecutionPlanSnapshotArgs,
 ):
     try:
         job_def = repo_def.get_maybe_subset_job_def(
             job_name,
-            op_selection=args.solid_selection,
+            op_selection=args.op_selection,
             asset_selection=args.asset_selection,
         )
 
         return snapshot_from_execution_plan(
             create_execution_plan(
                 job_def,
                 run_config=args.run_config,
```

### Comparing `dagster-1.3.4/dagster/_grpc/protos/api.proto` & `dagster-1.3.5/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/server.py` & `dagster-1.3.5/dagster/_grpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import uuid
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 from multiprocessing.synchronize import Event as MPEvent
 from subprocess import Popen
 from threading import Event as ThreadingEventType
 from time import sleep
-from typing import Any, Dict, Iterator, List, Mapping, NamedTuple, Optional, Sequence, Tuple, cast
+from typing import Any, Dict, Iterator, List, Mapping, Optional, Sequence, Tuple, cast
 
 import grpc
 from grpc_health.v1 import health, health_pb2, health_pb2_grpc
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._core.code_pointer import CodePointer
@@ -36,22 +36,22 @@
 )
 from dagster._core.host_representation.origin import ExternalRepositoryOrigin
 from dagster._core.instance import DagsterInstance, InstanceRef
 from dagster._core.libraries import DagsterLibraryRegistry
 from dagster._core.origin import DEFAULT_DAGSTER_ENTRY_POINT, get_python_environment_entry_point
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
 from dagster._core.workspace.autodiscovery import LoadableTarget
-from dagster._serdes import deserialize_value, serialize_value, whitelist_for_serdes
-from dagster._serdes.ipc import IPCErrorMessage, ipc_write_stream, open_ipc_subprocess
+from dagster._serdes import deserialize_value, serialize_value
+from dagster._serdes.ipc import IPCErrorMessage, open_ipc_subprocess
 from dagster._utils import (
     find_free_port,
     get_run_crash_explanation,
     safe_tempfile_path_unmanaged,
 )
-from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
+from dagster._utils.error import serializable_error_info_from_exc_info
 
 from .__generated__ import api_pb2
 from .__generated__.api_pb2_grpc import DagsterApiServicer, add_DagsterApiServicer_to_server
 from .impl import (
     RunInSubprocessComplete,
     StartRunInSubprocessSuccessful,
     get_external_execution_plan_snapshot,
@@ -546,15 +546,15 @@
             )
             serialized_external_pipeline_subset_result = serialize_value(
                 get_external_pipeline_subset_result(
                     self._get_repo_for_origin(
                         job_subset_snapshot_args.job_origin.external_repository_origin
                     ),
                     job_subset_snapshot_args.job_origin.job_name,
-                    job_subset_snapshot_args.solid_selection,
+                    job_subset_snapshot_args.op_selection,
                     job_subset_snapshot_args.asset_selection,
                 )
             )
         except Exception:
             serialized_external_pipeline_subset_result = serialize_value(
                 ExternalJobSubsetResult(
                     success=False, error=serializable_error_info_from_exc_info(sys.exc_info())
@@ -888,159 +888,76 @@
                     GetCurrentRunsResult(
                         current_runs=list(self._executions.keys()), serializable_error_info=None
                     )
                 )
             )
 
 
-@whitelist_for_serdes
-class GrpcServerStartedEvent(NamedTuple("_GrpcServerStartedEvent", [])):
-    pass
-
-
-@whitelist_for_serdes
-class GrpcServerFailedToBindEvent(NamedTuple("_GrpcServerFailedToBindEvent", [])):
-    pass
-
-
-@whitelist_for_serdes
-class GrpcServerLoadErrorEvent(
-    NamedTuple("GrpcServerLoadErrorEvent", [("error_info", SerializableErrorInfo)])
-):
-    def __new__(cls, error_info: SerializableErrorInfo):
-        return super(GrpcServerLoadErrorEvent, cls).__new__(
-            cls,
-            check.inst_param(error_info, "error_info", SerializableErrorInfo),
-        )
-
-
 def server_termination_target(termination_event, server):
     termination_event.wait()
     # We could make this grace period configurable if we set it in the ShutdownServer handler
     server.stop(grace=5)
 
 
 class DagsterGrpcServer:
     def __init__(
         self,
+        server_termination_event: threading.Event,
+        dagster_api_servicer: DagsterApiServicer,
         host="localhost",
-        port=None,
-        socket=None,
-        max_workers=None,
-        loadable_target_origin=None,
-        heartbeat=False,
-        heartbeat_timeout=30,
-        lazy_load_user_code=False,
-        ipc_output_file=None,
-        fixed_server_id=None,
-        entry_point=None,
-        container_image=None,
-        container_context=None,
-        inject_env_vars_from_instance=False,
-        instance_ref=None,
-        location_name=None,
+        port: Optional[int] = None,
+        socket: Optional[str] = None,
+        max_workers: Optional[int] = None,
     ):
-        check.opt_str_param(host, "host")
-        check.opt_int_param(port, "port")
-        check.opt_str_param(socket, "socket")
-        check.opt_int_param(max_workers, "max_workers")
-        check.opt_inst_param(loadable_target_origin, "loadable_target_origin", LoadableTargetOrigin)
         check.invariant(
             port is not None if seven.IS_WINDOWS else True,
             "You must pass a valid `port` on Windows: `socket` not supported.",
         )
         check.invariant(
             (port or socket) and not (port and socket),
             "You must pass one and only one of `port` or `socket`.",
         )
         check.invariant(
             host is not None if port else True,
             "Must provide a host when serving on a port",
         )
-        check.bool_param(heartbeat, "heartbeat")
-        check.int_param(heartbeat_timeout, "heartbeat_timeout")
-        self._ipc_output_file = check.opt_str_param(ipc_output_file, "ipc_output_file")
-        check.opt_str_param(fixed_server_id, "fixed_server_id")
-
-        check.invariant(heartbeat_timeout > 0, "heartbeat_timeout must be greater than 0")
-        check.invariant(
-            max_workers is None or max_workers > 1 if heartbeat else True,
-            (
-                "max_workers must be greater than 1 or set to None if heartbeat is True. "
-                "If set to None, the server will use the gRPC default."
-            ),
-        )
-
-        check.opt_bool_param(inject_env_vars_from_instance, "inject_env_vars_from_instance")
-        check.opt_inst_param(instance_ref, "instance_ref", InstanceRef)
-        check.opt_str_param(location_name, "location_name")
 
         self.server = grpc.server(
             ThreadPoolExecutor(
                 max_workers=max_workers,
                 thread_name_prefix="grpc-server-rpc-handler",
             ),
             compression=grpc.Compression.Gzip,
             options=[
                 ("grpc.max_send_message_length", max_send_bytes()),
                 ("grpc.max_receive_message_length", max_rx_bytes()),
             ],
         )
-        self._server_termination_event = threading.Event()
-
-        try:
-            self._api_servicer = DagsterApiServer(
-                server_termination_event=self._server_termination_event,
-                loadable_target_origin=loadable_target_origin,
-                heartbeat=heartbeat,
-                heartbeat_timeout=heartbeat_timeout,
-                lazy_load_user_code=lazy_load_user_code,
-                fixed_server_id=fixed_server_id,
-                entry_point=entry_point,
-                container_image=container_image,
-                container_context=container_context,
-                inject_env_vars_from_instance=inject_env_vars_from_instance,
-                instance_ref=instance_ref,
-                location_name=location_name,
-            )
-        except Exception:
-            if self._ipc_output_file:
-                with ipc_write_stream(self._ipc_output_file) as ipc_stream:
-                    ipc_stream.send(
-                        GrpcServerLoadErrorEvent(
-                            error_info=serializable_error_info_from_exc_info(sys.exc_info())
-                        )
-                    )
-            raise
+        self._server_termination_event = server_termination_event
+        self._api_servicer = dagster_api_servicer
 
         # Create a health check servicer
         self._health_servicer = health.HealthServicer()
         health_pb2_grpc.add_HealthServicer_to_server(self._health_servicer, self.server)
 
         add_DagsterApiServicer_to_server(self._api_servicer, self.server)
 
         if port:
             server_address = host + ":" + str(port)
         else:
-            server_address = "unix:" + os.path.abspath(socket)
+            server_address = "unix:" + os.path.abspath(check.not_none(socket))
 
         # grpc.Server.add_insecure_port returns:
         # - 0 on failure
         # - port number when a port is successfully bound
         # - 1 when a UDS is successfully bound
         res = self.server.add_insecure_port(server_address)
         if socket and res != 1:
-            if self._ipc_output_file:
-                with ipc_write_stream(self._ipc_output_file) as ipc_stream:
-                    ipc_stream.send(GrpcServerFailedToBindEvent())
             raise CouldNotBindGrpcServerToAddress(socket)
         if port and res != port:
-            if self._ipc_output_file:
-                with ipc_write_stream(self._ipc_output_file) as ipc_stream:
-                    ipc_stream.send(GrpcServerFailedToBindEvent())
             raise CouldNotBindGrpcServerToAddress(port)
 
     def serve(self):
         # Unfortunately it looks like ports bind late (here) and so this can fail with an error
         # from C++ like:
         #
         #    E0625 08:46:56.180112000 4697443776 server_chttp2.cc:40]
@@ -1064,18 +981,14 @@
 
         self.server.start()
 
         # Note: currently this is hardcoded as serving, since both services are cohosted
 
         self._health_servicer.set("DagsterApi", health_pb2.HealthCheckResponse.SERVING)
 
-        if self._ipc_output_file:
-            with ipc_write_stream(self._ipc_output_file) as ipc_stream:
-                ipc_stream.send(GrpcServerStartedEvent())
-
         server_termination_thread = threading.Thread(
             target=server_termination_target,
             args=[self._server_termination_event, self.server],
             name="grpc-server-termination",
         )
 
         server_termination_thread.daemon = True
```

### Comparing `dagster-1.3.4/dagster/_grpc/server_watcher.py` & `dagster-1.3.5/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_grpc/types.py` & `dagster-1.3.5/dagster/_grpc/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,57 +12,57 @@
     CodeLocationOrigin,
     ExternalJobOrigin,
     ExternalRepositoryOrigin,
 )
 from dagster._core.instance.ref import InstanceRef
 from dagster._core.origin import JobPythonOrigin, get_python_environment_entry_point
 from dagster._serdes import serialize_value, whitelist_for_serdes
+from dagster._serdes.serdes import SetToSequenceFieldSerializer
 from dagster._utils.error import SerializableErrorInfo
 
 
 @whitelist_for_serdes(
     storage_field_names={
         "job_origin": "pipeline_origin",
         "job_snapshot_id": "pipeline_snapshot_id",
+        "op_selection": "solid_selection",
     }
 )
 class ExecutionPlanSnapshotArgs(
     NamedTuple(
         "_ExecutionPlanSnapshotArgs",
         [
             ("job_origin", ExternalJobOrigin),
-            ("solid_selection", Sequence[str]),
+            ("op_selection", Sequence[str]),
             ("run_config", Mapping[str, object]),
             ("step_keys_to_execute", Optional[Sequence[str]]),
             ("job_snapshot_id", str),
             ("known_state", Optional[KnownExecutionState]),
             ("instance_ref", Optional[InstanceRef]),
             ("asset_selection", Optional[AbstractSet[AssetKey]]),
             ("mode", str),
         ],
     )
 ):
     def __new__(
         cls,
         job_origin: ExternalJobOrigin,
-        solid_selection: Sequence[str],
+        op_selection: Sequence[str],
         run_config: Mapping[str, object],
         step_keys_to_execute: Optional[Sequence[str]],
         job_snapshot_id: str,
         known_state: Optional[KnownExecutionState] = None,
         instance_ref: Optional[InstanceRef] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         mode: str = DEFAULT_MODE_NAME,
     ):
         return super(ExecutionPlanSnapshotArgs, cls).__new__(
             cls,
             job_origin=check.inst_param(job_origin, "job_origin", ExternalJobOrigin),
-            solid_selection=check.opt_sequence_param(
-                solid_selection, "solid_selection", of_type=str
-            ),
+            op_selection=check.opt_sequence_param(op_selection, "op_selection", of_type=str),
             run_config=check.mapping_param(run_config, "run_config", key_type=str),
             mode=check.str_param(mode, "mode"),
             step_keys_to_execute=check.opt_nullable_sequence_param(
                 step_keys_to_execute, "step_keys_to_execute", of_type=str
             ),
             job_snapshot_id=check.str_param(job_snapshot_id, "job_snapshot_id"),
             known_state=check.opt_inst_param(known_state, "known_state", KnownExecutionState),
@@ -464,41 +464,42 @@
         )
 
 
 @whitelist_for_serdes(
     storage_name="PipelineSubsetSnapshotArgs",
     storage_field_names={
         "job_origin": "pipeline_origin",
+        "op_selection": "solid_selection",
     },
+    # asset_selection previously was erroneously represented as a sequence
+    field_serializers={"asset_selection": SetToSequenceFieldSerializer},
 )
 class JobSubsetSnapshotArgs(
     NamedTuple(
         "_JobSubsetSnapshotArgs",
         [
             ("job_origin", ExternalJobOrigin),
-            ("solid_selection", Optional[Sequence[str]]),
-            ("asset_selection", Optional[Sequence[AssetKey]]),
+            ("op_selection", Optional[Sequence[str]]),
+            ("asset_selection", Optional[AbstractSet[AssetKey]]),
         ],
     )
 ):
     def __new__(
         cls,
         job_origin: ExternalJobOrigin,
-        solid_selection: Sequence[str],
-        asset_selection: Optional[Sequence[AssetKey]] = None,
+        op_selection: Optional[Sequence[str]],
+        asset_selection: Optional[AbstractSet[AssetKey]] = None,
     ):
         return super(JobSubsetSnapshotArgs, cls).__new__(
             cls,
             job_origin=check.inst_param(job_origin, "job_origin", ExternalJobOrigin),
-            solid_selection=check.sequence_param(solid_selection, "solid_selection", of_type=str)
-            if solid_selection
-            else None,
-            asset_selection=check.opt_sequence_param(
-                asset_selection, "asset_selection", of_type=AssetKey
+            op_selection=check.opt_nullable_sequence_param(
+                op_selection, "op_selection", of_type=str
             ),
+            asset_selection=check.opt_nullable_set_param(asset_selection, "asset_selection"),
         )
 
 
 # Different storage field name for backcompat
 @whitelist_for_serdes(storage_field_names={"code_location_origin": "repository_location_origin"})
 class NotebookPathArgs(
     NamedTuple(
```

### Comparing `dagster-1.3.4/dagster/_grpc/utils.py` & `dagster-1.3.5/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_loggers/__init__.py` & `dagster-1.3.5/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_module_alias_map.py` & `dagster-1.3.5/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_scheduler/scheduler.py` & `dagster-1.3.5/dagster/_scheduler/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
         else:
             run_request = raw_run_request
 
         job_subset_selector = JobSubsetSelector(
             location_name=schedule_origin.external_repository_origin.code_location_origin.location_name,
             repository_name=schedule_origin.external_repository_origin.repository_name,
             job_name=external_schedule.job_name,
-            solid_selection=external_schedule.solid_selection,
+            op_selection=external_schedule.op_selection,
             asset_selection=run_request.asset_selection,
         )
         external_job = code_location.get_external_job(job_subset_selector)
 
         run = _get_existing_run_for_request(instance, external_schedule, schedule_time, run_request)
         if run:
             if run.status != DagsterRunStatus.NOT_STARTED:
@@ -762,17 +762,17 @@
         },
     )
 
     return instance.create_run(
         job_name=external_schedule.job_name,
         run_id=None,
         run_config=run_config,
-        solids_to_execute=external_job.solids_to_execute,
+        resolved_op_selection=external_job.resolved_op_selection,
         step_keys_to_execute=None,
-        solid_selection=external_job.solid_selection,
+        op_selection=external_job.op_selection,
         status=DagsterRunStatus.NOT_STARTED,
         root_run_id=None,
         parent_run_id=None,
         tags=tags,
         job_snapshot=external_job.job_snapshot,
         execution_plan_snapshot=execution_plan_snapshot,
         parent_job_snapshot=external_job.parent_job_snapshot,
```

### Comparing `dagster-1.3.4/dagster/_scheduler/stale.py` & `dagster-1.3.5/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_serdes/__init__.py` & `dagster-1.3.5/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_serdes/config_class.py` & `dagster-1.3.5/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_serdes/ipc.py` & `dagster-1.3.5/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_serdes/serdes.py` & `dagster-1.3.5/dagster/_serdes/serdes.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,14 +572,30 @@
         __unpacked_value: Any,
         whitelist_map: WhitelistMap,
         descent_path: str,
     ) -> JsonSerializableValue:
         ...
 
 
+class SetToSequenceFieldSerializer(FieldSerializer):
+    def unpack(
+        self, sequence_value: Optional[Sequence[Any]], **_kwargs
+    ) -> Optional[AbstractSet[Any]]:
+        return set(sequence_value) if sequence_value is not None else None
+
+    def pack(
+        self, set_value: Optional[AbstractSet[Any]], whitelist_map: WhitelistMap, descent_path: str
+    ) -> Optional[Sequence[Any]]:
+        return (
+            sorted([pack_value(x, whitelist_map, descent_path) for x in set_value], key=str)
+            if set_value is not None
+            else None
+        )
+
+
 ###################################################################################################
 # Serialize / Pack
 ###################################################################################################
 
 
 def serialize_value(
     val: PackableValue,
```

### Comparing `dagster-1.3.4/dagster/_serdes/utils.py` & `dagster-1.3.5/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_seven/__init__.py` & `dagster-1.3.5/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_seven/abc.py` & `dagster-1.3.5/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_seven/compat/pendulum.py` & `dagster-1.3.5/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/__init__.py` & `dagster-1.3.5/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/alert.py` & `dagster-1.3.5/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/backcompat.py` & `dagster-1.3.5/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/backoff.py` & `dagster-1.3.5/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/cached_method.py` & `dagster-1.3.5/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.5/dagster/_utils/caching_instance_queryer.py`

 * *Files 5% similar despite different names*

```diff
@@ -334,45 +334,50 @@
             record_version = extract_data_version_from_entry(record.event_log_entry)
             if record_version is not None and record_version != data_version:
                 return record
 
         # no records found with a new data version
         return None
 
-    def new_version_exists(
+    def new_version_storage_id(
         self,
         observable_source_asset_key: AssetKey,
         after_cursor: Optional[int] = None,
-    ) -> bool:
-        """Returns True if there is an asset observation of the given observable source asset key
-        after the specified cursor.
+    ) -> Optional[int]:
+        """Returns the storage id of the latest asset observation of the given observable source
+        asset key after the specified cursor, or None if no such observation exists.
 
         Args:
             observable_source_asset_key (AssetKeyPartitionKey): The observable source asset to query.
             after_cursor (Optional[int]): Filter parameter such that only records with a storage_id
                 greater than this value will be considered.
         """
-        previous_version_record = self.get_observation_record(
-            asset_key=observable_source_asset_key,
-            # we're looking for if a new version exists after `after_cursor`, so we need to know
-            # what the version was before `after_cursor`
-            before_cursor=after_cursor,
+        previous_version_record = (
+            self.get_observation_record(
+                asset_key=observable_source_asset_key,
+                # we're looking for if a new version exists after `after_cursor`, so we need to know
+                # what the version was before `after_cursor`
+                before_cursor=after_cursor,
+            )
+            # if the after_cursor is None, then no previous version can exist
+            if after_cursor is not None
+            else None
         )
         previous_version = (
             extract_data_version_from_entry(previous_version_record.event_log_entry)
             if previous_version_record is not None
             else None
         )
 
         next_version_record = self.next_version_record(
             asset_key=observable_source_asset_key,
             after_cursor=after_cursor,
             data_version=previous_version,
         )
-        return next_version_record is not None
+        return next_version_record.storage_id if next_version_record else None
 
     def _new_version_of_source_exists_after_asset_partition(
         self,
         observable_source_asset_key: AssetKey,
         asset_partition: AssetKeyPartitionKey,
     ) -> bool:
         """Returns True if there is a new version of a given observable source asset after the latest
```

### Comparing `dagster-1.3.4/dagster/_utils/dagster_type.py` & `dagster-1.3.5/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/error.py` & `dagster-1.3.5/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/external.py` & `dagster-1.3.5/dagster/_utils/external.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dagster._core.host_representation.external import ExternalJob
 from dagster._core.host_representation.origin import ExternalJobOrigin
 
 
 def external_job_from_location(
     code_location: CodeLocation,
     external_job_origin: ExternalJobOrigin,
-    solid_selection: Optional[Sequence[str]],
+    op_selection: Optional[Sequence[str]],
 ) -> ExternalJob:
     check.inst_param(code_location, "code_location", CodeLocation)
     check.inst_param(external_job_origin, "external_pipeline_origin", ExternalJobOrigin)
 
     repo_name = external_job_origin.external_repository_origin.repository_name
     job_name = external_job_origin.job_name
 
@@ -24,11 +24,11 @@
     )
     external_repo = code_location.get_repository(repo_name)
 
     pipeline_selector = JobSubsetSelector(
         location_name=code_location.name,
         repository_name=external_repo.name,
         job_name=job_name,
-        solid_selection=solid_selection,
+        op_selection=op_selection,
     )
 
     return code_location.get_external_job(pipeline_selector)
```

### Comparing `dagster-1.3.4/dagster/_utils/forked_pdb.py` & `dagster-1.3.5/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/hosted_user_process.py` & `dagster-1.3.5/dagster/_utils/hosted_user_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,18 @@
 
 def external_repo_from_def(
     repository_def: "RepositoryDefinition", repository_handle: "RepositoryHandle"
 ) -> ExternalRepository:
     return ExternalRepository(external_repository_data_from_def(repository_def), repository_handle)
 
 
-def external_job_from_recon_job(
-    recon_job, solid_selection, repository_handle, asset_selection=None
-):
-    if solid_selection or asset_selection:
-        sub_recon_job = recon_job.subset_for_execution(
-            solid_selection=solid_selection, asset_selection=asset_selection
+def external_job_from_recon_job(recon_job, op_selection, repository_handle, asset_selection=None):
+    if op_selection or asset_selection:
+        sub_recon_job = recon_job.get_subset(
+            op_selection=op_selection, asset_selection=asset_selection
         )
         job_def = sub_recon_job.get_definition()
     else:
         job_def = recon_job.get_definition()
 
     return ExternalJob(
         external_job_data_from_def(job_def),
```

### Comparing `dagster-1.3.4/dagster/_utils/indenting_printer.py` & `dagster-1.3.5/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/interrupts.py` & `dagster-1.3.5/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/log.py` & `dagster-1.3.5/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/merger.py` & `dagster-1.3.5/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/net.py` & `dagster-1.3.5/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/schedules.py` & `dagster-1.3.5/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/tags.py` & `dagster-1.3.5/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/temp_file.py` & `dagster-1.3.5/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/test/__init__.py` & `dagster-1.3.5/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.5/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.5/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.5/dagster/_utils/test/schedule_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import sys
 import time
 
 import pendulum
 import pytest
 
+from dagster._core.definitions.asset_reconciliation_sensor import (
+    AutoMaterializeAssetEvaluation,
+)
+from dagster._core.definitions.auto_materialize_condition import MissingAutoMaterializeCondition
+from dagster._core.definitions.events import AssetKey
 from dagster._core.host_representation import (
     ExternalRepositoryOrigin,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
 from dagster._core.scheduler.instigation import (
     InstigatorState,
     InstigatorStatus,
@@ -48,14 +53,17 @@
     # Override this for schedule storages that are not allowed to delete state or ticks
     def can_delete(self):
         return True
 
     def can_purge(self):
         return True
 
+    def can_store_auto_materialize_asset_evaluations(self):
+        return True
+
     @staticmethod
     def fake_repo_target():
         return ExternalRepositoryOrigin(
             ManagedGrpcPythonEnvCodeLocationOrigin(
                 LoadableTargetOrigin(
                     executable_path=sys.executable, module_name="fake", attribute="fake"
                 ),
@@ -665,7 +673,79 @@
         )
 
         ticks_by_origin = storage.get_batch_ticks(["sensor_one", "sensor_two"], limit=1)
         assert set(ticks_by_origin.keys()) == {"sensor_one", "sensor_two"}
         assert len(ticks_by_origin["sensor_one"]) == 1
         assert ticks_by_origin["sensor_one"][0].tick_id == b.tick_id
         assert ticks_by_origin["sensor_two"][0].tick_id == d.tick_id
+
+    def test_auto_materialize_asset_evaluations(self, storage):
+        if not self.can_store_auto_materialize_asset_evaluations():
+            pytest.skip("Storage cannot store auto materialize asset evaluations")
+
+        storage.add_auto_materialize_asset_evaluations(
+            evaluation_id=10,
+            asset_evaluations=[
+                AutoMaterializeAssetEvaluation(
+                    asset_key=AssetKey("asset_one"),
+                    conditions=[],
+                    num_requested=0,
+                    num_skipped=0,
+                    num_discarded=0,
+                ),
+                AutoMaterializeAssetEvaluation(
+                    asset_key=AssetKey("asset_two"),
+                    conditions=[MissingAutoMaterializeCondition()],
+                    num_requested=1,
+                    num_skipped=0,
+                    num_discarded=0,
+                ),
+            ],
+        )
+
+        res = storage.get_auto_materialize_asset_evaluations(
+            asset_key=AssetKey("asset_one"), limit=100
+        )
+        assert len(res) == 1
+        assert res[0].evaluation.asset_key == AssetKey("asset_one")
+        assert res[0].evaluation_id == 10
+        assert res[0].evaluation.num_requested == 0
+
+        res = storage.get_auto_materialize_asset_evaluations(
+            asset_key=AssetKey("asset_two"), limit=100
+        )
+        assert len(res) == 1
+        assert res[0].evaluation.asset_key == AssetKey("asset_two")
+        assert res[0].evaluation_id == 10
+        assert res[0].evaluation.num_requested == 1
+
+        storage.add_auto_materialize_asset_evaluations(
+            evaluation_id=11,
+            asset_evaluations=[
+                AutoMaterializeAssetEvaluation(
+                    asset_key=AssetKey("asset_one"),
+                    conditions=[],
+                    num_requested=0,
+                    num_skipped=0,
+                    num_discarded=0,
+                ),
+            ],
+        )
+
+        res = storage.get_auto_materialize_asset_evaluations(
+            asset_key=AssetKey("asset_one"), limit=100
+        )
+        assert len(res) == 2
+        assert res[0].evaluation_id == 11
+        assert res[1].evaluation_id == 10
+
+        res = storage.get_auto_materialize_asset_evaluations(
+            asset_key=AssetKey("asset_one"), limit=1
+        )
+        assert len(res) == 1
+        assert res[0].evaluation_id == 11
+
+        res = storage.get_auto_materialize_asset_evaluations(
+            asset_key=AssetKey("asset_one"), limit=1, cursor=11
+        )
+        assert len(res) == 1
+        assert res[0].evaluation_id == 10
```

### Comparing `dagster-1.3.4/dagster/_utils/timing.py` & `dagster-1.3.5/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/typing_api.py` & `dagster-1.3.5/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster/_utils/yaml_utils.py` & `dagster-1.3.5/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.4/dagster.egg-info/PKG-INFO` & `dagster-1.3.5/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.4
+Version: 1.3.5
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.4/dagster.egg-info/SOURCES.txt` & `dagster-1.3.5/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 dagster/_core/definitions/asset_layer.py
 dagster/_core/definitions/asset_out.py
 dagster/_core/definitions/asset_reconciliation_sensor.py
 dagster/_core/definitions/asset_selection.py
 dagster/_core/definitions/asset_sensor_definition.py
 dagster/_core/definitions/assets.py
 dagster/_core/definitions/assets_job.py
+dagster/_core/definitions/auto_materialize_condition.py
 dagster/_core/definitions/auto_materialize_policy.py
 dagster/_core/definitions/cacheable_assets.py
 dagster/_core/definitions/composition.py
 dagster/_core/definitions/config.py
 dagster/_core/definitions/configurable.py
 dagster/_core/definitions/data_time.py
 dagster/_core/definitions/data_version.py
@@ -387,14 +388,15 @@
 dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
 dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
 dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
 dagster/_core/storage/alembic/versions/035_add_run_job_index.py
 dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
 dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
 dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
 dagster/_core/storage/alembic/versions/__init__.py
 dagster/_core/storage/branching/__init__.py
 dagster/_core/storage/branching/branching_io_manager.py
 dagster/_core/storage/event_log/__init__.py
 dagster/_core/storage/event_log/base.py
 dagster/_core/storage/event_log/in_memory.py
 dagster/_core/storage/event_log/migration.py
```

### Comparing `dagster-1.3.4/dagster.egg-info/requires.txt` & `dagster-1.3.5/dagster.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 click>=5.0
 coloredlogs<=14.0,>=6.1
 Jinja2
 PyYAML>=5.1
-alembic!=1.6.3,!=1.7.0,>=1.2.1
+alembic!=1.6.3,!=1.7.0,<1.11.0,>=1.2.1
 croniter>=0.3.34
 grpcio-health-checking>=1.44.0
 packaging>=20.9
 pendulum
 protobuf>=3.20.0
 python-dateutil
 python-dotenv
```

### Comparing `dagster-1.3.4/setup.py` & `dagster-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         "click>=5.0",
         "coloredlogs>=6.1, <=14.0",
         "contextvars; python_version < '3.7'",
         "Jinja2",
         "PyYAML>=5.1",
         # core (not explicitly expressed atm)
         # pin around issues in specific versions of alembic that broke our migrations
-        "alembic>=1.2.1,!=1.6.3,!=1.7.0",
+        "alembic>=1.2.1,!=1.6.3,!=1.7.0,<1.11.0",
         "croniter>=0.3.34",
         # grpcio 1.44.0 is the min version compatible with both protobuf 3 and 4
         # Also pinned <1.48.0 until the resolution of https://github.com/grpc/grpc/issues/31885
         # (except on python 3.11, where newer versions are required just to install the grpcio package)
         "grpcio>=1.44.0,<1.48.0; python_version<'3.11'",
         "grpcio>=1.44.0; python_version>='3.11'",
         "grpcio-health-checking>=1.44.0",
```

