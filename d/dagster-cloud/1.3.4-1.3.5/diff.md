# Comparing `tmp/dagster_cloud-1.3.4.tar.gz` & `tmp/dagster_cloud-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.3.4.tar", last modified: Thu May 11 17:10:42 2023, max compression
+gzip compressed data, was "dagster_cloud-1.3.5.tar", last modified: Thu May 18 20:49:47 2023, max compression
```

## Comparing `dagster_cloud-1.3.4.tar` & `dagster_cloud-1.3.5.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.827479 dagster_cloud-1.3.4/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-05-11 17:10:42.827479 dagster_cloud-1.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.735480 dagster_cloud-1.3.4/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.739480 dagster_cloud-1.3.4/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.739480 dagster_cloud-1.3.4/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43075 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.743480 dagster_cloud-1.3.4/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.743480 dagster_cloud-1.3.4/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.743480 dagster_cloud-1.3.4/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.747480 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.751480 dagster_cloud-1.3.4/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14188 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.755480 dagster_cloud-1.3.4/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.759480 dagster_cloud-1.3.4/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.759480 dagster_cloud-1.3.4/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.771480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.779480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.787480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.787480 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.791480 dagster_cloud-1.3.4/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.791480 dagster_cloud-1.3.4/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.795480 dagster_cloud-1.3.4/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.795480 dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.799480 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26932 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.803480 dagster_cloud-1.3.4/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19041 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.803480 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     6552 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.803480 dagster_cloud-1.3.4/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.807479 dagster_cloud-1.3.4/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.807479 dagster_cloud-1.3.4/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.811480 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.815480 dagster_cloud-1.3.4/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.819480 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23263 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    21621 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.819480 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.823480 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74026 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:42.739480 dagster_cloud-1.3.4/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-11 17:10:42.000000 dagster_cloud-1.3.4/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 17:10:42.827479 dagster_cloud-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-05-11 16:59:01.000000 dagster_cloud-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.317680 dagster_cloud-1.3.5/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.321680 dagster_cloud-1.3.5/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.321680 dagster_cloud-1.3.5/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43075 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.321680 dagster_cloud-1.3.5/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.325680 dagster_cloud-1.3.5/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.325680 dagster_cloud-1.3.5/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.333680 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.333680 dagster_cloud-1.3.5/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.337680 dagster_cloud-1.3.5/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.337680 dagster_cloud-1.3.5/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.337680 dagster_cloud-1.3.5/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.341680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.341680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.345680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.345680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.349680 dagster_cloud-1.3.5/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.349680 dagster_cloud-1.3.5/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.349680 dagster_cloud-1.3.5/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.353680 dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.357680 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    26932 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.357680 dagster_cloud-1.3.5/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19041 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.361680 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.361680 dagster_cloud-1.3.5/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.361680 dagster_cloud-1.3.5/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.365680 dagster_cloud-1.3.5/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.365680 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.369680 dagster_cloud-1.3.5/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.373680 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23263 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    21621 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.377680 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74026 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.317680 dagster_cloud-1.3.5/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/setup.py
```

### Comparing `dagster_cloud-1.3.4/PKG-INFO` & `dagster_cloud-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.3.4
+Version: 1.3.5
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.4/README.md` & `dagster_cloud-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.3.5/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/agent/queries.py` & `dagster_cloud-1.3.5/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.3.5/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/auth/constants.py` & `dagster_cloud-1.3.5/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.3.5/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.3.5/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.3.5/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/client.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.3.5/dagster_cloud/storage/schedules/storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence, Set
 
 import dagster._check as check
+from dagster import AssetKey
+from dagster._core.definitions.asset_reconciliation_sensor import AutoMaterializeAssetEvaluation
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.scheduler.instigation import (
+    AutoMaterializeAssetEvaluationRecord,
     InstigatorState,
     InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.schedules.base import ScheduleStorage
@@ -188,12 +191,24 @@
         origin_id: str,
         selector_id: str,
         before: float,
         tick_statuses: Optional[Sequence[TickStatus]] = None,
     ):
         raise NotImplementedError("Not callable from user cloud")
 
+    def add_auto_materialize_asset_evaluations(
+        self,
+        evaluation_id: int,
+        asset_evaluations: Sequence[AutoMaterializeAssetEvaluation],
+    ) -> None:
+        raise NotImplementedError("Not callable from user cloud")
+
+    def get_auto_materialize_asset_evaluations(
+        self, asset_key: AssetKey, limit: int, cursor: Optional[int] = None
+    ) -> Sequence[AutoMaterializeAssetEvaluationRecord]:
+        raise NotImplementedError("Not callable from user cloud")
+
     def upgrade(self):
         raise NotImplementedError("Not callable from user cloud")
 
     def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int):
         raise NotImplementedError("Not callable from user cloud")
```

### Comparing `dagster_cloud-1.3.4/dagster_cloud/util/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.3.5/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.3.4
+Version: 1.3.5
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.4/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.3.5/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.4/setup.py` & `dagster_cloud-1.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.4",
-        "dagster-cloud-cli==1.3.4",
+        "dagster==1.3.5",
+        "dagster-cloud-cli==1.3.5",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.19.4",
+            "dagster_k8s==0.19.5",
         ],
-        "docker": ["docker", "dagster_docker==0.19.4"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.19.4"],
-        "ecs": ["dagster_aws==0.19.4", "boto3"],
+        "docker": ["docker", "dagster_docker==0.19.5"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.19.5"],
+        "ecs": ["dagster_aws==0.19.5", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

