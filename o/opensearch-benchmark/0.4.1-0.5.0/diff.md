# Comparing `tmp/opensearch-benchmark-0.4.1.tar.gz` & `tmp/opensearch-benchmark-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-benchmark-0.4.1.tar", last modified: Thu Apr 27 22:59:58 2023, max compression
+gzip compressed data, was "opensearch-benchmark-0.5.0.tar", last modified: Thu May 18 21:29:21 2023, max compression
```

## Comparing `opensearch-benchmark-0.4.1.tar` & `opensearch-benchmark-0.5.0.tar`

### file list

```diff
@@ -1,312 +1,314 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.735031 opensearch-benchmark-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-27 22:59:58.735031 opensearch-benchmark-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.707031 opensearch-benchmark-0.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.707031 opensearch-benchmark-0.4.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/client-options.md
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/execute-test.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/kill-running-process.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/target-hosts.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/test-mode.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/api/workload.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/get-started.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.707031 opensearch-benchmark-0.4.1/docs/user-guides/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/user-guides/create-pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/docs/user-guides/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.711031 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 22:59:58.000000 opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.711031 opensearch-benchmark-0.4.1/osbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/async_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    49684 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/benchmarkd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31285 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/cluster_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/listers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/configs/utils/config_path_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/builders/binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/builders/source_binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/opensearch_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/executors/exception_handling_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/executors/local_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/executors/shell_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/bare_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/docker_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/exception_handling_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.715031 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/opensearch_preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/plugin_preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/java_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.719031 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/docker_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/exception_handling_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/local_process_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/no_op_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.719031 opensearch-benchmark-0.4.1/osbenchmark/builder/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/architecture_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/bootstrap_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/cluster_flavors.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/cluster_infra_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/host.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/plugin_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/provision_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/provision_config_instance_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/models/provision_config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/provision_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.719031 opensearch-benchmark-0.4.1/osbenchmark/builder/provisioners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/provisioners/provisioner.py
--rw-r--r--   0 runner    (1001) docker     (123)    34133 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/supplier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.719031 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/artifact_variables_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/binary_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/config_applier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/git_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/host_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/java_home_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/jdk_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/path_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/builder/utils/template_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    77539 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/chart_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    88571 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/min-os-version.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/benchmark.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/logging.json
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/metrics-template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.699031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.723031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.727031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.703031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.707031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/results-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/test-executions-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/workload-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/resources/workload.json.j2
--rw-r--r--   0 runner    (1001) docker     (123)    34843 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/results_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    76561 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18757 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/test_execution_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/periodic_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/sysstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89687 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    97801 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/worker_coordinator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.731031 opensearch-benchmark-0.4.1/osbenchmark/workload/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79356 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    36839 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.735031 opensearch-benchmark-0.4.1/osbenchmark/workload_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload_generator/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload_generator/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/osbenchmark/workload_generator/workload_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.735031 opensearch-benchmark-0.4.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10512 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/scripts/expand-data-corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-27 22:59:58.735031 opensearch-benchmark-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:59:58.735031 opensearch-benchmark-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/tests/test_async_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/tests/test_execution_orchestrator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 22:58:46.000000 opensearch-benchmark-0.4.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/client-options.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/execute-test.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/kill-running-process.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/target-hosts.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/test-mode.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/workload.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/get-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/docs/user-guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/user-guides/create-pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/user-guides/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:29:20.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50515 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/benchmarkd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31285 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/cluster_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/local_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/shell_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/bare_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/docker_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/exception_handling_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/java_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/docker_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/local_process_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/no_op_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/builder/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/architecture_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/bootstrap_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/cluster_flavors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/cluster_infra_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/plugin_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provision_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34133 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/artifact_variables_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/binary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/config_applier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/git_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/host_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/java_home_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/jdk_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/template_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77539 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/chart_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88571 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/min-os-version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/base-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/benchmark.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/custom-query-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/default-query-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/metrics-template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/results-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/test-executions-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/workload-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34843 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/results_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76561 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18757 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/test_execution_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/periodic_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/sysstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89687 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97801 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/worker_coordinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/osbenchmark/workload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79356 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55903 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37160 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/workload_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10512 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/scripts/expand-data-corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/tests/test_async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/tests/test_execution_orchestrator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/version.txt
```

### Comparing `opensearch-benchmark-0.4.1/AUTHORS` & `opensearch-benchmark-0.5.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/CONTRIBUTING.md` & `opensearch-benchmark-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/LICENSE` & `opensearch-benchmark-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/PKG-INFO` & `opensearch-benchmark-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-benchmark
-Version: 0.4.1
+Version: 0.5.0
 Summary: Macrobenchmarking framework for OpenSearch
 Home-page: https://github.com/opensearch-project/OpenSearch-Benchmark
 Maintainer: Ian Hoang, Govind Kamat
 Maintainer-email: hoangia@amazon.com, govkamat@amazon.com
 License: Apache License, Version 2.0
 Classifier: Topic :: System :: Benchmark
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,15 +63,15 @@
 If you have any trouble or need more detailed instructions, please look in the [detailed installation guide](<https://github.com/opensearch-project/OpenSearch-Benchmark/blob/main/DEVELOPER_GUIDE.md>).
 
 Run your first test execution
 -----------------------------
 
 Now we're ready to run our first test execution:
 
-    opensearch-benchmark execute_test --distribution-version=1.0.0 --workload=geonames --test-mode
+    opensearch-benchmark execute-test --distribution-version=1.0.0 --workload=geonames --test-mode
 
 This will download OpenSearch 1.0.0 and run one of OpenSearch Benchmark's official workloads - the [geonames workload](<https://github.com/opensearch-project/opensearch-benchmark-workloads/tree/main/geonames>) - against it.
 Note that this uses the `--test-mode` argument to only run a single instance of each operation in order to reduce the time needed for a test execution. This argument is used as a sanity check and should be removed in an actual benchmarking scenario.
 After the test execution, a summary report is written to the command line:
 
     ------------------------------------------------------
         _______             __   _____
@@ -127,14 +127,17 @@
     | 99.9th percentile service time |     painless_dynamic |   457.352 |     ms |
     |  100th percentile service time |     painless_dynamic |   459.474 |     ms |
 
     ----------------------------------
     [INFO] SUCCESS (took 2634 seconds)
     ----------------------------------
 
+Creating Your Own Workloads
+---------------------------
+For more information on how users can create their own workloads, see [the Create Workload Guide](./CREATE_WORKLOAD_GUIDE.md)
 
 Getting help
 ------------
 
 * Quick help: ``opensearch-benchmark --help``
 * Look in [OpenSearch Benchmark's user guide](<https://github.com/opensearch-project/OpenSearch-Benchmark/blob/main/DEVELOPER_GUIDE.md>) for more information
 * For any questions or answers, visit our [community forum](<https://discuss.opendistrocommunity.dev/>).
```

### Comparing `opensearch-benchmark-0.4.1/README.md` & `opensearch-benchmark-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 If you have any trouble or need more detailed instructions, please look in the [detailed installation guide](<https://github.com/opensearch-project/OpenSearch-Benchmark/blob/main/DEVELOPER_GUIDE.md>).
 
 Run your first test execution
 -----------------------------
 
 Now we're ready to run our first test execution:
 
-    opensearch-benchmark execute_test --distribution-version=1.0.0 --workload=geonames --test-mode
+    opensearch-benchmark execute-test --distribution-version=1.0.0 --workload=geonames --test-mode
 
 This will download OpenSearch 1.0.0 and run one of OpenSearch Benchmark's official workloads - the [geonames workload](<https://github.com/opensearch-project/opensearch-benchmark-workloads/tree/main/geonames>) - against it.
 Note that this uses the `--test-mode` argument to only run a single instance of each operation in order to reduce the time needed for a test execution. This argument is used as a sanity check and should be removed in an actual benchmarking scenario.
 After the test execution, a summary report is written to the command line:
 
     ------------------------------------------------------
         _______             __   _____
@@ -99,14 +99,17 @@
     | 99.9th percentile service time |     painless_dynamic |   457.352 |     ms |
     |  100th percentile service time |     painless_dynamic |   459.474 |     ms |
 
     ----------------------------------
     [INFO] SUCCESS (took 2634 seconds)
     ----------------------------------
 
+Creating Your Own Workloads
+---------------------------
+For more information on how users can create their own workloads, see [the Create Workload Guide](./CREATE_WORKLOAD_GUIDE.md)
 
 Getting help
 ------------
 
 * Quick help: ``opensearch-benchmark --help``
 * Look in [OpenSearch Benchmark's user guide](<https://github.com/opensearch-project/OpenSearch-Benchmark/blob/main/DEVELOPER_GUIDE.md>) for more information
 * For any questions or answers, visit our [community forum](<https://discuss.opendistrocommunity.dev/>).
```

### Comparing `opensearch-benchmark-0.4.1/docs/api/execute-test.md` & `opensearch-benchmark-0.5.0/docs/api/execute-test.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ---
 layout: default
 title: Execute Test
 parent: Benchmark API
 nav_order: 10
 ---
 
-The `execute_test` command of OpenSearch Benchmark executes tests against your OpenSearch cluster.
+The `execute-test` command of OpenSearch Benchmark executes tests against your OpenSearch cluster.
 
 
-## Syntax 
+## Syntax
 
 ```bash
-opensearch-benchmark execute_test <arguments>
+opensearch-benchmark execute-test <arguments>
 ```
 
 
 ### Common Arguments
 
 See [All Arguments](#all-arguments) for an exhaustive list of arguments
 
@@ -30,34 +30,34 @@
 `target-hosts` | The OpenSearch endpoint(s) to execute a test against. This should only be specified with  `--pipeline=benchmark-only`  | No
 `test-mode` | Run a single iteration of each operation in the test procedure. The test provides a quick way for sanity checking a testing configuration. Therefore, do not use `test-mode` for actual benchmarking. | No
 `kill-running-processes` | Kill any running OpenSearch Benchmark processes on the local machine before the test executes. | No
 
 *Example 1*
 
 ```
-opensearch-benchmark execute_test --workload eventdata --test-mode
+opensearch-benchmark execute-test --workload eventdata --test-mode
 ```
 
-Provision an OpenSearch node on the local machine based on the latest source code in Github and execute the `eventdata` workload in test mode. 
+Provision an OpenSearch node on the local machine based on the latest source code in Github and execute the `eventdata` workload in test mode.
 
 *Example 2*
 
 ```
-opensearch-benchmark execute_test --workload http_logs --pipeline benchmark-only --target-hosts <endpoint> --workload-params "bulk_indexing_clients:1,ingest_percentage:10"
+opensearch-benchmark execute-test --workload http_logs --pipeline benchmark-only --target-hosts <endpoint> --workload-params "bulk_indexing_clients:1,ingest_percentage:10"
 ```
 
-Execute the `http_logs` workload against an existing OpenSearch cluster but only use one client for indexing and only ingest 10% of the total data corpus. 
+Execute the `http_logs` workload against an existing OpenSearch cluster but only use one client for indexing and only ingest 10% of the total data corpus.
 
 *Example 3*
 
 ```
-opensearch-benchmark execute_test --workload nyc_taxis --pipeline benchmark-only --target-hosts <endpoint> --client-options "verify_certs:false,use_ssl:true,basic_auth_user:admin,basic_auth_password:admin"
+opensearch-benchmark execute-test --workload nyc_taxis --pipeline benchmark-only --target-hosts <endpoint> --client-options "verify_certs:false,use_ssl:true,basic_auth_user:admin,basic_auth_password:admin"
 ```
 
-Execute the `nyc_taxis` workload against an existing OpenSearch cluster with the security plugin enabled. 
+Execute the `nyc_taxis` workload against an existing OpenSearch cluster with the security plugin enabled.
 
 
 ### All Arguments
 
 Argument | Description | Required
 :--- | :--- |:---
 `distribution-version` | Define the version of the OpenSearch distribution to download. Check https://opensearch.org/docs/version-history/ for released versions. | No
```

### Comparing `opensearch-benchmark-0.4.1/docs/user-guides/create-pipeline.md` & `opensearch-benchmark-0.5.0/docs/user-guides/create-pipeline.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/PKG-INFO` & `opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-benchmark
-Version: 0.4.1
+Version: 0.5.0
 Summary: Macrobenchmarking framework for OpenSearch
 Home-page: https://github.com/opensearch-project/OpenSearch-Benchmark
 Maintainer: Ian Hoang, Govind Kamat
 Maintainer-email: hoangia@amazon.com, govkamat@amazon.com
 License: Apache License, Version 2.0
 Classifier: Topic :: System :: Benchmark
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,15 +63,15 @@
 If you have any trouble or need more detailed instructions, please look in the [detailed installation guide](<https://github.com/opensearch-project/OpenSearch-Benchmark/blob/main/DEVELOPER_GUIDE.md>).
 
 Run your first test execution
 -----------------------------
 
 Now we're ready to run our first test execution:
 
-    opensearch-benchmark execute_test --distribution-version=1.0.0 --workload=geonames --test-mode
+    opensearch-benchmark execute-test --distribution-version=1.0.0 --workload=geonames --test-mode
 
 This will download OpenSearch 1.0.0 and run one of OpenSearch Benchmark's official workloads - the [geonames workload](<https://github.com/opensearch-project/opensearch-benchmark-workloads/tree/main/geonames>) - against it.
 Note that this uses the `--test-mode` argument to only run a single instance of each operation in order to reduce the time needed for a test execution. This argument is used as a sanity check and should be removed in an actual benchmarking scenario.
 After the test execution, a summary report is written to the command line:
 
     ------------------------------------------------------
         _______             __   _____
@@ -127,14 +127,17 @@
     | 99.9th percentile service time |     painless_dynamic |   457.352 |     ms |
     |  100th percentile service time |     painless_dynamic |   459.474 |     ms |
 
     ----------------------------------
     [INFO] SUCCESS (took 2634 seconds)
     ----------------------------------
 
+Creating Your Own Workloads
+---------------------------
+For more information on how users can create their own workloads, see [the Create Workload Guide](./CREATE_WORKLOAD_GUIDE.md)
 
 Getting help
 ------------
 
 * Quick help: ``opensearch-benchmark --help``
 * Look in [OpenSearch Benchmark's user guide](<https://github.com/opensearch-project/OpenSearch-Benchmark/blob/main/DEVELOPER_GUIDE.md>) for more information
 * For any questions or answers, visit our [community forum](<https://discuss.opendistrocommunity.dev/>).
```

### Comparing `opensearch-benchmark-0.4.1/opensearch_benchmark.egg-info/SOURCES.txt` & `opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,22 +113,24 @@
 osbenchmark/builder/utils/config_applier.py
 osbenchmark/builder/utils/git_manager.py
 osbenchmark/builder/utils/host_cleaner.py
 osbenchmark/builder/utils/java_home_resolver.py
 osbenchmark/builder/utils/jdk_resolver.py
 osbenchmark/builder/utils/path_manager.py
 osbenchmark/builder/utils/template_renderer.py
+osbenchmark/resources/base-workload.json.j2
 osbenchmark/resources/benchmark.ini
+osbenchmark/resources/custom-query-workload.json.j2
+osbenchmark/resources/default-query-workload.json.j2
 osbenchmark/resources/docker-compose.yml.j2
 osbenchmark/resources/logging.json
 osbenchmark/resources/metrics-template.json
 osbenchmark/resources/results-template.json
 osbenchmark/resources/test-executions-template.json
 osbenchmark/resources/workload-schema.json
-osbenchmark/resources/workload.json.j2
 osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
 osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
 osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
 osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
 osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
 osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
 osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/__init__.py` & `opensearch-benchmark-0.5.0/osbenchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/actor.py` & `opensearch-benchmark-0.5.0/osbenchmark/actor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/async_connection.py` & `opensearch-benchmark-0.5.0/osbenchmark/async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/benchmark.py` & `opensearch-benchmark-0.5.0/osbenchmark/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         sys.exit(1)
 
     subparsers = parser.add_subparsers(
         title="subcommands",
         dest="subcommand",
         help="")
 
-    test_execution_parser = subparsers.add_parser("execute_test", help="Run a benchmark")
+    test_execution_parser = subparsers.add_parser("execute-test", help="Run a benchmark")
     # change in favor of "list telemetry", "list workloads", "list pipelines"
     list_parser = subparsers.add_parser("list", help="List configuration options")
     list_parser.add_argument(
         "configuration",
         metavar="configuration",
         help="The configuration for which Benchmark should show the available options. "
              "Possible values are: telemetry, workloads, pipelines, test_executions, provision_config_instances, opensearch-plugins",
@@ -172,14 +172,25 @@
         "--client-options",
         default=opts.ClientOptions.DEFAULT_CLIENT_OPTIONS,
         help=f"Comma-separated list of client options to use. (default: {opts.ClientOptions.DEFAULT_CLIENT_OPTIONS})")
     create_workload_parser.add_argument(
         "--output-path",
         default=os.path.join(os.getcwd(), "workloads"),
         help="Workload output directory (default: workloads/)")
+    create_workload_parser.add_argument(
+        "--custom-queries",
+        type=argparse.FileType('r'),
+        help="Input JSON file to use containing custom workload queries that override the default match_all query")
+    create_workload_parser.add_argument(
+        "--number-of-docs",
+        action=opts.StoreKeyPairAsDict,
+        nargs='+',
+        metavar="KEY:VAL",
+        help="Map of index name and integer doc count to extract. Ensure that index name also exists in --indices parameter. " +
+        "To specify several indices and doc counts, use format: <index1>:<doc_count1> <index2>:<doc_count2> ...")
 
     generate_parser = subparsers.add_parser("generate", help="Generate artifacts")
     generate_parser.add_argument(
         "artifact",
         metavar="artifact",
         help="The artifact to create. Possible values are: charts",
         choices=["charts"])
@@ -854,18 +865,18 @@
             cfg.add(config.Scope.applicationOverride, "builder", "runtime.jdk", args.runtime_jdk)
             configure_telemetry_params(args, cfg)
             builder.start(cfg)
         elif sub_command == "stop":
             cfg.add(config.Scope.applicationOverride, "builder", "preserve.install", convert.to_bool(args.preserve_install))
             cfg.add(config.Scope.applicationOverride, "system", "install.id", args.installation_id)
             builder.stop(cfg)
-        elif sub_command == "execute_test":
-            # As the execute_test command is doing more work than necessary at the moment, we duplicate several parameters
+        elif sub_command == "execute-test":
+            # As the execute-test command is doing more work than necessary at the moment, we duplicate several parameters
             # in this section that actually belong to dedicated subcommands (like install, start or stop). Over time
-            # these duplicated parameters will vanish as we move towards dedicated subcommands and use "execute_test" only
+            # these duplicated parameters will vanish as we move towards dedicated subcommands and use "execute-test" only
             # to run the actual benchmark (i.e. generating load).
             if args.effective_start_date:
                 cfg.add(config.Scope.applicationOverride, "system", "time.start", args.effective_start_date)
             cfg.add(config.Scope.applicationOverride, "system", "test_execution.id", args.test_execution_id)
             # use the test_execution id implicitly also as the install id.
             cfg.add(config.Scope.applicationOverride, "system", "install.id", args.test_execution_id)
             cfg.add(config.Scope.applicationOverride, "test_execution", "pipeline", args.pipeline)
@@ -898,16 +909,18 @@
         elif sub_command == "generate":
             cfg.add(config.Scope.applicationOverride, "generator", "chart.spec.path", args.chart_spec_path)
             cfg.add(config.Scope.applicationOverride, "generator", "chart.type", args.chart_type)
             cfg.add(config.Scope.applicationOverride, "generator", "output.path", args.output_path)
             generate(cfg)
         elif sub_command == "create-workload":
             cfg.add(config.Scope.applicationOverride, "generator", "indices", args.indices)
+            cfg.add(config.Scope.applicationOverride, "generator", "number_of_docs", args.number_of_docs)
             cfg.add(config.Scope.applicationOverride, "generator", "output.path", args.output_path)
             cfg.add(config.Scope.applicationOverride, "workload", "workload.name", args.workload)
+            cfg.add(config.Scope.applicationOverride, "workload", "custom_queries", args.custom_queries)
             configure_connection_params(arg_parser, args, cfg)
 
             workload_generator.create_workload(cfg)
         elif sub_command == "info":
             configure_workload_params(arg_parser, args, cfg)
             workload.workload_info(cfg)
         else:
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/benchmarkd.py` & `opensearch-benchmark-0.5.0/osbenchmark/benchmarkd.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/__init__.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/builder.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/cluster.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/cluster.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/cluster_builder.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/cluster_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/configs/utils/config_path_resolver.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/builders/binary_builder.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/builders/source_binary_builder.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/core_plugin_source_downloader.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/downloader.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/external_plugin_source_downloader.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/opensearch_source_downloader.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/plugin_distribution_downloader.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/repository_url_provider.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/downloaders/repositories/source_repository_provider.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/executors/local_shell_executor.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/executors/local_shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/executors/shell_executor.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/executors/shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/bare_installer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/bare_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/docker_installer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/docker_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/exception_handling_installer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/exception_handling_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/installer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/opensearch_preparer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/plugin_preparer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/installers/preparers/preparer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/java_resolver.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/java_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/launcher.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/docker_launcher.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/docker_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/exception_handling_launcher.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/launcher.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/launchers/local_process_launcher.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/local_process_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/models/architecture_types.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/models/architecture_types.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/models/config_instance_types.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/models/config_instance_types.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/models/plugin_config_instance.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/models/plugin_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/models/provision_config_instance.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/models/provision_config_instance_descriptor.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/provision_config.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/provision_config.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/provisioner.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/provisioners/provisioner.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/supplier.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/supplier.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/artifact_variables_provider.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/artifact_variables_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/config_applier.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/config_applier.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/git_manager.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/git_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/host_cleaner.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/host_cleaner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/java_home_resolver.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/java_home_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/jdk_resolver.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/jdk_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/path_manager.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/path_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/builder/utils/template_renderer.py` & `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/template_renderer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/chart_generator.py` & `opensearch-benchmark-0.5.0/osbenchmark/chart_generator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/client.py` & `opensearch-benchmark-0.5.0/osbenchmark/client.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/config.py` & `opensearch-benchmark-0.5.0/osbenchmark/config.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/exceptions.py` & `opensearch-benchmark-0.5.0/osbenchmark/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/log.py` & `opensearch-benchmark-0.5.0/osbenchmark/log.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/metrics.py` & `opensearch-benchmark-0.5.0/osbenchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/paths.py` & `opensearch-benchmark-0.5.0/osbenchmark/paths.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/benchmark.ini` & `opensearch-benchmark-0.5.0/osbenchmark/resources/benchmark.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/docker-compose.yml.j2` & `opensearch-benchmark-0.5.0/osbenchmark/resources/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/logging.json` & `opensearch-benchmark-0.5.0/osbenchmark/resources/logging.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/metrics-template.json` & `opensearch-benchmark-0.5.0/osbenchmark/resources/metrics-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/results-template.json` & `opensearch-benchmark-0.5.0/osbenchmark/resources/results-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/test-executions-template.json` & `opensearch-benchmark-0.5.0/osbenchmark/resources/test-executions-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/workload-schema.json` & `opensearch-benchmark-0.5.0/osbenchmark/resources/workload-schema.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/resources/workload.json.j2` & `opensearch-benchmark-0.5.0/osbenchmark/resources/base-workload.json.j2`

 * *Files 4% similar despite different names*

```diff
@@ -46,10 +46,11 @@
     {
       "operation": {
         "operation-type": "bulk",
         "bulk-size": {{bulk_size | default(5000)}},
         "ingest-percentage": {{ingest_percentage | default(100)}}
       },
       "clients": {{bulk_indexing_clients | default(8)}}
-    }
-  ]{% endraw %}
+    },{% endraw -%}
+    {% block queries %}{% endblock %}
+  ]
 }
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/results_publisher.py` & `opensearch-benchmark-0.5.0/osbenchmark/results_publisher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/telemetry.py` & `opensearch-benchmark-0.5.0/osbenchmark/telemetry.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/test_execution_orchestrator.py` & `opensearch-benchmark-0.5.0/osbenchmark/test_execution_orchestrator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/time.py` & `opensearch-benchmark-0.5.0/osbenchmark/time.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/__init__.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/collections.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/collections.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/console.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/console.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/convert.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/convert.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/git.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/git.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/io.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/io.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/jvm.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/modules.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/modules.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/net.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/net.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/opts.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/opts.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 import difflib
 import json
+import argparse
 
+from osbenchmark import exceptions
 from osbenchmark.utils import io
 
 
 def csv_to_list(csv):
     if csv is None:
         return None
     elif len(csv.strip()) == 0:
         return []
     else:
         return [e.strip() for e in csv.split(",")]
 
-
 def to_bool(v):
     if v is None:
         return None
     elif v.lower() == "false":
         return False
     elif v.lower() == "true":
         return True
@@ -113,14 +114,33 @@
     for param in word_list:
         matched_word = difflib.get_close_matches(param, all_possibilities, n=1)
         if matched_word:
             close_matches.append(matched_word[0])
 
     return close_matches
 
+class StoreKeyPairAsDict(argparse.Action):
+    """
+    Custom Argparse action that allows users to pass in a key:value pairs after specifying a parameter.
+    Used as action for --number-of-docs parameter for create-workload subcommand.
+    """
+    def __call__(self, parser, namespace, values, option_string=None):
+        custom_dict = {}
+        for kv in values:
+            try:
+                k,v = kv.split(":")
+                custom_dict[k] = v
+            except ValueError:
+                raise exceptions.InvalidSyntax(
+                    "StoreKeyPairAsDict: Could not convert string to dict due to invalid syntax."
+                    )
+        setattr(namespace, self.dest, custom_dict)
+
+        return custom_dict
+
 
 class ConnectOptions:
     """
     Base Class to help either parsing --target-hosts or --client-options
     """
 
     def __getitem__(self, key):
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/periodic_waiter.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/periodic_waiter.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/process.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/process.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/repo.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/repo.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/sysstats.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/sysstats.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/utils/versions.py` & `opensearch-benchmark-0.5.0/osbenchmark/utils/versions.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/version.py` & `opensearch-benchmark-0.5.0/osbenchmark/version.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/__init__.py` & `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/runner.py` & `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/runner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/scheduler.py` & `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/scheduler.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/worker_coordinator/worker_coordinator.py` & `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/worker_coordinator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload/__init__.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload/loader.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload/loader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload/params.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,44 +196,51 @@
             for idx in workload.indices:
                 if not filter_idx or idx.name in filter_idx:
                     body = idx.body
                     if body and settings:
                         if "settings" in body:
                             # merge (and potentially override)
                             body["settings"].update(settings)
+                            self.validate_index_codec(body["settings"])
                         else:
                             body["settings"] = settings
                     elif not body and settings:
                         body = {
                             "settings": settings
                         }
-
                     self.index_definitions.append((idx.name, body))
         else:
             try:
                 # only 'index' is mandatory, the body is optional (may be ok to create an index without a body)
                 idx = params["index"]
                 body = params.get("body")
+                if body and "settings" in body:
+                    self.validate_index_codec(body["settings"])
                 if isinstance(idx, str):
                     idx = [idx]
                 for i in idx:
                     self.index_definitions.append((i, body))
+            except ValueError as e:
+                raise exceptions.InvalidSyntax(f"Please set the value properly for the create-index operation. {e}")
             except KeyError:
                 raise exceptions.InvalidSyntax("Please set the property 'index' for the create-index operation")
 
     def params(self):
         p = {}
         # ensure we pass all parameters...
         p.update(self._params)
         p.update({
             "indices": self.index_definitions,
             "request-params": self.request_params
         })
         return p
 
+    def validate_index_codec(self, settings):
+        if "index.codec" in settings:
+            return workload.IndexCodec.is_codec_valid(settings["index.codec"])
 
 class CreateDataStreamParamSource(ParamSource):
     def __init__(self, workload, params, **kwargs):
         super().__init__(workload, params, **kwargs)
         self.request_params = params.get("request-params", {})
         self.data_stream_definitions = []
         if workload.data_streams:
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload/workload.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload/workload.py`

 * *Files 1% similar despite different names*

```diff
@@ -709,14 +709,27 @@
         elif v == "delete-point-in-time":
             return OperationType.DeletePointInTime
         elif v == "list-all-point-in-time":
             return OperationType.ListAllPointInTime
         else:
             raise KeyError(f"No enum value for [{v}]")
 
+@unique
+class IndexCodec(Enum):
+    Default = "default"
+    BestCompression = "best_compression"
+
+    @classmethod
+    def is_codec_valid(cls, codec):
+        for valid_codec in cls:
+            if codec == valid_codec.value:
+                return True
+
+        raise ValueError(f"Invalid index.codec value '{codec}'")
+
 
 class TaskNameFilter:
     def __init__(self, name):
         self.name = name
 
     def matches(self, task):
         return self.name == task.name
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload_generator/__init__.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload_generator/corpus.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/corpus.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,61 +46,64 @@
     }
 
 
 def get_doc_outpath(outdir, name, suffix=""):
     return os.path.join(outdir, f"{name}-documents{suffix}.json")
 
 
-def extract(client, output_path, index):
+def extract(client, output_path, index, number_of_docs_requested=None):
     """
     Scroll an index with a match-all query, dumping document source to ``outdir/documents.json``.
 
     :param client: OpenSearch client used to extract data
     :param output_path: Destination directory for corpus dump
     :param index: Name of index to dump
     :return: dict of properties describing the corpus for templates
     """
 
     logger = logging.getLogger(__name__)
 
-    total_docs = client.count(index=index)["count"]
+    number_of_docs = client.count(index=index)["count"]
+
+    total_docs = number_of_docs if not number_of_docs_requested else min(number_of_docs, number_of_docs_requested)
+
     if total_docs > 0:
-        logger.info("[%d] total docs in index [%s].", total_docs, index)
+        logger.info("[%d] total docs in index [%s]. Extracting [%s] docs.", number_of_docs, index, total_docs)
         docs_path = get_doc_outpath(output_path, index)
         dump_documents(client, index, get_doc_outpath(output_path, index, "-1k"), min(total_docs, 1000), " for test mode")
         dump_documents(client, index, docs_path, total_docs)
         return template_vars(index, docs_path, total_docs)
     else:
         logger.info("Skipping corpus extraction fo index [%s] as it contains no documents.", index)
         return None
 
 
-def dump_documents(client, index, out_path, total_docs, progress_message_suffix=""):
+def dump_documents(client, index, out_path, number_of_docs, progress_message_suffix=""):
     # pylint: disable=import-outside-toplevel
     from opensearchpy import helpers
 
     logger = logging.getLogger(__name__)
-    freq = max(1, total_docs // 1000)
+    freq = max(1, number_of_docs // 1000)
 
     progress = console.progress()
     compressor = DOCS_COMPRESSOR()
     comp_outpath = out_path + COMP_EXT
     with open(out_path, "wb") as outfile:
         with open(comp_outpath, "wb") as comp_outfile:
             logger.info("Dumping corpus for index [%s] to [%s].", index, out_path)
             query = {"query": {"match_all": {}}}
             for n, doc in enumerate(helpers.scan(client, query=query, index=index)):
-                if n >= total_docs:
+                if n >= number_of_docs:
                     break
                 data = (json.dumps(doc["_source"], separators=(",", ":")) + "\n").encode("utf-8")
 
                 outfile.write(data)
                 comp_outfile.write(compressor.compress(data))
 
-                render_progress(progress, progress_message_suffix, index, n + 1, total_docs, freq)
+                render_progress(progress, progress_message_suffix, index, n + 1, number_of_docs, freq)
 
             comp_outfile.write(compressor.flush())
     progress.finish()
 
 
 def render_progress(progress, progress_message_suffix, index, cur, total, freq):
     if cur % freq == 0 or total - cur < freq:
```

### Comparing `opensearch-benchmark-0.4.1/osbenchmark/workload_generator/index.py` & `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/index.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/scripts/expand-data-corpus.py` & `opensearch-benchmark-0.5.0/scripts/expand-data-corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 data corpus associated an OSB workload.  Currently, this capability is
 implemented only for the http_logs workload.
 
 TLDR: to generate a 100 GB corpus and then run a test against it:
 
 $ expand-data-corpus.py --corpus-size 100 --output-file-suffix 100gb
 
-$ opensearch-benchmark execute_test --workload http_logs \\
+$ opensearch-benchmark execute-test --workload http_logs \\
     --workload_params=generated_corpus:t ...
 
 The script generates new documents by duplicating ones in the existing
 corpus files, while modifying the timestamp field.  It takes several
 arguments, listed below.  The two primary ones deal with specifying
 the desired target corpus size and the corpus name.  The remaining
 options, tagged with "EXPERT", are mainly intended for advanced users.
```

### Comparing `opensearch-benchmark-0.4.1/setup.py` & `opensearch-benchmark-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/tests/test_async_connection.py` & `opensearch-benchmark-0.5.0/tests/test_async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.4.1/tests/test_execution_orchestrator_test.py` & `opensearch-benchmark-0.5.0/tests/test_execution_orchestrator_test.py`

 * *Files identical despite different names*

