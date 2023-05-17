# Comparing `tmp/covalent-0.221.1rc0.tar.gz` & `tmp/covalent-0.222.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-0.221.1rc0.tar", last modified: Thu Apr 27 23:01:09 2023, max compression
+gzip compressed data, was "covalent-0.222.0rc0.tar", last modified: Wed May 17 15:47:03 2023, max compression
```

## Comparing `covalent-0.221.1rc0.tar` & `covalent-0.222.0rc0.tar`

### file list

```diff
@@ -1,271 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.593279 covalent-0.221.1rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-27 23:01:09.593279 covalent-0.221.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.553279 covalent-0.221.1rc0/covalent/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.557279 covalent-0.221.1rc0/covalent/_data_store/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_data_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.557279 covalent-0.221.1rc0/covalent/_data_store/storage_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_data_store/storage_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_data_store/storage_backends/localstoragebackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_data_store/storage_backends/storagebackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.557279 covalent-0.221.1rc0/covalent/_dispatcher_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_dispatcher_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_dispatcher_plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_dispatcher_plugins/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.561279 covalent-0.221.1rc0/covalent/_file_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.561279 covalent-0.221.1rc0/covalent/_file_transfer/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/strategies/http_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/strategies/rsync_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/strategies/s3_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.561279 covalent-0.221.1rc0/covalent/_results_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_results_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_results_manager/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_results_manager/results_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_results_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_results_manager/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.561279 covalent-0.221.1rc0/covalent/_shared_files/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/util_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_shared_files/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent/_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/depsbash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/depscall.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/depspip.py
--rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/lepton.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/transport_graph_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/_workflow/transportable_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent/executor/
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23966 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent/executor/executor_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/executor_plugins/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/executor_plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/executor_plugins/remote_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent/executor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/executor/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent/leptons/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/leptons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/triggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/triggers/dir_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/triggers/time_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent/triggers/trigger_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.557279 covalent-0.221.1rc0/covalent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 23:01:09.000000 covalent-0.221.1rc0/covalent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/_cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_cli/groups/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/_core/data_modules/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/data_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/data_modules/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/_core/runner_modules/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/runner_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.565279 covalent-0.221.1rc0/covalent_dispatcher/_db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/dispatchdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_db/write_result_to_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_dispatcher/_service/
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_service/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_service/app_dask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_dispatcher/_triggers_app/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_triggers_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/_triggers_app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_dispatcher/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/versions/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/versions/26d71848a404_v12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/versions/97202f5f47cb_v13.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/versions/9b9d58f02985_v11.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/versions/b60c5ecdf927_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/electron_dal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/graph_dal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/lattice_dal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/logs_dal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/summary_dal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/v1/database/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/v1/database/config/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/config/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/electron_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/lattices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.569279 covalent-0.221.1rc0/covalent_ui/api/v1/models/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/dispatch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/electrons_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/graph_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/lattices_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/logs_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/models/settings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.573279 covalent-0.221.1rc0/covalent_ui/api/v1/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.573279 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/graph_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/logs_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/routes/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.573279 covalent-0.221.1rc0/covalent_ui/api/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/utils/file_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/utils/file_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/utils/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/utils/models_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/api/v1/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-27 22:57:03.000000 covalent-0.221.1rc0/covalent_ui/result_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.549279 covalent-0.221.1rc0/covalent_ui/webapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.573279 covalent-0.221.1rc0/covalent_ui/webapp/build/
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/favicon64x64.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/logo192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    29252 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/logo512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/logo64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 22:58:10.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.553279 covalent-0.221.1rc0/covalent_ui/webapp/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.573279 covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.589279 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)  2724726 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  9525024 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   307919 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   675742 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   312555 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   826288 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js
--rw-r--r--   0 runner    (1001) docker     (123)    15931 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:01:09.593279 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/back.c0aa0e78.svg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/close.2a867415.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/download.d767a1c5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/exit.a2c5304b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/loader.7df2c6ef.svg
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/logs.551f3d28.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/sublattice.f6ee1fb5.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/zoom-in.f2603f36.svg
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 23:01:07.000000 covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/zoom-out.24dd0db1.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-27 22:57:04.000000 covalent-0.221.1rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-27 22:57:04.000000 covalent-0.221.1rc0/requirements-client.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 22:57:04.000000 covalent-0.221.1rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:01:09.593279 covalent-0.221.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-27 22:57:04.000000 covalent-0.221.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.388189 covalent-0.222.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-17 15:47:03.388189 covalent-0.222.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/_data_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_data_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/_data_store/storage_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_data_store/storage_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_data_store/storage_backends/localstoragebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_data_store/storage_backends/storagebackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/_dispatcher_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_dispatcher_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_dispatcher_plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_dispatcher_plugins/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/_file_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/_file_transfer/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/strategies/http_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/strategies/rsync_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/strategies/s3_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent/_results_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_results_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_results_manager/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_results_manager/results_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_results_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_results_manager/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/_shared_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/util_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_shared_files/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/depsbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/depscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/depspip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/lepton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/transport_graph_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/_workflow/transportable_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/cloud_resource_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/cloud_resource_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/cloud_resource_manager/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23966 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/executor/executor_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/executor_plugins/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/executor_plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/executor_plugins/remote_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/executor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/executor/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/leptons/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/leptons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/triggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/triggers/dir_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/triggers/time_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent/triggers/trigger_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 15:47:03.000000 covalent-0.222.0rc0/covalent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.356189 covalent-0.222.0rc0/covalent_dispatcher/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_cli/groups/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_core/data_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/data_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/data_modules/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_core/runner_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/runner_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/dispatchdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_db/write_result_to_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_service/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_service/app_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_dispatcher/_triggers_app/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_triggers_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/_triggers_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_dispatcher/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/versions/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/versions/26d71848a404_v12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/versions/97202f5f47cb_v13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/versions/9b9d58f02985_v11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/versions/b60c5ecdf927_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_ui/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.360189 covalent-0.222.0rc0/covalent_ui/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/electron_dal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/graph_dal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/lattice_dal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/logs_dal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/summary_dal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/database/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/config/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/electron_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/lattices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/dispatch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/electrons_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/graph_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/lattices_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/logs_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/models/settings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/graph_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/logs_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/routes/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.364189 covalent-0.222.0rc0/covalent_ui/api/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/utils/file_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/utils/file_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/utils/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/utils/models_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/api/v1/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/covalent_ui/result_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent_ui/webapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.368189 covalent-0.222.0rc0/covalent_ui/webapp/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/favicon64x64.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/logo192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29252 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/logo512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/logo64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 15:44:11.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.352189 covalent-0.222.0rc0/covalent_ui/webapp/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.368189 covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.384189 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  2724726 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  9525024 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   307919 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   675742 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   312555 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   826288 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15931 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:03.388189 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/back.c0aa0e78.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/close.2a867415.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/download.d767a1c5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/exit.a2c5304b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/loader.7df2c6ef.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/logs.551f3d28.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/sublattice.f6ee1fb5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/zoom-in.f2603f36.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 15:47:01.000000 covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/zoom-out.24dd0db1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:47:03.388189 covalent-0.222.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-17 15:43:07.000000 covalent-0.222.0rc0/setup.py
```

### Comparing `covalent-0.221.1rc0/LICENSE` & `covalent-0.222.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/PKG-INFO` & `covalent-0.222.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent
-Version: 0.221.1rc0
+Version: 0.222.0rc0
 Summary: Covalent Workflow Tool
 Home-page: https://github.com/AgnostiqHQ/covalent
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.221.1-rc.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.222.0-rc.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="https://raw.githubusercontent.com/AgnostiqHQ/covalent/master/doc/source/_static/covalent_readme_banner.svg" width=150%>
         
         [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/covalent?color=navy&include_prereleases&label=version&sort=semver)](https://github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md)
```

### Comparing `covalent-0.221.1rc0/README.md` & `covalent-0.222.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/__init__.py` & `covalent-0.222.0rc0/covalent/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_data_store/__init__.py` & `covalent-0.222.0rc0/covalent/_data_store/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_data_store/storage_backends/__init__.py` & `covalent-0.222.0rc0/covalent/_data_store/storage_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_data_store/storage_backends/localstoragebackend.py` & `covalent-0.222.0rc0/covalent/_data_store/storage_backends/localstoragebackend.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_data_store/storage_backends/storagebackend.py` & `covalent-0.222.0rc0/covalent/_data_store/storage_backends/storagebackend.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_dispatcher_plugins/__init__.py` & `covalent-0.222.0rc0/covalent/_dispatcher_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_dispatcher_plugins/base.py` & `covalent-0.222.0rc0/covalent/_dispatcher_plugins/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_dispatcher_plugins/local.py` & `covalent-0.222.0rc0/covalent/_dispatcher_plugins/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,19 @@
             Returns:
                 The dispatch id of the workflow.
             """
 
             # To access the disable_run passed to the dispatch function
             nonlocal disable_run
 
+            if not isinstance(orig_lattice, Lattice):
+                message = f"Dispatcher expected a Lattice, received {type(orig_lattice)} instead."
+                app_log.error(message)
+                raise TypeError(message)
+
             lattice = deepcopy(orig_lattice)
 
             lattice.build_graph(*args, **kwargs)
 
             # Serialize the transport graph to JSON
             json_lattice = lattice.serialize_to_json()
 
@@ -137,20 +142,25 @@
                 # Determine whether to disable first run based on trigger_data
                 disable_run = triggers_data is not None
 
             json_lattice = json.dumps(json_lattice)
 
             submit_dispatch_url = f"{dispatcher_addr}/api/submit"
 
-            r = requests.post(
-                submit_dispatch_url, data=json_lattice, params={"disable_run": disable_run}
-            )
-            r.raise_for_status()
-
-            lattice_dispatch_id = r.content.decode("utf-8").strip().replace('"', "")
+            lattice_dispatch_id = None
+            try:
+                r = requests.post(
+                    submit_dispatch_url, data=json_lattice, params={"disable_run": disable_run}
+                )
+                r.raise_for_status()
+                lattice_dispatch_id = r.content.decode("utf-8").strip().replace('"', "")
+            except requests.exceptions.ConnectionError as e:
+                message = f"The Covalent dispatcher server is not running at {dispatcher_addr}. You must start Covalent (with `covalent start`) before dispatching your workflow."
+                app_log.error(message)
+                raise ConnectionError(message) from e
 
             if not disable_run or triggers_data is None:
                 return lattice_dispatch_id
 
             LocalDispatcher.register_triggers(triggers_data, lattice_dispatch_id)
 
             return lattice_dispatch_id
```

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/__init__.py` & `covalent-0.222.0rc0/covalent/_file_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/enums.py` & `covalent-0.222.0rc0/covalent/_file_transfer/enums.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/file.py` & `covalent-0.222.0rc0/covalent/_file_transfer/file.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/file_transfer.py` & `covalent-0.222.0rc0/covalent/_file_transfer/file_transfer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/folder.py` & `covalent-0.222.0rc0/covalent/_file_transfer/folder.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/strategies/__init__.py` & `covalent-0.222.0rc0/covalent/_file_transfer/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/strategies/http_strategy.py` & `covalent-0.222.0rc0/covalent/_file_transfer/strategies/http_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/strategies/rsync_strategy.py` & `covalent-0.222.0rc0/covalent/_file_transfer/strategies/rsync_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/strategies/s3_strategy.py` & `covalent-0.222.0rc0/covalent/_file_transfer/strategies/s3_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py` & `covalent-0.222.0rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_results_manager/__init__.py` & `covalent-0.222.0rc0/covalent/_results_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_results_manager/result.py` & `covalent-0.222.0rc0/covalent/_results_manager/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_results_manager/results_manager.py` & `covalent-0.222.0rc0/covalent/_results_manager/results_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_results_manager/utils.py` & `covalent-0.222.0rc0/covalent/_results_manager/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_results_manager/wait.py` & `covalent-0.222.0rc0/covalent/_results_manager/wait.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/__init__.py` & `covalent-0.222.0rc0/covalent/_shared_files/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/config.py` & `covalent-0.222.0rc0/covalent/_shared_files/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,14 @@
             self.update_config()
         except FileNotFoundError:
             Path(self.config_file).parent.mkdir(parents=True, exist_ok=True)
             self.write_config()
 
         Path(self.get("sdk.log_dir")).mkdir(parents=True, exist_ok=True)
         Path(self.get("sdk.executor_dir")).mkdir(parents=True, exist_ok=True)
-        Path(self.get("dispatcher.cache_dir")).mkdir(parents=True, exist_ok=True)
-        Path(self.get("dispatcher.results_dir")).mkdir(parents=True, exist_ok=True)
-        Path(self.get("dispatcher.log_dir")).mkdir(parents=True, exist_ok=True)
-        Path(self.get("user_interface.log_dir")).mkdir(parents=True, exist_ok=True)
         Path(self.get("dispatcher.db_path")).parent.mkdir(parents=True, exist_ok=True)
 
     def generate_default_config(self) -> None:
         """
         Load the default configuration into memory.
 
         Args:
@@ -279,15 +275,15 @@
     """
     Read the configuration from the TOML file and append to default
         (or existing) configuration. Optionally, update configuration
         data with an input dict.
 
     Args:
         new_entries: Dictionary of new entries added or updated in the config
-        defaults: If False (which is the default), default values do not overwrite
+        override_existing: If True (which is the default), default values overwrite
             existing entries.
 
     Returns:
         None
     """
     cm = ConfigManager()
     cm.update_config(new_entries, override_existing)
```

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/context_managers.py` & `covalent-0.222.0rc0/covalent/_shared_files/context_managers.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/defaults.py` & `covalent-0.222.0rc0/covalent/_shared_files/defaults.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/exceptions.py` & `covalent-0.222.0rc0/covalent_dispatcher/_cli/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,18 +14,9 @@
 #
 # Covalent is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the License for more details.
 #
 # Relief from the License may be granted by purchasing a commercial license.
 
-
-class MissingLatticeRecordError(Exception):
-    pass
-
-
-class TaskRuntimeError(Exception):
-    pass
-
-
-class TaskCancelledError(Exception):
-    pass
+"""Import CLI tool functionalities."""
+from .service import _is_server_running
```

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/logger.py` & `covalent-0.222.0rc0/covalent/_shared_files/logger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/metrics.py` & `covalent-0.222.0rc0/covalent/_shared_files/metrics.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/util_classes.py` & `covalent-0.222.0rc0/covalent/_shared_files/util_classes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_shared_files/utils.py` & `covalent-0.222.0rc0/covalent/_shared_files/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,27 @@
 
 import inspect
 import socket
 from datetime import timedelta
 from typing import Callable, Dict, Set, Tuple
 
 from . import logger
+from .config import get_config
 
 app_log = logger.app_log
 log_stack_info = logger.log_stack_info
 
+DEFAULT_UI_ADDRESS = get_config("user_interface.address")
+DEFAULT_UI_PORT = get_config("user_interface.port")
+
+
+def get_ui_url(path):
+    baseUrl = f"http://{DEFAULT_UI_ADDRESS}:{DEFAULT_UI_PORT}"
+    return f"{baseUrl}{path}"
+
 
 def get_random_available_port() -> int:
     """
     Return a random port that is available on the machine
     """
     sock = socket.socket()
     sock.bind(("127.0.0.1", 0))
```

### Comparing `covalent-0.221.1rc0/covalent/_workflow/__init__.py` & `covalent-0.222.0rc0/covalent/_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/deps.py` & `covalent-0.222.0rc0/covalent/_workflow/deps.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/depsbash.py` & `covalent-0.222.0rc0/covalent/_workflow/depsbash.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/depscall.py` & `covalent-0.222.0rc0/covalent/_workflow/depscall.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/depspip.py` & `covalent-0.222.0rc0/covalent/_workflow/depspip.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/electron.py` & `covalent-0.222.0rc0/covalent/_workflow/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/lattice.py` & `covalent-0.222.0rc0/covalent/_workflow/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 # Relief from the License may be granted by purchasing a commercial license.
 
 """Class corresponding to computation workflow."""
 
 import json
 import os
 import warnings
+import webbrowser
 from builtins import list
 from contextlib import redirect_stdout
 from copy import deepcopy
 from dataclasses import asdict
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, Union
 
 from .._shared_files import logger
 from .._shared_files.config import get_config
 from .._shared_files.context_managers import active_lattice_manager
 from .._shared_files.defaults import DefaultMetadataValues
-from .._shared_files.utils import get_named_params, get_serialized_function_str
+from .._shared_files.utils import get_named_params, get_serialized_function_str, get_ui_url
 from .depsbash import DepsBash
 from .depscall import DepsCall
 from .depspip import DepsPip
 from .postprocessing import Postprocessor
 from .transport import TransportableObject, _TransportGraph, encode_metadata
 
 if TYPE_CHECKING:
@@ -266,14 +267,19 @@
             None
         """
 
         import covalent_ui.result_webhook as result_webhook
 
         self.build_graph(*args, **kwargs)
         result_webhook.send_draw_request(self)
+        draw_preview_url = get_ui_url("/preview")
+        message = f"To preview the transport graph of the lattice, visit {draw_preview_url}"
+        app_log.info(message)
+        print(message)
+        webbrowser.open(draw_preview_url)
 
     def __call__(self, *args, **kwargs):
         """Execute lattice as an ordinary function for testing purposes."""
 
         workflow_function = self.workflow_function.get_deserialized()
         return workflow_function(*args, **kwargs)
```

### Comparing `covalent-0.221.1rc0/covalent/_workflow/lepton.py` & `covalent-0.222.0rc0/covalent/_workflow/lepton.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/postprocessing.py` & `covalent-0.222.0rc0/covalent/_workflow/postprocessing.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/transport.py` & `covalent-0.222.0rc0/covalent/_workflow/transport.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/transport_graph_ops.py` & `covalent-0.222.0rc0/covalent/_workflow/transport_graph_ops.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/_workflow/transportable_object.py` & `covalent-0.222.0rc0/covalent/_workflow/transportable_object.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/__init__.py` & `covalent-0.222.0rc0/covalent/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/base.py` & `covalent-0.222.0rc0/covalent/executor/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/executor_plugins/dask.py` & `covalent-0.222.0rc0/covalent/executor/executor_plugins/dask.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/executor_plugins/local.py` & `covalent-0.222.0rc0/covalent/executor/executor_plugins/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/executor_plugins/remote_executor.py` & `covalent-0.222.0rc0/covalent/executor/executor_plugins/remote_executor.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/utils/__init__.py` & `covalent-0.222.0rc0/covalent/executor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/executor/utils/wrappers.py` & `covalent-0.222.0rc0/covalent/executor/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/leptons/__init__.py` & `covalent-0.222.0rc0/covalent/leptons/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/triggers/__init__.py` & `covalent-0.222.0rc0/covalent/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/triggers/base.py` & `covalent-0.222.0rc0/covalent/triggers/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/triggers/dir_trigger.py` & `covalent-0.222.0rc0/covalent/triggers/dir_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/triggers/time_trigger.py` & `covalent-0.222.0rc0/covalent/triggers/time_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent/triggers/trigger_loader.py` & `covalent-0.222.0rc0/covalent/triggers/trigger_loader.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent.egg-info/PKG-INFO` & `covalent-0.222.0rc0/covalent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent
-Version: 0.221.1rc0
+Version: 0.222.0rc0
 Summary: Covalent Workflow Tool
 Home-page: https://github.com/AgnostiqHQ/covalent
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.221.1-rc.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.222.0-rc.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         <img src="https://raw.githubusercontent.com/AgnostiqHQ/covalent/master/doc/source/_static/covalent_readme_banner.svg" width=150%>
         
         [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/covalent?color=navy&include_prereleases&label=version&sort=semver)](https://github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md)
```

### Comparing `covalent-0.221.1rc0/covalent.egg-info/SOURCES.txt` & `covalent-0.222.0rc0/covalent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 covalent/_workflow/electron.py
 covalent/_workflow/lattice.py
 covalent/_workflow/lepton.py
 covalent/_workflow/postprocessing.py
 covalent/_workflow/transport.py
 covalent/_workflow/transport_graph_ops.py
 covalent/_workflow/transportable_object.py
+covalent/cloud_resource_manager/__init__.py
+covalent/cloud_resource_manager/core.py
 covalent/executor/__init__.py
 covalent/executor/base.py
 covalent/executor/executor_plugins/dask.py
 covalent/executor/executor_plugins/local.py
 covalent/executor/executor_plugins/remote_executor.py
 covalent/executor/utils/__init__.py
 covalent/executor/utils/wrappers.py
```

### Comparing `covalent-0.221.1rc0/covalent.egg-info/requires.txt` & `covalent-0.222.0rc0/covalent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/__init__.py` & `covalent-0.222.0rc0/covalent_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_cli/__init__.py` & `covalent-0.222.0rc0/covalent/cloud_resource_manager/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Agnostiq Inc.
+# Copyright 2023 Agnostiq Inc.
 #
 # This file is part of Covalent.
 #
 # Licensed under the GNU Affero General Public License 3.0 (the "License").
 # A copy of the License may be obtained with this software package or at
 #
 #      https://www.gnu.org/licenses/agpl-3.0.en.html
@@ -14,9 +14,8 @@
 #
 # Covalent is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the License for more details.
 #
 # Relief from the License may be granted by purchasing a commercial license.
 
-"""Import CLI tool functionalities."""
-from .service import _is_server_running
+from .core import CloudResourceManager
```

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_cli/cli.py` & `covalent-0.222.0rc0/covalent_dispatcher/_cli/cli.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_cli/groups/__init__.py` & `covalent-0.222.0rc0/covalent_dispatcher/_cli/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_cli/groups/db.py` & `covalent-0.222.0rc0/covalent_dispatcher/_cli/groups/db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_cli/migrate.py` & `covalent-0.222.0rc0/covalent_dispatcher/_cli/migrate.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_cli/service.py` & `covalent-0.222.0rc0/covalent_dispatcher/_cli/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import asyncio
 import contextlib
 import json
 import os
 import shutil
 import socket
 import time
+from pathlib import Path
 from subprocess import DEVNULL, Popen
 from typing import Optional
 
 import click
 import dask.system
 import psutil
 import requests
@@ -215,14 +216,20 @@
         except requests.exceptions.ConnectionError as err:
             time.sleep(1)
 
     if triggers_only:
         click.echo(f"Covalent Triggers server has started at {dispatcher_addr}")
     else:
         click.echo(f"Covalent server has started at {dispatcher_addr}")
+
+    Path(get_config("dispatcher.cache_dir")).mkdir(parents=True, exist_ok=True)
+    Path(get_config("dispatcher.results_dir")).mkdir(parents=True, exist_ok=True)
+    Path(get_config("dispatcher.log_dir")).mkdir(parents=True, exist_ok=True)
+    Path(get_config("user_interface.log_dir")).mkdir(parents=True, exist_ok=True)
+
     return port
 
 
 def _terminate_child_processes(pid: int) -> None:
     """For a given process, find all the child processes and terminate them.
 
     Args:
```

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/__init__.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/data_manager.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/data_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/data_modules/__init__.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/data_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/data_modules/job_manager.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/data_modules/job_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/dispatcher.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/execution.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/execution.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/runner.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     executor: Any,
 ) -> None:
     # Resolve abstract task and inputs to their concrete (serialized) values
     result_object = datasvc.get_result_object(dispatch_id)
     timestamp = datetime.now(timezone.utc)
 
     try:
-        cancel_req = await _get_cancel_requested(dispatch_id, node_id)
+        cancel_req = await executor_proxy._get_cancel_requested(dispatch_id, node_id)
         if cancel_req:
             app_log.debug(f"Don't run cancelled task {dispatch_id}:{node_id}")
             return datasvc.generate_node_result(
                 node_id=node_id,
                 node_name=node_name,
                 start_time=timestamp,
                 end_time=timestamp,
@@ -414,22 +414,7 @@
 
     Return(s)
         List of node metadata for the given `node_ids`
     """
     res = datasvc.get_result_object(dispatch_id)
     tg = res.lattice.transport_graph
     return list(map(lambda x: tg.get_node_value(x, "metadata"), node_ids))
-
-
-async def _get_cancel_requested(dispatch_id: str, task_id: int) -> Any:
-    """
-    Query if a specific task has been requested to be cancelled
-
-    Arg(s)
-        dispatch_id: Dispatch ID of the workflow
-        task_id: ID of the node to be cancelled
-
-    Return(s)
-        Whether the task has been requested to be cancelled or not
-    """
-    records = await get_jobs_metadata(dispatch_id, [task_id])
-    return records[0]["cancel_requested"]
```

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/runner_modules/__init__.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/runner_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py` & `covalent-0.222.0rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/datastore.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/datastore.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/dispatchdb.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/dispatchdb.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/jobdb.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/jobdb.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/load.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/load.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/models.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/models.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/update.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/update.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/upsert.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/upsert.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_db/write_result_to_db.py` & `covalent-0.222.0rc0/covalent_dispatcher/_db/write_result_to_db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_service/app.py` & `covalent-0.222.0rc0/covalent_dispatcher/_service/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_service/app_dask.py` & `covalent-0.222.0rc0/covalent_dispatcher/_service/app_dask.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+# Copyright 2023 Agnostiq Inc.
+#
+# This file is part of Covalent.
+#
+# Licensed under the GNU Affero General Public License 3.0 (the "License").
+# A copy of the License may be obtained with this software package or at
+#
+#      https://www.gnu.org/licenses/agpl-3.0.en.html
+#
+# Use of this file is prohibited except in compliance with the License. Any
+# modifications or derivative works of this file must retain this copyright
+# notice, and modified files must contain a notice indicating that they have
+# been altered from the originals.
+#
+# Covalent is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
+# FITNESS FOR A PARTICULAR PURPOSE. See the License for more details.
+#
+# Relief from the License may be granted by purchasing a commercial license.
+
 from __future__ import annotations
 
 import asyncio
 import os
 from logging import Logger
 from multiprocessing import Process, current_process
 from threading import Thread
@@ -187,15 +207,18 @@
         """
         Runs a local dask cluster along with its monitoring thread
         """
         try:
             self.cluster = LocalCluster(
                 n_workers=self.num_workers,
                 threads_per_worker=self.threads_per_worker,
-                **{"memory_limit": self.mem_per_worker},
+                **{
+                    "memory_limit": self.mem_per_worker,
+                    "local_directory": get_config("dispatcher.cache_dir"),
+                },
             )
         except Exception as e:
             self.logger.exception(e)
 
         scheduler_address = self.cluster.scheduler_address
         dashboard_link = self.cluster.dashboard_link
```

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_triggers_app/__init__.py` & `covalent-0.222.0rc0/covalent_dispatcher/_triggers_app/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/_triggers_app/app.py` & `covalent-0.222.0rc0/covalent_dispatcher/_triggers_app/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_dispatcher/entry_point.py` & `covalent-0.222.0rc0/covalent_dispatcher/entry_point.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/README.md` & `covalent-0.222.0rc0/covalent_migrations/README.md`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/alembic.ini` & `covalent-0.222.0rc0/covalent_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/env.py` & `covalent-0.222.0rc0/covalent_migrations/env.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/script.py.mako` & `covalent-0.222.0rc0/covalent_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/versions/26d71848a404_v12.py` & `covalent-0.222.0rc0/covalent_migrations/versions/26d71848a404_v12.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/versions/97202f5f47cb_v13.py` & `covalent-0.222.0rc0/covalent_migrations/versions/97202f5f47cb_v13.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/versions/9b9d58f02985_v11.py` & `covalent-0.222.0rc0/covalent_migrations/versions/9b9d58f02985_v11.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/versions/b60c5ecdf927_init.py` & `covalent-0.222.0rc0/covalent_migrations/versions/b60c5ecdf927_init.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py` & `covalent-0.222.0rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/main.py` & `covalent-0.222.0rc0/covalent_ui/api/main.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/electron_dal.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/electron_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/graph_dal.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/graph_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/lattice_dal.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/lattice_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/logs_dal.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/logs_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/data_layer/summary_dal.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/data_layer/summary_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/config/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/config/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/config/db.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/config/db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/electron.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/electron_dependency.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/electron_dependency.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/database/schema/lattices.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/database/schema/lattices.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/dispatch_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/dispatch_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/electrons_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/electrons_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/file_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/file_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/graph_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/graph_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/lattices_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/lattices_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/logs_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/logs_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/models/settings_model.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/models/settings_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/graph_route.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/graph_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/logs_route.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/logs_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/routes/routes.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/routes/routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/utils/__init__.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/utils/file_handle.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/utils/file_handle.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/utils/file_name.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/utils/file_name.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/utils/log_handler.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/utils/models_helper.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/utils/models_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/api/v1/utils/status.py` & `covalent-0.222.0rc0/covalent_ui/api/v1/utils/status.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/app.py` & `covalent-0.222.0rc0/covalent_ui/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/result_webhook.py` & `covalent-0.222.0rc0/covalent_ui/result_webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,22 @@
 
 import aiohttp
 import requests
 
 import covalent_ui.app as ui_server
 from covalent._results_manager import Result
 from covalent._shared_files import logger
-from covalent._shared_files.config import get_config
+from covalent._shared_files.utils import get_ui_url
 from covalent_dispatcher._db.dispatchdb import encode_dict, extract_graph, extract_metadata
 
-DEFAULT_PORT = get_config("user_interface.port")
-
 app_log = logger.app_log
 
 # UI server webhook for result updates
 
 
-def get_ui_url(path):
-    baseUrl = f"http://localhost:{DEFAULT_PORT}"
-    return f"{baseUrl}{path}"
-
-
 async def send_update(result: Result) -> None:
     """
     Signal UI server about a result update. Note that the server will expect the
     updated result to have been saved to the results directory prior to the
     update.
 
     Args: result: The updated result object.
```

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/asset-manifest.json` & `covalent-0.222.0rc0/covalent_ui/webapp/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/favicon.ico` & `covalent-0.222.0rc0/covalent_ui/webapp/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/favicon64x64.ico` & `covalent-0.222.0rc0/covalent_ui/webapp/build/favicon64x64.ico`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/index.html` & `covalent-0.222.0rc0/covalent_ui/webapp/build/index.html`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/logo192x192.png` & `covalent-0.222.0rc0/covalent_ui/webapp/build/logo192x192.png`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/logo512x512.png` & `covalent-0.222.0rc0/covalent_ui/webapp/build/logo512x512.png`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/logo64x64.png` & `covalent-0.222.0rc0/covalent_ui/webapp/build/logo64x64.png`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/css/main.44ddb339.chunk.css.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.LICENSE.txt` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/2.a5457a17.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/3.db864693.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/4.37ca7cf4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/main.9eb5cdc8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js.map` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/js/runtime-main.d303549c.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/loader.7df2c6ef.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/loader.7df2c6ef.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg` & `covalent-0.222.0rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/pyproject.toml` & `covalent-0.222.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-0.221.1rc0/setup.py` & `covalent-0.222.0rc0/setup.py`

 * *Files identical despite different names*

