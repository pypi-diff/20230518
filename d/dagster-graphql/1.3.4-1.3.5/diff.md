# Comparing `tmp/dagster-graphql-1.3.4.tar.gz` & `tmp/dagster-graphql-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.4.tar", last modified: Thu May 11 17:05:47 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.5.tar", last modified: Thu May 18 20:45:04 2023, max compression
```

## Comparing `dagster-graphql-1.3.4.tar` & `dagster-graphql-1.3.5.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.131948 dagster-graphql-1.3.4/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.135948 dagster-graphql-1.3.4/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21544 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.151948 dagster-graphql-1.3.4/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.155948 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11506 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8930 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4404 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12609 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15110 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10796 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8081 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.187948 dagster-graphql-1.3.4/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40498 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16767 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.191948 dagster-graphql-1.3.4/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17489 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.199948 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11062 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39461 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25580 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    36191 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8309 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7986 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.207948 dagster-graphql-1.3.4/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6376 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:05:47.131948 dagster-graphql-1.3.4/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4150 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-11 17:05:47.000000 dagster-graphql-1.3.4/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-11 17:05:47.211948 dagster-graphql-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-11 16:58:41.000000 dagster-graphql-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.009603 dagster-graphql-1.3.5/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.013603 dagster-graphql-1.3.5/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17835 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.029603 dagster-graphql-1.3.5/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.033603 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11457 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8885 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25629 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12470 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.065603 dagster-graphql-1.3.5/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40498 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16767 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.069603 dagster-graphql-1.3.5/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.117603 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39385 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.125603 dagster-graphql-1.3.5/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25294 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    36755 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.009603 dagster-graphql-1.3.5/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-18 20:45:04.133603 dagster-graphql-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/setup.py
```

### Comparing `dagster-graphql-1.3.4/LICENSE` & `dagster-graphql-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/PKG-INFO` & `dagster-graphql-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.4
+Version: 1.3.5
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/cli.py` & `dagster-graphql-1.3.5/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/client/client.py` & `dagster-graphql-1.3.5/dagster_graphql/client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         pipeline_name: str,
         repository_location_name: Optional[str] = None,
         repository_name: Optional[str] = None,
         run_config: Optional[Mapping[str, Any]] = None,
         mode: str = "default",
         preset: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
-        solid_selection: Optional[Sequence[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
         is_using_job_op_graph_apis: Optional[bool] = False,
     ):
         check.opt_str_param(repository_location_name, "repository_location_name")
         check.opt_str_param(repository_name, "repository_name")
         check.str_param(pipeline_name, "pipeline_name")
         check.opt_str_param(mode, "mode")
         check.opt_str_param(preset, "preset")
@@ -166,15 +166,15 @@
 
         variables: Dict[str, Any] = {
             "executionParams": {
                 "selector": {
                     "repositoryLocationName": repository_location_name,
                     "repositoryName": repository_name,
                     "pipelineName": pipeline_name,
-                    "solidSelection": solid_selection,
+                    "solidSelection": op_selection,
                 }
             }
         }
         if preset is not None:
             variables["executionParams"]["preset"] = preset
         if mode is not None and run_config is not None:
             variables["executionParams"] = {
@@ -208,84 +208,23 @@
         ):
             raise DagsterGraphQLClientError(query_result_type, query_result["errors"])
         else:
             # query_result_type is a ConflictingExecutionParamsError, a PresetNotFoundError
             # a PipelineNotFoundError, a RunConflict, or a PythonError
             raise DagsterGraphQLClientError(query_result_type, query_result["message"])
 
-    def submit_pipeline_execution(
-        self,
-        pipeline_name: str,
-        repository_location_name: Optional[str] = None,
-        repository_name: Optional[str] = None,
-        run_config: Optional[Any] = None,
-        mode: str = "default",
-        preset: Optional[str] = None,
-        tags: Optional[Dict[str, Any]] = None,
-        solid_selection: Optional[Sequence[str]] = None,
-    ) -> str:
-        """Submits a Pipeline with attached configuration for execution.
-
-        Args:
-            pipeline_name (str): The pipeline's name
-            repository_location_name (Optional[str], optional): The name of the repository location where
-                the pipeline is located. If omitted, the client will try to infer the repository location
-                from the available options on the Dagster deployment. Defaults to None.
-            repository_name (Optional[str], optional): The name of the repository where the pipeline is located.
-                If omitted, the client will try to infer the repository from the available options
-                on the Dagster deployment. Defaults to None.
-            run_config (Optional[Any], optional): This is the run config to execute the pipeline with.
-                Note that runConfigData is any-typed in the GraphQL type system. This type is used when passing in
-                an arbitrary object for run config. However, it must conform to the constraints of the config
-                schema for this pipeline. If it does not, the client will throw a DagsterGraphQLClientError with a message of
-                RunConfigValidationInvalid. Defaults to None.
-            mode (Optional[str], optional): The mode to run the pipeline with. If you have not
-                defined any custom modes for your pipeline, the default mode is "default". Defaults to None.
-            preset (Optional[str], optional): The name of a pre-defined preset to use instead of a
-                run config. Defaults to None.
-            tags (Optional[Dict[str, Any]], optional): A set of tags to add to the pipeline execution.
-
-        Raises:
-            DagsterGraphQLClientError("InvalidStepError", invalid_step_key): the pipeline has an invalid step
-            DagsterGraphQLClientError("InvalidOutputError", body=error_object): some solid has an invalid output within the pipeline.
-                The error_object is of type dagster_graphql.InvalidOutputErrorInfo.
-            DagsterGraphQLClientError("ConflictingExecutionParamsError", invalid_step_key): a preset and a run_config & mode are present
-                that conflict with one another
-            DagsterGraphQLClientError("PresetNotFoundError", message): if the provided preset name is not found
-            DagsterGraphQLClientError("RunConflict", message): a `DagsterRunConflict` occured during execution.
-                This indicates that a conflicting pipeline run already exists in run storage.
-            DagsterGraphQLClientError("PipelineConfigurationInvalid", invalid_step_key): the run_config is not in the expected format
-                for the pipeline
-            DagsterGraphQLClientError("PipelineNotFoundError", message): the requested pipeline does not exist
-            DagsterGraphQLClientError("PythonError", message): an internal framework error occurred
-
-        Returns:
-            str: run id of the submitted pipeline run
-        """
-        return self._core_submit_execution(
-            pipeline_name,
-            repository_location_name,
-            repository_name,
-            run_config,
-            mode,
-            preset,
-            tags,
-            solid_selection,
-            is_using_job_op_graph_apis=False,
-        )
-
     @public
     def submit_job_execution(
         self,
         job_name: str,
         repository_location_name: Optional[str] = None,
         repository_name: Optional[str] = None,
         run_config: Optional[Dict[str, Any]] = None,
         tags: Optional[Dict[str, Any]] = None,
-        op_selection: Optional[List[str]] = None,
+        op_selection: Optional[Sequence[str]] = None,
     ) -> str:
         """Submits a job with attached configuration for execution.
 
         Args:
             job_name (str): The job's name
             repository_location_name (Optional[str]): The name of the repository location where
                 the job is located. If omitted, the client will try to infer the repository location
@@ -318,15 +257,15 @@
             pipeline_name=job_name,
             repository_location_name=repository_location_name,
             repository_name=repository_name,
             run_config=run_config,
             mode="default",
             preset=None,
             tags=tags,
-            solid_selection=op_selection,
+            op_selection=op_selection,
             is_using_job_op_graph_apis=True,
         )
 
     @public
     def get_run_status(self, run_id: str) -> DagsterRunStatus:
         """Get the status of a given Pipeline Run.
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.5/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/client/query.py` & `dagster-graphql-1.3.5/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.5/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.roots.mutation import GrapheneTerminateRunPolicy
 
 from ..utils import (
     assert_permission,
     assert_permission_for_location,
-    capture_error,
 )
 from .backfill import (
     cancel_partition_backfill as cancel_partition_backfill,
     create_and_launch_partition_backfill as create_and_launch_partition_backfill,
     resume_partition_backfill as resume_partition_backfill,
 )
 
@@ -141,15 +140,14 @@
         return GrapheneTerminateRunSuccess(graphene_run)
 
     return GrapheneTerminateRunFailure(
         run=graphene_run, message=f"Unable to terminate run {run.run_id}"
     )
 
 
-@capture_error
 def delete_pipeline_run(
     graphene_info: "ResolveInfo", run_id: str
 ) -> Union["GrapheneDeletePipelineRunSuccess", "GrapheneRunNotFoundError"]:
     from ...schema.errors import GrapheneRunNotFoundError
     from ...schema.roots.mutation import GrapheneDeletePipelineRunSuccess
 
     instance = graphene_info.context.instance
@@ -317,15 +315,14 @@
             update = await queue.get()
             yield from_captured_log_data(update)  # type: ignore
             is_complete = subscription.is_complete
     finally:
         subscription.dispose()
 
 
-@capture_error
 def wipe_assets(
     graphene_info: "ResolveInfo", asset_keys: Sequence[AssetKey]
 ) -> "GrapheneAssetWipeSuccess":
     from ...schema.roots.mutation import GrapheneAssetWipeSuccess
 
     instance = graphene_info.context.instance
     instance.wipe_assets(asset_keys)
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dagster._core.execution.job_backfill import submit_backfill_runs
 from dagster._core.host_representation.external_data import ExternalPartitionExecutionErrorData
 from dagster._core.utils import make_new_backfill_id
 from dagster._core.workspace.permissions import Permissions
 from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
-from ..utils import BackfillParams, assert_permission, assert_permission_for_location, capture_error
+from ..utils import BackfillParams, assert_permission, assert_permission_for_location
 
 BACKFILL_CHUNK_SIZE = 25
 
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.util import ResolveInfo
 
@@ -170,15 +170,14 @@
             "Backfill requested without specifying partition set selector or asset selection"
         )
 
     graphene_info.context.instance.add_backfill(backfill)
     return GrapheneLaunchBackfillSuccess(backfill_id=backfill_id)
 
 
-@capture_error
 def cancel_partition_backfill(
     graphene_info: "ResolveInfo", backfill_id: str
 ) -> "GrapheneCancelBackfillSuccess":
     from ...schema.backfill import GrapheneCancelBackfillSuccess
 
     backfill = graphene_info.context.instance.get_backfill(backfill_id)
     if not backfill:
@@ -190,15 +189,14 @@
         graphene_info, Permissions.CANCEL_PARTITION_BACKFILL, location_name
     )
 
     graphene_info.context.instance.update_backfill(backfill.with_status(BulkActionStatus.CANCELED))
     return GrapheneCancelBackfillSuccess(backfill_id=backfill_id)
 
 
-@capture_error
 def resume_partition_backfill(
     graphene_info: "ResolveInfo", backfill_id: str
 ) -> "GrapheneResumeBackfillSuccess":
     from ...schema.backfill import GrapheneResumeBackfillSuccess
 
     backfill = graphene_info.context.instance.get_backfill(backfill_id)
     if not backfill:
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dagster._core.definitions.selector import (
     RepositorySelector,
 )
 from dagster._core.workspace.permissions import Permissions
 
 from dagster_graphql.schema.errors import GrapheneDuplicateDynamicPartitionError
 
-from ..utils import UserFacingGraphQLError, assert_permission_for_location, capture_error
+from ..utils import UserFacingGraphQLError, assert_permission_for_location
 
 if TYPE_CHECKING:
     from ...schema.inputs import GrapheneRepositorySelector
     from ...schema.partition_sets import GrapheneAddDynamicPartitionSuccess
 
 
 def _repository_contains_dynamic_partitions_def(
@@ -49,15 +49,14 @@
                     _is_matching_partitions_def(partitions_def)
                     for partitions_def in found_partitions_defs
                 ]
             )
     return False
 
 
-@capture_error
 def add_dynamic_partition(
     graphene_info,
     repository_selector: "GrapheneRepositorySelector",
     partitions_def_name: str,
     partition_key: str,
 ) -> "GrapheneAddDynamicPartitionSuccess":
     from dagster_graphql.schema.errors import GrapheneUnauthorizedError
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,28 @@
 from dagster._core.workspace.permissions import Permissions
 
 from ..external import get_external_job_or_raise
 from ..utils import (
     ExecutionMetadata,
     ExecutionParams,
     assert_permission_for_location,
-    capture_error,
 )
 from .run_lifecycle import create_valid_pipeline_run
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.runs import GrapheneLaunchRunSuccess
     from dagster_graphql.schema.util import ResolveInfo
 
 
-@capture_error
 def launch_pipeline_reexecution(
     graphene_info: "ResolveInfo", execution_params: ExecutionParams
 ) -> "GrapheneLaunchRunSuccess":
     return _launch_pipeline_execution(graphene_info, execution_params, is_reexecuted=True)
 
 
-@capture_error
 def launch_pipeline_execution(
     graphene_info: "ResolveInfo", execution_params: ExecutionParams
 ) -> "GrapheneLaunchRunSuccess":
     return _launch_pipeline_execution(graphene_info, execution_params)
 
 
 def do_launch(
@@ -68,15 +65,14 @@
 
     run = do_launch(graphene_info, execution_params, is_reexecuted)
     records = graphene_info.context.instance.get_run_records(RunsFilter(run_ids=[run.run_id]))
 
     return GrapheneLaunchRunSuccess(run=GrapheneRun(records[0]))
 
 
-@capture_error
 def launch_reexecution_from_parent_run(
     graphene_info: "ResolveInfo", parent_run_id: str, strategy: str
 ) -> "GrapheneLaunchRunSuccess":
     """Launch a re-execution by referencing the parent run id."""
     from ...schema.pipelines.pipeline import GrapheneRun
     from ...schema.runs import GrapheneLaunchRunSuccess
 
@@ -87,15 +83,15 @@
         instance.get_run_by_id(parent_run_id), f"Could not find parent run with id: {parent_run_id}"
     )
     origin = check.not_none(parent_run.external_job_origin)
     selector = JobSubsetSelector(
         location_name=origin.external_repository_origin.code_location_origin.location_name,
         repository_name=origin.external_repository_origin.repository_name,
         job_name=parent_run.job_name,
-        solid_selection=None,
+        op_selection=None,
     )
 
     assert_permission_for_location(
         graphene_info,
         Permissions.LAUNCH_PIPELINE_REEXECUTION,
         selector.location_name,
     )
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         job_name=execution_params.selector.job_name,
         run_id=execution_params.execution_metadata.run_id
         if execution_params.execution_metadata.run_id
         else make_new_run_id(),
         asset_selection=frozenset(execution_params.selector.asset_selection)
         if execution_params.selector.asset_selection
         else None,
-        solid_selection=execution_params.selector.solid_selection,
-        solids_to_execute=frozenset(execution_params.selector.solid_selection)
-        if execution_params.selector.solid_selection
+        op_selection=execution_params.selector.op_selection,
+        resolved_op_selection=frozenset(execution_params.selector.op_selection)
+        if execution_params.selector.op_selection
         else None,
         run_config=execution_params.run_config,
         step_keys_to_execute=step_keys_to_execute,
         tags=tags,
         root_run_id=execution_params.execution_metadata.root_run_id,
         parent_run_id=execution_params.execution_metadata.parent_run_id,
         status=DagsterRunStatus.NOT_STARTED,
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dagster._core.definitions.selector import JobSubsetSelector, RepositorySelector
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.host_representation import ExternalJob
 from dagster._core.host_representation.external import ExternalExecutionPlan
 from dagster._core.workspace.context import BaseWorkspaceRequestContext, WorkspaceRequestContext
 from dagster._utils.error import serializable_error_info_from_exc_info
 
-from .utils import UserFacingGraphQLError, capture_error
+from .utils import UserFacingGraphQLError
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.errors import GrapheneRepositoryNotFoundError
     from dagster_graphql.schema.external import (
         GrapheneRepository,
         GrapheneRepositoryConnection,
         GrapheneWorkspace,
@@ -103,15 +103,14 @@
         external_job=external_pipeline,
         run_config=run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
     )
 
 
-@capture_error
 def fetch_repositories(graphene_info: "ResolveInfo") -> GrapheneRepositoryConnection:
     from ..schema.external import GrapheneRepository, GrapheneRepositoryConnection
 
     return GrapheneRepositoryConnection(
         nodes=[
             GrapheneRepository(
                 instance=graphene_info.context.instance,
@@ -120,15 +119,14 @@
             )
             for location in graphene_info.context.code_locations
             for repository in location.get_repositories().values()
         ]
     )
 
 
-@capture_error
 def fetch_repository(
     graphene_info: "ResolveInfo", repository_selector: RepositorySelector
 ) -> Union[GrapheneRepository, GrapheneRepositoryNotFoundError]:
     from ..schema.errors import GrapheneRepositoryNotFoundError
     from ..schema.external import GrapheneRepository
 
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
@@ -143,15 +141,14 @@
             )
 
     return GrapheneRepositoryNotFoundError(
         repository_selector.location_name, repository_selector.repository_name
     )
 
 
-@capture_error
 def fetch_workspace(workspace_request_context: WorkspaceRequestContext) -> GrapheneWorkspace:
     from ..schema.external import GrapheneWorkspace, GrapheneWorkspaceLocationEntry
 
     check.inst_param(
         workspace_request_context, "workspace_request_context", BaseWorkspaceRequestContext
     )
 
@@ -159,15 +156,14 @@
         GrapheneWorkspaceLocationEntry(entry)
         for entry in workspace_request_context.get_workspace_snapshot().values()
     ]
 
     return GrapheneWorkspace(locationEntries=nodes)
 
 
-@capture_error
 def fetch_location_statuses(
     workspace_request_context: WorkspaceRequestContext,
 ) -> GrapheneWorkspaceLocationStatusEntries:
     from ..schema.external import (
         GrapheneRepositoryLocationLoadStatus,
         GrapheneWorkspaceLocationStatusEntries,
         GrapheneWorkspaceLocationStatusEntry,
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,14 @@
 )
 
 from dagster_graphql.implementation.loader import (
     CrossRepoAssetDependedByLoader,
     StaleStatusLoader,
 )
 
-from .utils import capture_error
-
 if TYPE_CHECKING:
     from ..schema.asset_graph import GrapheneAssetNode, GrapheneAssetNodeDefinitionCollision
     from ..schema.errors import GrapheneAssetNotFoundError
     from ..schema.freshness_policy import GrapheneAssetFreshnessInfo
     from ..schema.pipelines.pipeline import (
         GrapheneAsset,
         GrapheneDefaultPartitions,
@@ -86,15 +84,14 @@
 
     try:
         return seven.json.dumps(seven.json.loads(cursor_string))
     except seven.JSONDecodeError:
         return cursor_string
 
 
-@capture_error
 def get_assets(
     graphene_info: "ResolveInfo",
     prefix: Optional[Sequence[str]] = None,
     cursor: Optional[str] = None,
     limit: Optional[int] = None,
 ) -> "GrapheneAssetConnection":
     from ..schema.pipelines.pipeline import GrapheneAsset
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_backfills.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 from typing import TYPE_CHECKING, Optional
 
 from dagster._core.execution.backfill import BulkActionStatus
 
-from .utils import capture_error
-
 if TYPE_CHECKING:
     from dagster_graphql.schema.util import ResolveInfo
 
     from ..schema.backfill import (
         GraphenePartitionBackfill,
         GraphenePartitionBackfills,
     )
 
 
-@capture_error
 def get_backfill(graphene_info: "ResolveInfo", backfill_id: str) -> "GraphenePartitionBackfill":
     from ..schema.backfill import GrapheneBackfillNotFoundError, GraphenePartitionBackfill
 
     backfill_job = graphene_info.context.instance.get_backfill(backfill_id)
     if backfill_job is None:
         return GrapheneBackfillNotFoundError(backfill_id)
 
     return GraphenePartitionBackfill(backfill_job)
 
 
-@capture_error
 def get_backfills(
     graphene_info: "ResolveInfo",
     status: Optional[BulkActionStatus] = None,
     cursor: Optional[str] = None,
     limit: Optional[int] = None,
 ) -> "GraphenePartitionBackfills":
     from ..schema.backfill import GraphenePartitionBackfill, GraphenePartitionBackfills
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 
 from dagster_graphql.schema.env_vars import (
     GrapheneEnvVarWithConsumers,
     GrapheneEnvVarWithConsumersList,
     GrapheneEnvVarWithConsumersListOrError,
 )
 
-from .utils import capture_error
 
-
-@capture_error
 def get_utilized_env_vars_or_error(
     graphene_info, repository_selector
 ) -> GrapheneEnvVarWithConsumersListOrError:
     check.inst_param(graphene_info, "graphene_info", ResolveInfo)
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
 
     location: CodeLocation = graphene_info.context.get_code_location(
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_instigators.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dagster._check as check
 from dagster._core.definitions.instigation_logger import get_instigation_log_records
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.definitions.selector import InstigatorSelector
 from dagster._core.log_manager import DAGSTER_META_KEY
 from dagster._core.scheduler.instigation import InstigatorStatus
 
-from .utils import capture_error
-
 if TYPE_CHECKING:
     from dagster_graphql.schema.util import ResolveInfo
 
     from ..schema.instigation import (
         GrapheneInstigationEventConnection,
         GrapheneInstigationState,
         GrapheneInstigationStateNotFoundError,
         GrapheneInstigationStates,
     )
 
 
-@capture_error
 def get_unloadable_instigator_states_or_error(
     graphene_info: "ResolveInfo", instigator_type: Optional[InstigatorType] = None
 ) -> "GrapheneInstigationStates":
     from ..schema.instigation import GrapheneInstigationState, GrapheneInstigationStates
 
     check.opt_inst_param(instigator_type, "instigator_type", InstigatorType)
     instigator_states = graphene_info.context.instance.all_instigator_state(
@@ -52,15 +49,14 @@
         results=[
             GrapheneInstigationState(instigator_state=instigator_state)
             for instigator_state in unloadable_states
         ]
     )
 
 
-@capture_error
 def get_instigator_state_or_error(
     graphene_info: "ResolveInfo", selector: InstigatorSelector
 ) -> Union["GrapheneInstigationState", "GrapheneInstigationStateNotFoundError"]:
     from ..schema.instigation import GrapheneInstigationState, GrapheneInstigationStateNotFoundError
 
     check.inst_param(selector, "selector", InstigatorSelector)
     location = graphene_info.context.get_code_location(selector.location_name)
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     TagType,
     get_tag_type,
 )
 from dagster._utils.yaml_utils import dump_run_config_yaml
 
 from dagster_graphql.schema.util import ResolveInfo
 
-from .utils import capture_error
-
 if TYPE_CHECKING:
     from dagster_graphql.schema.errors import GraphenePartitionSetNotFoundError
     from dagster_graphql.schema.partition_sets import (
         GraphenePartition,
         GraphenePartitionRun,
         GraphenePartitionRunConfig,
         GraphenePartitions,
@@ -37,15 +35,14 @@
         GraphenePartitionSets,
         GraphenePartitionStatus,
         GraphenePartitionStatusCounts,
         GraphenePartitionTags,
     )
 
 
-@capture_error
 def get_partition_sets_or_error(
     graphene_info: ResolveInfo, repository_selector: RepositorySelector, pipeline_name: str
 ) -> "GraphenePartitionSets":
     from ..schema.partition_sets import GraphenePartitionSet, GraphenePartitionSets
 
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
     check.str_param(pipeline_name, "pipeline_name")
@@ -71,15 +68,14 @@
                     partition_set.name,
                 ),
             )
         ]
     )
 
 
-@capture_error
 def get_partition_set(
     graphene_info: ResolveInfo, repository_selector: RepositorySelector, partition_set_name: str
 ) -> Union["GraphenePartitionSet", "GraphenePartitionSetNotFoundError"]:
     from ..schema.partition_sets import GraphenePartitionSet, GraphenePartitionSetNotFoundError
 
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
     check.str_param(partition_set_name, "partition_set_name")
@@ -92,15 +88,14 @@
                 external_repository_handle=repository.handle,
                 external_partition_set=partition_set,
             )
 
     return GraphenePartitionSetNotFoundError(partition_set_name)
 
 
-@capture_error
 def get_partition_by_name(
     graphene_info: ResolveInfo,
     repository_handle: RepositoryHandle,
     partition_set: ExternalPartitionSet,
     partition_name: str,
 ) -> "GraphenePartition":
     from ..schema.partition_sets import GraphenePartition
@@ -111,15 +106,14 @@
     return GraphenePartition(
         external_repository_handle=repository_handle,
         external_partition_set=partition_set,
         partition_name=partition_name,
     )
 
 
-@capture_error
 def get_partition_config(
     graphene_info: ResolveInfo,
     repository_handle: RepositoryHandle,
     partition_set_name: str,
     partition_name: str,
 ) -> "GraphenePartitionRunConfig":
     from ..schema.partition_sets import GraphenePartitionRunConfig
@@ -137,15 +131,14 @@
 
     if isinstance(result, ExternalPartitionExecutionErrorData):
         raise DagsterUserCodeProcessError.from_error_info(result.error)
 
     return GraphenePartitionRunConfig(yaml=dump_run_config_yaml(result.run_config))
 
 
-@capture_error
 def get_partition_tags(
     graphene_info: ResolveInfo,
     repository_handle: RepositoryHandle,
     partition_set_name: str,
     partition_name: str,
 ) -> "GraphenePartitionTags":
     from ..schema.partition_sets import GraphenePartitionTags
@@ -167,15 +160,14 @@
             GraphenePipelineTag(key=key, value=value)
             for key, value in result.tags.items()
             if get_tag_type(key) != TagType.HIDDEN
         ]
     )
 
 
-@capture_error
 def get_partitions(
     graphene_info: ResolveInfo,
     repository_handle: RepositoryHandle,
     partition_set: ExternalPartitionSet,
     cursor: Optional[str] = None,
     limit: Optional[int] = None,
     reverse: bool = False,
@@ -223,15 +215,14 @@
             start = end - limit
         else:
             end = start + limit
 
     return items[max(start, 0) : end]
 
 
-@capture_error
 def get_partition_set_partition_statuses(
     graphene_info: ResolveInfo, external_partition_set: ExternalPartitionSet
 ) -> Sequence["GraphenePartitionStatus"]:
     check.inst_param(external_partition_set, "external_partition_set", ExternalPartitionSet)
 
     repository_handle = external_partition_set.repository_handle
     partition_set_name = external_partition_set.name
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 import dagster._check as check
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRun
 
 from dagster_graphql.schema.util import ResolveInfo
 
 from .external import get_external_job_or_raise, get_full_external_job_or_raise
-from .utils import JobSubsetSelector, UserFacingGraphQLError, capture_error
+from .utils import JobSubsetSelector, UserFacingGraphQLError
 
 if TYPE_CHECKING:
     from ..schema.pipelines.pipeline import GraphenePipeline
     from ..schema.pipelines.pipeline_ref import GrapheneUnknownPipeline
     from ..schema.pipelines.snapshot import GraphenePipelineSnapshot
 
 
-@capture_error
 def get_job_snapshot_or_error_from_job_selector(
     graphene_info: ResolveInfo, job_selector: JobSubsetSelector
 ) -> "GraphenePipelineSnapshot":
     from ..schema.pipelines.snapshot import GraphenePipelineSnapshot
 
     check.inst_param(job_selector, "pipeline_selector", JobSubsetSelector)
     return GraphenePipelineSnapshot(get_full_external_job_or_raise(graphene_info, job_selector))
 
 
-@capture_error
 def get_job_snapshot_or_error_from_snapshot_id(
     graphene_info: ResolveInfo, snapshot_id: str
 ) -> "GraphenePipelineSnapshot":
     check.str_param(snapshot_id, "snapshot_id")
     return _get_job_snapshot_from_instance(graphene_info.context.instance, snapshot_id)
 
 
@@ -48,15 +46,14 @@
     if not historical_pipeline:
         # Either a temporary error or it has been deleted in the interim
         raise UserFacingGraphQLError(GraphenePipelineSnapshotNotFoundError(snapshot_id))
 
     return GraphenePipelineSnapshot(historical_pipeline)
 
 
-@capture_error
 def get_job_or_error(graphene_info: ResolveInfo, selector: JobSubsetSelector) -> "GraphenePipeline":
     """Returns a PipelineOrError."""
     return get_job_from_selector(graphene_info, selector)
 
 
 def get_job_or_raise(graphene_info: ResolveInfo, selector: JobSubsetSelector) -> "GraphenePipeline":
     """Returns a Pipeline or raises a UserFacingGraphQLError if one cannot be retrieved
@@ -71,18 +68,20 @@
     """Returns a PipelineReference or raises a UserFacingGraphQLError if a pipeline
     reference cannot be retrieved based on the run, e.g, a UserFacingGraphQLError that wraps an
     InvalidSubsetError.
     """
     from ..schema.pipelines.pipeline_ref import GrapheneUnknownPipeline
 
     check.inst_param(dagster_run, "pipeline_run", DagsterRun)
-    solid_selection = list(dagster_run.solids_to_execute) if dagster_run.solids_to_execute else None
+    op_selection = (
+        list(dagster_run.resolved_op_selection) if dagster_run.resolved_op_selection else None
+    )
 
     if dagster_run.job_snapshot_id is None:
-        return GrapheneUnknownPipeline(dagster_run.job_name, solid_selection)
+        return GrapheneUnknownPipeline(dagster_run.job_name, op_selection)
 
     return _get_job_snapshot_from_instance(
         graphene_info.context.instance, dagster_run.job_snapshot_id
     )
 
 
 def get_job_from_selector(
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import TYPE_CHECKING
 
 import dagster._check as check
 from dagster._core.definitions.selector import RepositorySelector, ResourceSelector
 from dagster._core.host_representation.code_location import CodeLocation
 from graphene import ResolveInfo
 
-from .utils import UserFacingGraphQLError, capture_error
+from .utils import UserFacingGraphQLError
 
 if TYPE_CHECKING:
     from ..schema.resources import GrapheneResourceDetails, GrapheneResourceDetailsList
 
 
-@capture_error
 def get_top_level_resources_or_error(
     graphene_info: "ResolveInfo", repository_selector: RepositorySelector
 ) -> "GrapheneResourceDetailsList":
     from ..schema.resources import GrapheneResourceDetails, GrapheneResourceDetailsList
 
     check.inst_param(graphene_info, "graphene_info", ResolveInfo)
     check.inst_param(repository_selector, "repository_selector", RepositorySelector)
@@ -35,15 +34,14 @@
         for external_resource in external_resources
         if external_resource.is_top_level
     ]
 
     return GrapheneResourceDetailsList(results=results)
 
 
-@capture_error
 def get_resource_or_error(
     graphene_info: "ResolveInfo", resource_selector: ResourceSelector
 ) -> "GrapheneResourceDetails":
     from ..schema.errors import GrapheneResourceNotFoundError
     from ..schema.resources import GrapheneResourceDetails
 
     check.inst_param(graphene_info, "graphene_info", ResolveInfo)
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.errors import DagsterRunNotFoundError
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, StepEventStatus
 from dagster._core.storage.dagster_run import DagsterRunStatus, RunRecord, RunsFilter
 from dagster._core.storage.tags import TagType, get_tag_type
 
 from .external import ensure_valid_config, get_external_job_or_raise
-from .utils import capture_error
 
 if TYPE_CHECKING:
     from ..schema.asset_graph import GrapheneAssetLatestInfo, GrapheneAssetNode
     from ..schema.errors import GrapheneRunNotFoundError
     from ..schema.execution import GrapheneExecutionPlan
     from ..schema.logs.events import GrapheneRunStepStats
     from ..schema.pipelines.config import GraphenePipelineConfigValidationValid
@@ -49,28 +48,26 @@
     record = instance.get_run_record_by_id(run_id)
     if not record:
         return GrapheneRunNotFoundError(run_id)
     else:
         return GrapheneRun(record)
 
 
-@capture_error
 def get_run_tag_keys(graphene_info: "ResolveInfo") -> "GrapheneRunTagKeys":
     from ..schema.runs import GrapheneRunTagKeys
 
     return GrapheneRunTagKeys(
         keys=[
             tag_key
             for tag_key in graphene_info.context.instance.get_run_tag_keys()
             if get_tag_type(tag_key) != TagType.HIDDEN
         ]
     )
 
 
-@capture_error
 def get_run_tags(
     graphene_info: "ResolveInfo",
     tag_keys: Optional[List[str]] = None,
     value_prefix: Optional[str] = None,
     limit: Optional[int] = None,
 ) -> "GrapheneRunTags":
     from ..schema.runs import GrapheneRunTags
@@ -84,15 +81,14 @@
                 tag_keys=tag_keys, value_prefix=value_prefix, limit=limit
             )
             if get_tag_type(key) != TagType.HIDDEN
         ]
     )
 
 
-@capture_error
 def get_run_group(graphene_info: "ResolveInfo", run_id: str) -> "GrapheneRunGroup":
     from ..schema.errors import GrapheneRunGroupNotFoundError
     from ..schema.pipelines.pipeline import GrapheneRun
     from ..schema.runs import GrapheneRunGroup
 
     instance = graphene_info.context.instance
     try:
@@ -326,30 +322,28 @@
 
     return [
         GrapheneRunGroup(root_run_id=root_run_id, runs=run_group["runs"])
         for root_run_id, run_group in run_groups.items()
     ]
 
 
-@capture_error
 def validate_pipeline_config(
     graphene_info: "ResolveInfo",
     selector: JobSubsetSelector,
     run_config: Union[str, Mapping[str, object]],
 ) -> "GraphenePipelineConfigValidationValid":
     from ..schema.pipelines.config import GraphenePipelineConfigValidationValid
 
     check.inst_param(selector, "selector", JobSubsetSelector)
 
     external_job = get_external_job_or_raise(graphene_info, selector)
     ensure_valid_config(external_job, run_config)
     return GraphenePipelineConfigValidationValid(pipeline_name=external_job.name)
 
 
-@capture_error
 def get_execution_plan(
     graphene_info: "ResolveInfo",
     selector: JobSubsetSelector,
     run_config: Mapping[str, Any],
 ) -> "GrapheneExecutionPlan":
     from ..schema.execution import GrapheneExecutionPlan
 
@@ -363,15 +357,14 @@
             run_config=run_config,
             step_keys_to_execute=None,
             known_state=None,
         )
     )
 
 
-@capture_error
 def get_stats(graphene_info: "ResolveInfo", run_id: str) -> "GrapheneRunStatsSnapshot":
     from ..schema.pipelines.pipeline_run_stats import GrapheneRunStatsSnapshot
 
     stats = graphene_info.context.instance.get_run_stats(run_id)
     stats.id = "stats-{run_id}"  # type: ignore  # (unused code path)
     return GrapheneRunStatsSnapshot(stats)
 
@@ -381,15 +374,14 @@
 ) -> Sequence["GrapheneRunStepStats"]:
     from ..schema.logs.events import GrapheneRunStepStats
 
     step_stats = graphene_info.context.instance.get_run_step_stats(run_id, step_keys)
     return [GrapheneRunStepStats(stats) for stats in step_stats]
 
 
-@capture_error
 def get_logs_for_run(
     graphene_info: "ResolveInfo",
     run_id: str,
     cursor: Optional[str] = None,
     limit: Optional[int] = None,
 ) -> Union["GrapheneRunNotFoundError", "GrapheneEventConnection"]:
     from ..schema.errors import GrapheneRunNotFoundError
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 from dagster_graphql.schema.util import ResolveInfo
 
 from .loader import RepositoryScopedBatchLoader
 from .utils import (
     UserFacingGraphQLError,
     assert_permission,
     assert_permission_for_location,
-    capture_error,
 )
 
 if TYPE_CHECKING:
     from ..schema.instigation import GrapheneDryRunInstigationTick
     from ..schema.schedules import (
         GrapheneSchedule,
         GrapheneScheduler,
         GrapheneSchedules,
         GrapheneScheduleStateResult,
     )
 
 
-@capture_error
 def start_schedule(
     graphene_info: ResolveInfo, schedule_selector: ScheduleSelector
 ) -> "GrapheneScheduleStateResult":
     from ..schema.instigation import GrapheneInstigationState
     from ..schema.schedules import GrapheneScheduleStateResult
 
     check.inst_param(schedule_selector, "schedule_selector", ScheduleSelector)
@@ -44,15 +42,14 @@
     instance = graphene_info.context.instance
     schedule_state = instance.start_schedule(
         repository.get_external_schedule(schedule_selector.schedule_name)
     )
     return GrapheneScheduleStateResult(GrapheneInstigationState(schedule_state))
 
 
-@capture_error
 def stop_schedule(
     graphene_info: ResolveInfo, schedule_origin_id: str, schedule_selector_id: str
 ) -> "GrapheneScheduleStateResult":
     from ..schema.instigation import GrapheneInstigationState
     from ..schema.schedules import GrapheneScheduleStateResult
 
     instance = graphene_info.context.instance
@@ -80,28 +77,26 @@
 
     schedule_state = instance.stop_schedule(
         schedule_origin_id, schedule_selector_id, external_schedule
     )
     return GrapheneScheduleStateResult(GrapheneInstigationState(schedule_state))
 
 
-@capture_error
 def get_scheduler_or_error(graphene_info: ResolveInfo) -> "GrapheneScheduler":
     from ..schema.errors import GrapheneSchedulerNotDefinedError
     from ..schema.schedules import GrapheneScheduler
 
     instance = graphene_info.context.instance
 
     if not instance.scheduler:
         raise UserFacingGraphQLError(GrapheneSchedulerNotDefinedError())
 
     return GrapheneScheduler(scheduler_class=instance.scheduler.__class__.__name__)
 
 
-@capture_error
 def get_schedules_or_error(
     graphene_info: ResolveInfo,
     repository_selector: RepositorySelector,
     instigator_statuses: Optional[Set[InstigatorStatus]] = None,
 ) -> "GrapheneSchedules":
     from ..schema.schedules import GrapheneSchedule, GrapheneSchedules
 
@@ -160,15 +155,14 @@
             external_schedule.selector_id,
         )
         results.append(GrapheneSchedule(external_schedule, schedule_state))
 
     return results
 
 
-@capture_error
 def get_schedule_or_error(
     graphene_info: ResolveInfo, schedule_selector: ScheduleSelector
 ) -> "GrapheneSchedule":
     from ..schema.errors import GrapheneScheduleNotFoundError
     from ..schema.schedules import GrapheneSchedule
 
     check.inst_param(schedule_selector, "schedule_selector", ScheduleSelector)
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_sensors.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,27 +14,22 @@
 from dagster_graphql.schema.util import ResolveInfo
 
 from .loader import RepositoryScopedBatchLoader
 from .utils import (
     UserFacingGraphQLError,
     assert_permission,
     assert_permission_for_location,
-    capture_error,
 )
 
 if TYPE_CHECKING:
     from dagster_graphql.schema.instigation import GrapheneDryRunInstigationTick
 
-    from ..schema.instigation import (
-        GrapheneInstigationStates,
-    )
     from ..schema.sensors import GrapheneSensor, GrapheneSensors, GrapheneStopSensorMutationResult
 
 
-@capture_error
 def get_sensors_or_error(
     graphene_info: ResolveInfo,
     repository_selector: RepositorySelector,
     instigator_statuses: Optional[Set[InstigatorStatus]] = None,
 ) -> "GrapheneSensors":
     from ..schema.sensors import GrapheneSensor, GrapheneSensors
 
@@ -66,15 +61,14 @@
         results=[
             GrapheneSensor(sensor, sensor_states_by_name.get(sensor.name), batch_loader)
             for sensor in filtered
         ]
     )
 
 
-@capture_error
 def get_sensor_or_error(graphene_info: ResolveInfo, selector: SensorSelector) -> "GrapheneSensor":
     from ..schema.errors import GrapheneSensorNotFoundError
     from ..schema.sensors import GrapheneSensor
 
     check.inst_param(selector, "selector", SensorSelector)
     location = graphene_info.context.get_code_location(selector.location_name)
     repository = location.get_repository(selector.repository_name)
@@ -86,15 +80,14 @@
         external_sensor.get_external_origin_id(),
         external_sensor.selector_id,
     )
 
     return GrapheneSensor(external_sensor, sensor_state)
 
 
-@capture_error
 def start_sensor(graphene_info: ResolveInfo, sensor_selector: SensorSelector) -> "GrapheneSensor":
     from ..schema.errors import GrapheneSensorNotFoundError
     from ..schema.sensors import GrapheneSensor
 
     check.inst_param(sensor_selector, "sensor_selector", SensorSelector)
 
     location = graphene_info.context.get_code_location(sensor_selector.location_name)
@@ -106,15 +99,14 @@
     sensor_state = graphene_info.context.instance.get_instigator_state(
         external_sensor.get_external_origin_id(),
         external_sensor.selector_id,
     )
     return GrapheneSensor(external_sensor, sensor_state)
 
 
-@capture_error
 def stop_sensor(
     graphene_info: ResolveInfo, instigator_origin_id: str, instigator_selector_id: str
 ) -> "GrapheneStopSensorMutationResult":
     from ..schema.sensors import GrapheneStopSensorMutationResult
 
     check.str_param(instigator_origin_id, "instigator_origin_id")
     instance = graphene_info.context.instance
@@ -143,48 +135,14 @@
         instigator_origin_id,
         instigator_selector_id,
         external_sensor,
     )
     return GrapheneStopSensorMutationResult(state)
 
 
-@capture_error
-def get_unloadable_sensor_states_or_error(
-    graphene_info: ResolveInfo,
-) -> "GrapheneInstigationStates":
-    from ..schema.instigation import GrapheneInstigationState, GrapheneInstigationStates
-
-    sensor_states = graphene_info.context.instance.all_instigator_state(
-        instigator_type=InstigatorType.SENSOR
-    )
-    external_sensors = [
-        sensor
-        for repository_location in graphene_info.context.code_locations
-        for repository in repository_location.get_repositories().values()
-        for sensor in repository.get_external_sensors()
-    ]
-
-    sensor_origin_ids = {
-        external_sensor.get_external_origin_id() for external_sensor in external_sensors
-    }
-
-    unloadable_states = [
-        sensor_state
-        for sensor_state in sensor_states
-        if sensor_state.instigator_origin_id not in sensor_origin_ids
-    ]
-
-    return GrapheneInstigationStates(
-        results=[
-            GrapheneInstigationState(instigator_state=sensor_state)
-            for sensor_state in unloadable_states
-        ]
-    )
-
-
 def get_sensors_for_pipeline(
     graphene_info: ResolveInfo, pipeline_selector: JobSubsetSelector
 ) -> Sequence["GrapheneSensor"]:
     from ..schema.sensors import GrapheneSensor
 
     check.inst_param(pipeline_selector, "pipeline_selector", JobSubsetSelector)
 
@@ -246,15 +204,14 @@
 
     next_timestamp = latest_tick.timestamp + external_sensor.min_interval_seconds
     if next_timestamp < get_timestamp_from_utc_datetime(get_current_datetime_in_utc()):
         return None
     return GrapheneDryRunInstigationTick(external_sensor.sensor_selector, next_timestamp)
 
 
-@capture_error
 def set_sensor_cursor(
     graphene_info: ResolveInfo, selector: SensorSelector, cursor: Optional[str]
 ) -> "GrapheneSensor":
     check.inst_param(selector, "selector", SensorSelector)
     check.opt_str_param(cursor, "cursor")
 
     from ..schema.errors import GrapheneSensorNotFoundError
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_solids.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import OrderedDict, defaultdict
 
 import dagster._check as check
 from dagster._core.host_representation import ExternalRepository
 
-from .utils import GraphSelector, capture_error
+from .utils import GraphSelector
 
 
 def get_solid(repo, name):
     return get_used_solid_map(repo)[name]
 
 
 def get_solids(repo):
@@ -47,15 +47,14 @@
                 ),
             ),
         )
         for definition in sorted(definitions, key=lambda d: d.name)
     )
 
 
-@capture_error
 def get_graph_or_error(graphene_info, graph_selector):
     from ..schema.errors import GrapheneGraphNotFoundError
     from ..schema.pipelines.pipeline import GrapheneGraph
     from ..schema.solids import build_solid_handles
 
     check.inst_param(graph_selector, "graph_selector", GraphSelector)
     if not graphene_info.context.has_code_location(graph_selector.location_name):
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/run_config_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 from dagster._core.host_representation import RepresentedJob
 from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 
 from dagster_graphql.schema.errors import GrapheneModeNotFoundError
 from dagster_graphql.schema.util import ResolveInfo
 
 from .external import get_external_job_or_raise
-from .utils import JobSubsetSelector, UserFacingGraphQLError, capture_error
+from .utils import JobSubsetSelector, UserFacingGraphQLError
 
 if TYPE_CHECKING:
     from ..schema.pipelines.config import (
         GraphenePipelineConfigValidationValid,
     )
     from ..schema.run_config import GrapheneRunConfigSchema
 
 
-@capture_error
 def resolve_run_config_schema_or_error(
     graphene_info: ResolveInfo, selector: JobSubsetSelector, mode: Optional[str] = None
 ) -> "GrapheneRunConfigSchema":
     from ..schema.run_config import GrapheneRunConfigSchema
 
     check.inst_param(selector, "selector", JobSubsetSelector)
 
@@ -36,15 +35,14 @@
 
     return GrapheneRunConfigSchema(
         represented_job=external_job,
         mode=DEFAULT_MODE_NAME,
     )
 
 
-@capture_error
 def resolve_is_run_config_valid(
     graphene_info: ResolveInfo,
     represented_pipeline: RepresentedJob,
     mode: str,
     run_config: Mapping[str, object],
 ) -> "GraphenePipelineConfigValidationValid":
     from ..schema.pipelines.config import (
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.5/dagster_graphql/implementation/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 def pipeline_selector_from_graphql(data: Mapping[str, Any]) -> JobSubsetSelector:
     asset_selection = cast(Optional[Iterable[Dict[str, List[str]]]], data.get("assetSelection"))
     return JobSubsetSelector(
         location_name=data["repositoryLocationName"],
         repository_name=data["repositoryName"],
         job_name=data.get("pipelineName") or data.get("jobName"),  # type: ignore
-        solid_selection=data.get("solidSelection"),
+        op_selection=data.get("solidSelection"),
         asset_selection=[AssetKey.from_graphql_input(asset_key) for asset_key in asset_selection]
         if asset_selection
         else None,
     )
 
 
 def graph_selector_from_graphql(data: Mapping[str, Any]) -> GraphSelector:
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/partition_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     get_partition_config,
     get_partition_set_partition_runs,
     get_partition_set_partition_statuses,
     get_partition_tags,
     get_partitions,
 )
 from dagster_graphql.implementation.fetch_runs import get_runs
+from dagster_graphql.implementation.utils import capture_error
 
 from .asset_key import GrapheneAssetKey
 from .backfill import GraphenePartitionBackfill
 from .errors import (
     GrapheneDuplicateDynamicPartitionError,
     GraphenePartitionSetNotFoundError,
     GraphenePipelineNotFoundError,
@@ -194,26 +195,28 @@
             external_partition_set, "external_partition_set", ExternalPartitionSet
         )
         self._partition_name = check.str_param(partition_name, "partition_name")
 
         super().__init__(
             name=partition_name,
             partition_set_name=external_partition_set.name,
-            solid_selection=external_partition_set.solid_selection,
+            solid_selection=external_partition_set.op_selection,
             mode=external_partition_set.mode,
         )
 
+    @capture_error
     def resolve_runConfigOrError(self, graphene_info: ResolveInfo):
         return get_partition_config(
             graphene_info,
             self._external_repository_handle,
             self._external_partition_set.name,
             self._partition_name,
         )
 
+    @capture_error
     def resolve_tagsOrError(self, graphene_info: ResolveInfo):
         return get_partition_tags(
             graphene_info,
             self._external_repository_handle,
             self._external_partition_set.name,
             self._partition_name,
         )
@@ -292,21 +295,22 @@
         self._external_partition_set = check.inst_param(
             external_partition_set, "external_partition_set", ExternalPartitionSet
         )
 
         super().__init__(
             name=external_partition_set.name,
             pipeline_name=external_partition_set.job_name,
-            solid_selection=external_partition_set.solid_selection,
+            solid_selection=external_partition_set.op_selection,
             mode=external_partition_set.mode,
         )
 
     def resolve_id(self, _graphene_info: ResolveInfo):
         return self._external_partition_set.get_external_origin_id()
 
+    @capture_error
     def resolve_partitionsOrError(
         self,
         graphene_info: ResolveInfo,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
         reverse: Optional[bool] = None,
     ):
@@ -326,14 +330,15 @@
             self._external_partition_set,
             partition_name,
         )
 
     def resolve_partitionRuns(self, graphene_info: ResolveInfo):
         return get_partition_set_partition_runs(graphene_info, self._external_partition_set)
 
+    @capture_error
     def resolve_partitionStatusesOrError(self, graphene_info: ResolveInfo):
         return get_partition_set_partition_statuses(
             graphene_info,
             self._external_partition_set,
         )
 
     def resolve_repositoryOrigin(self, _):
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 from typing import List, Optional, Sequence
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.time_window_partitions import PartitionRangeStatus
 from dagster._core.events import DagsterEventType
 from dagster._core.host_representation.external import ExternalExecutionPlan, ExternalJob
@@ -424,35 +423,36 @@
     def resolve_pipelineName(self, _graphene_info: ResolveInfo):
         return self.dagster_run.job_name
 
     def resolve_jobName(self, _graphene_info: ResolveInfo):
         return self.dagster_run.job_name
 
     def resolve_solidSelection(self, _graphene_info: ResolveInfo):
-        return self.dagster_run.solid_selection
+        return self.dagster_run.op_selection
 
     def resolve_assetSelection(self, _graphene_info: ResolveInfo):
         return self.dagster_run.asset_selection
 
     def resolve_resolvedOpSelection(self, _graphene_info: ResolveInfo):
-        return self.dagster_run.solids_to_execute
+        return self.dagster_run.resolved_op_selection
 
     def resolve_pipelineSnapshotId(self, _graphene_info: ResolveInfo):
         return self.dagster_run.job_snapshot_id
 
     def resolve_parentPipelineSnapshotId(self, graphene_info: ResolveInfo):
         pipeline_snapshot_id = self.dagster_run.job_snapshot_id
         if pipeline_snapshot_id is not None and graphene_info.context.instance.has_job_snapshot(
             pipeline_snapshot_id
         ):
             snapshot = graphene_info.context.instance.get_job_snapshot(pipeline_snapshot_id)
             if snapshot.lineage_snapshot is not None:
                 return snapshot.lineage_snapshot.parent_snapshot_id
         return None
 
+    @capture_error
     def resolve_stats(self, graphene_info: ResolveInfo):
         return get_stats(graphene_info, self.run_id)
 
     def resolve_stepStats(self, graphene_info: ResolveInfo):
         return get_step_stats(graphene_info, self.run_id)
 
     def resolve_computeLogs(self, _graphene_info: ResolveInfo, stepKey):
@@ -567,16 +567,15 @@
             if self._run_stats is None or self._run_stats.end_time is None:
                 self._run_stats = graphene_info.context.instance.get_run_stats(self.runId)
             return self._run_stats.end_time
         return run_record.end_time
 
     def resolve_updateTime(self, graphene_info: ResolveInfo):
         run_record = self._get_run_record(graphene_info.context.instance)
-        updated = run_record.update_timestamp.timestamp()
-        return datetime_as_float(datetime.datetime.utcfromtimestamp(updated))
+        return datetime_as_float(run_record.update_timestamp)
 
 
 class GrapheneIPipelineSnapshotMixin:
     # Mixin this class to implement IPipelineSnapshot
     #
     # Graphene has some strange properties that make it so that you cannot
     # implement ABCs nor use properties in an overridable way. So the way
@@ -708,15 +707,15 @@
         ]
 
     def resolve_metadata_entries(self, _graphene_info: ResolveInfo) -> List[GrapheneMetadataEntry]:
         represented_pipeline = self.get_represented_job()
         return list(iterate_metadata_entries(represented_pipeline.job_snapshot.metadata))
 
     def resolve_solidSelection(self, _graphene_info: ResolveInfo):
-        return self.get_represented_job().solid_selection
+        return self.get_represented_job().op_selection
 
     def resolve_runs(
         self, graphene_info: ResolveInfo, cursor: Optional[str] = None, limit: Optional[int] = None
     ) -> Sequence[GrapheneRun]:
         pipeline = self.get_represented_job()
         if isinstance(pipeline, ExternalJob):
             runs_filter = RunsFilter(
@@ -813,15 +812,15 @@
         )
         self._job_name = check.str_param(pipeline_name, "pipeline_name")
 
     def resolve_name(self, _graphene_info: ResolveInfo):
         return self._active_preset_data.name
 
     def resolve_solidSelection(self, _graphene_info: ResolveInfo):
-        return self._active_preset_data.solid_selection
+        return self._active_preset_data.op_selection
 
     def resolve_runConfigYaml(self, _graphene_info: ResolveInfo):
         return dump_run_config_yaml(self._active_preset_data.run_config) or ""
 
     def resolve_mode(self, _graphene_info: ResolveInfo):
         return self._active_preset_data.mode
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             )
 
         if graphql_execution_params.get("mode"):
             raise UserFacingGraphQLError(
                 GrapheneConflictingExecutionParamsError(conflicting_param="mode")
             )
 
-        if selector.solid_selection:
+        if selector.op_selection:
             raise UserFacingGraphQLError(
                 GrapheneConflictingExecutionParamsError(
                     conflicting_param="selector.solid_selection"
                 )
             )
 
         external_pipeline = get_full_external_job_or_raise(
@@ -110,15 +110,15 @@
             raise UserFacingGraphQLError(
                 GraphenePresetNotFoundError(preset=preset_name, selector=selector)
             )
 
         preset = external_pipeline.get_preset(preset_name)
 
         return ExecutionParams(
-            selector=selector.with_solid_selection(preset.solid_selection),
+            selector=selector.with_op_selection(preset.op_selection),
             run_config=preset.run_config,
             mode=preset.mode,
             execution_metadata=create_execution_metadata(
                 graphql_execution_params.get("executionMetadata")
             ),
             step_keys=graphql_execution_params.get("stepKeys"),
         )
@@ -245,16 +245,14 @@
             GrapheneUnauthorizedError,
             GraphenePythonError,
         )
         name = "TerminateRunResult"
 
 
 def create_execution_params_and_launch_pipeline_exec(graphene_info, execution_params_dict):
-    # refactored into a helper function here in order to wrap with @capture_error,
-    # because create_execution_params may raise
     execution_params = create_execution_params(graphene_info, execution_params_dict)
     assert_permission_for_location(
         graphene_info,
         Permissions.LAUNCH_PIPELINE_EXECUTION,
         execution_params.selector.location_name,
     )
     return launch_pipeline_execution(
@@ -356,18 +354,15 @@
         partitionKey: str,
     ):
         return add_dynamic_partition(
             graphene_info, repositorySelector, partitionsDefName, partitionKey
         )
 
 
-@capture_error
 def create_execution_params_and_launch_pipeline_reexec(graphene_info, execution_params_dict):
-    # refactored into a helper function here in order to wrap with @capture_error,
-    # because create_execution_params may raise
     execution_params = create_execution_params(graphene_info, execution_params_dict)
     assert_permission_for_location(
         graphene_info,
         Permissions.LAUNCH_PIPELINE_REEXECUTION,
         execution_params.selector.location_name,
     )
     return launch_pipeline_reexecution(graphene_info, execution_params=execution_params)
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,19 @@
 from ...implementation.fetch_solids import get_graph_or_error
 from ...implementation.loader import (
     BatchMaterializationLoader,
     CrossRepoAssetDependedByLoader,
     StaleStatusLoader,
 )
 from ...implementation.run_config_schema import resolve_run_config_schema_or_error
-from ...implementation.utils import graph_selector_from_graphql, pipeline_selector_from_graphql
+from ...implementation.utils import (
+    capture_error,
+    graph_selector_from_graphql,
+    pipeline_selector_from_graphql,
+)
 from ..asset_graph import (
     GrapheneAssetLatestInfo,
     GrapheneAssetNode,
     GrapheneAssetNodeDefinitionCollision,
     GrapheneAssetNodeOrError,
 )
 from ..backfill import (
@@ -455,14 +459,15 @@
     )
 
     test = graphene.Field(
         GrapheneTestFields,
         description="Provides fields for testing behavior",
     )
 
+    @capture_error
     def resolve_repositoriesOrError(
         self,
         graphene_info: ResolveInfo,
         repositorySelector: Optional[GrapheneRepositorySelector] = None,
     ):
         if repositorySelector:
             return GrapheneRepositoryConnection(
@@ -471,27 +476,31 @@
                         graphene_info,
                         RepositorySelector.from_graphql_input(repositorySelector),
                     )
                 ]
             )
         return fetch_repositories(graphene_info)
 
+    @capture_error
     def resolve_repositoryOrError(
         self, graphene_info: ResolveInfo, repositorySelector: GrapheneRepositorySelector
     ):
         return fetch_repository(
             graphene_info, RepositorySelector.from_graphql_input(repositorySelector)
         )
 
+    @capture_error
     def resolve_workspaceOrError(self, graphene_info: ResolveInfo):
         return fetch_workspace(graphene_info.context)
 
+    @capture_error
     def resolve_locationStatusesOrError(self, graphene_info: ResolveInfo):
         return fetch_location_statuses(graphene_info.context)
 
+    @capture_error
     def resolve_pipelineSnapshotOrError(
         self,
         graphene_info: ResolveInfo,
         snapshotId: Optional[str] = None,
         activePipelineSelector: Optional[GraphenePipelineSelector] = None,
     ):
         check.invariant(
@@ -505,34 +514,38 @@
         elif snapshotId:
             return get_job_snapshot_or_error_from_snapshot_id(graphene_info, snapshotId)
         else:
             check.failed(
                 "Must set one of snapshotId or activePipelineSelector",
             )
 
+    @capture_error
     def resolve_graphOrError(
         self, graphene_info: ResolveInfo, selector: Optional[GrapheneGraphSelector] = None
     ):
         assert selector is not None
         graph_selector = graph_selector_from_graphql(selector)
         return get_graph_or_error(graphene_info, graph_selector)
 
     def resolve_version(self, graphene_info: ResolveInfo):
         return graphene_info.context.version
 
+    @capture_error
     def resolve_scheduler(self, graphene_info: ResolveInfo):
         return get_scheduler_or_error(graphene_info)
 
+    @capture_error
     def resolve_scheduleOrError(
         self, graphene_info: ResolveInfo, schedule_selector: GrapheneScheduleSelector
     ):
         return get_schedule_or_error(
             graphene_info, ScheduleSelector.from_graphql_input(schedule_selector)
         )
 
+    @capture_error
     def resolve_schedulesOrError(
         self,
         graphene_info: ResolveInfo,
         repositorySelector: GrapheneRepositorySelector,
         scheduleStatus: Optional[GrapheneInstigationStatus] = None,
     ):
         if scheduleStatus == GrapheneInstigationStatus.RUNNING:
@@ -544,36 +557,40 @@
 
         return get_schedules_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(repositorySelector),
             instigator_statuses,
         )
 
+    @capture_error
     def resolve_topLevelResourceDetailsOrError(self, graphene_info: ResolveInfo, resourceSelector):
         return get_resource_or_error(
             graphene_info, ResourceSelector.from_graphql_input(resourceSelector)
         )
 
     def resolve_allTopLevelResourceDetailsOrError(self, graphene_info: ResolveInfo, **kwargs):
         return get_top_level_resources_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(kwargs.get("repositorySelector")),
         )
 
+    @capture_error
     def resolve_utilizedEnvVarsOrError(self, graphene_info: ResolveInfo, **kwargs):
         return get_utilized_env_vars_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(kwargs.get("repositorySelector")),
         )
 
+    @capture_error
     def resolve_sensorOrError(
         self, graphene_info: ResolveInfo, sensorSelector: GrapheneRepositorySelector
     ):
         return get_sensor_or_error(graphene_info, SensorSelector.from_graphql_input(sensorSelector))
 
+    @capture_error
     def resolve_sensorsOrError(
         self,
         graphene_info,
         repositorySelector: GrapheneRepositorySelector,
         sensorStatus: Optional[GrapheneInstigationStatus] = None,
     ):
         if sensorStatus == GrapheneInstigationStatus.RUNNING:
@@ -584,27 +601,30 @@
             instigator_statuses = None
         return get_sensors_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(repositorySelector),
             instigator_statuses,
         )
 
+    @capture_error
     def resolve_instigationStateOrError(
         self, graphene_info: ResolveInfo, instigationSelector: GrapheneInstigationSelector
     ):
         return get_instigator_state_or_error(
             graphene_info, InstigatorSelector.from_graphql_input(instigationSelector)
         )
 
+    @capture_error
     def resolve_unloadableInstigationStatesOrError(
         self, graphene_info: ResolveInfo, instigationType: Optional[GrapheneInstigationType] = None
     ):
         instigation_type = InstigatorType(instigationType) if instigationType else None
         return get_unloadable_instigator_states_or_error(graphene_info, instigation_type)
 
+    @capture_error
     def resolve_pipelineOrError(self, graphene_info: ResolveInfo, params: GraphenePipelineSelector):
         return get_job_or_error(
             graphene_info,
             pipeline_selector_from_graphql(params),
         )
 
     def resolve_pipelineRunsOrError(
@@ -652,77 +672,85 @@
     ):
         selector = filter.to_selector() if filter is not None else None
 
         return GrapheneRunGroupsOrError(
             results=get_run_groups(graphene_info, selector, cursor, limit)
         )
 
+    @capture_error
     def resolve_partitionSetsOrError(
         self, graphene_info: ResolveInfo, repositorySelector: RepositorySelector, pipelineName: str
     ):
         return get_partition_sets_or_error(
             graphene_info,
             RepositorySelector.from_graphql_input(repositorySelector),
             pipelineName,
         )
 
+    @capture_error
     def resolve_partitionSetOrError(
         self,
         graphene_info: ResolveInfo,
         repositorySelector: RepositorySelector,
         partitionSetName: Optional[str] = None,
     ):
         return get_partition_set(
             graphene_info,
             RepositorySelector.from_graphql_input(repositorySelector),
             # partitionSetName should prob be required
             partitionSetName,  # type: ignore
         )
 
+    @capture_error
     def resolve_runTagKeysOrError(self, graphene_info: ResolveInfo):
         return get_run_tag_keys(graphene_info)
 
+    @capture_error
     def resolve_runTagsOrError(
         self,
         graphene_info: ResolveInfo,
         tagKeys: Optional[List[str]] = None,
         valuePrefix: Optional[str] = None,
         limit: Optional[int] = None,
     ):
         return get_run_tags(graphene_info, tagKeys, valuePrefix, limit)
 
+    @capture_error
     def resolve_runGroupOrError(self, graphene_info: ResolveInfo, runId):
         return get_run_group(graphene_info, runId)
 
+    @capture_error
     def resolve_isPipelineConfigValid(
         self,
         graphene_info: ResolveInfo,
         pipeline: GraphenePipelineSelector,
         mode: str,
         runConfigData: Optional[Any] = None,  # custom scalar (GrapheneRunConfigData)
     ):
         return validate_pipeline_config(
             graphene_info,
             pipeline_selector_from_graphql(pipeline),
             parse_run_config_input(runConfigData or {}, raise_on_error=False),
         )
 
+    @capture_error
     def resolve_executionPlanOrError(
         self,
         graphene_info: ResolveInfo,
         pipeline: GraphenePipelineSelector,
         mode: str,
         runConfigData: Optional[Any] = None,  # custom scalar (GrapheneRunConfigData)
     ):
         return get_execution_plan(
             graphene_info,
             pipeline_selector_from_graphql(pipeline),
             parse_run_config_input(runConfigData or {}, raise_on_error=True),  # type: ignore  # (possible str)
         )
 
+    @capture_error
     def resolve_runConfigSchemaOrError(
         self,
         graphene_info: ResolveInfo,
         selector: GraphenePipelineSelector,
         mode: Optional[str] = None,
     ):
         return resolve_run_config_schema_or_error(
@@ -837,14 +865,15 @@
             for node in results
         ]
 
     def resolve_assetNodeOrError(self, graphene_info: ResolveInfo, assetKey: GrapheneAssetKeyInput):
         asset_key_input = cast(Mapping[str, Sequence[str]], assetKey)
         return get_asset_node(graphene_info, AssetKey.from_graphql_input(asset_key_input))
 
+    @capture_error
     def resolve_assetsOrError(
         self,
         graphene_info: ResolveInfo,
         prefix: Optional[Sequence[str]] = None,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
     ):
@@ -864,17 +893,19 @@
         assetKeys: Optional[Sequence[GrapheneAssetKeyInput]] = None,
     ):
         assert assetKeys is not None
         raw_asset_keys = cast(Sequence[Mapping[str, Sequence[str]]], assetKeys)
         asset_keys = set(AssetKey.from_graphql_input(asset_key) for asset_key in raw_asset_keys)
         return get_asset_node_definition_collisions(graphene_info, asset_keys)
 
+    @capture_error
     def resolve_partitionBackfillOrError(self, graphene_info: ResolveInfo, backfillId: str):
         return get_backfill(graphene_info, backfillId)
 
+    @capture_error
     def resolve_partitionBackfillsOrError(
         self,
         graphene_info: ResolveInfo,
         status: Optional[GrapheneBulkActionStatus] = None,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
     ):
@@ -902,14 +933,15 @@
             node.external_asset_node.asset_key: node.external_asset_node.op_names
             for node in results
             if node.assetKey in asset_keys
         }
 
         return get_assets_latest_info(graphene_info, step_keys_by_asset)
 
+    @capture_error
     def resolve_logsForRun(
         self,
         graphene_info: ResolveInfo,
         runId: str,
         afterCursor: Optional[str] = None,
         limit: Optional[int] = None,
     ):
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/run_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import graphene
 from dagster._config.snap import ConfigSchemaSnapshot
 from dagster._core.host_representation import RepresentedJob
 from dagster._core.host_representation.external_data import DEFAULT_MODE_NAME
 from dagster._core.snap.snap_to_yaml import default_values_yaml_from_type_snap
 
 from ..implementation.run_config_schema import resolve_is_run_config_valid
+from ..implementation.utils import capture_error
 from .config_types import GrapheneConfigType, to_config_type
 from .errors import (
     GrapheneInvalidSubsetError,
     GrapheneModeNotFoundError,
     GraphenePipelineNotFoundError,
     GraphenePythonError,
 )
@@ -80,14 +81,15 @@
         return to_config_type(
             self._represented_job.config_schema_snapshot,
             self._represented_job.get_mode_def_snap(  # type: ignore  # (possible none)
                 self._mode or DEFAULT_MODE_NAME
             ).root_config_key,
         )
 
+    @capture_error
     def resolve_isRunConfigValid(
         self,
         graphene_info: ResolveInfo,
         runConfigData: Optional[Any] = None,  # custom scalar (GrapheneRunConfigData)
     ):
         return resolve_is_run_config_valid(
             graphene_info,
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/schedules/schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         super().__init__(
             name=external_schedule.name,
             cron_schedule=str(
                 external_schedule.cron_schedule
             ),  # can be sequence, coercing to str for now
             pipeline_name=external_schedule.job_name,
-            solid_selection=external_schedule.solid_selection,
+            solid_selection=external_schedule.op_selection,
             mode=external_schedule.mode,
             execution_timezone=(
                 self._external_schedule.execution_timezone
                 if self._external_schedule.execution_timezone
                 else "UTC"
             ),
             description=external_schedule.description,
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def __init__(self, external_target: ExternalTargetData):
         self._external_target = check.inst_param(
             external_target, "external_target", ExternalTargetData
         )
         super().__init__(
             pipelineName=external_target.job_name,
             mode=external_target.mode,
-            solidSelection=external_target.solid_selection,
+            solidSelection=external_target.op_selection,
         )
 
 
 class GrapheneSensorMetadata(graphene.ObjectType):
     assetKeys = graphene.List(graphene.NonNull(GrapheneAssetKey))
 
     class Meta:
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.5/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.5/dagster_graphql/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,38 +156,38 @@
         "repositoryName": repository.name,
     }
 
 
 def infer_job_or_pipeline_selector(
     graphql_context: WorkspaceRequestContext,
     pipeline_name: str,
-    solid_selection: Optional[Sequence[str]] = None,
+    op_selection: Optional[Sequence[str]] = None,
     asset_selection: Optional[Sequence[GqlAssetKey]] = None,
 ) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update(
         {
             "pipelineName": pipeline_name,
-            "solidSelection": solid_selection,
+            "solidSelection": op_selection,
             "assetSelection": asset_selection,
         }
     )
     return selector
 
 
 def infer_pipeline_selector(
     graphql_context: WorkspaceRequestContext,
     pipeline_name: str,
-    solid_selection: Optional[Sequence[str]] = None,
+    op_selection: Optional[Sequence[str]] = None,
 ) -> Selector:
     selector = infer_repository_selector(graphql_context)
     selector.update(
         {
             "pipelineName": pipeline_name,
-            "solidSelection": solid_selection,
+            "solidSelection": op_selection,
         }
     )
     return selector
 
 
 def infer_schedule_selector(
     graphql_context: WorkspaceRequestContext, schedule_name: str
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.5/dagster_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.4
+Version: 1.3.5
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.4/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.5/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.4/setup.py` & `dagster-graphql-1.3.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.4",
+        "dagster==1.3.5",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

