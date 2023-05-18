# Comparing `tmp/domino-py-0.2.5.tar.gz` & `tmp/domino-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.2.5.tar", last modified: Sat May 13 14:33:06 2023, max compression
+gzip compressed data, was "domino-py-0.3.0.tar", last modified: Thu May 18 06:57:42 2023, max compression
```

## Comparing `domino-py-0.2.5.tar` & `domino-py-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.514493 domino-py-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-13 14:32:51.000000 domino-py-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-13 14:33:06.514493 domino-py-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-13 14:32:51.000000 domino-py-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.506493 domino-py-0.2.5/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.506493 domino-py-0.2.5/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.506493 domino-py-0.2.5/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    24061 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/docker_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/external_python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/custom_operators/sidecar/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/schemas/deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/piece_dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/run_piece_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/utils/piece_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 14:32:51.000000 domino-py-0.2.5/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:33:06.510493 domino-py-0.2.5/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-13 14:33:06.000000 domino-py-0.2.5/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-13 14:33:06.000000 domino-py-0.2.5/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 14:33:06.000000 domino-py-0.2.5/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-13 14:33:06.000000 domino-py-0.2.5/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-13 14:33:06.000000 domino-py-0.2.5/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 14:33:06.000000 domino-py-0.2.5/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 14:33:06.514493 domino-py-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-13 14:32:51.000000 domino-py-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.772395 domino-py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 06:57:28.000000 domino-py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-18 06:57:42.772395 domino-py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-18 06:57:28.000000 domino-py-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.752395 domino-py-0.3.0/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.752395 domino-py-0.3.0/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.756395 domino-py-0.3.0/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24061 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.760395 domino-py-0.3.0/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.760395 domino-py-0.3.0/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.760395 domino-py-0.3.0/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/sidecar/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.764395 domino-py-0.3.0/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.764395 domino-py-0.3.0/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/display_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.768395 domino-py-0.3.0/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/run_piece_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.768395 domino-py-0.3.0/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.772395 domino-py-0.3.0/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:57:42.772395 domino-py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-18 06:57:29.000000 domino-py-0.3.0/setup.py
```

### Comparing `domino-py-0.2.5/LICENSE` & `domino-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/PKG-INFO` & `domino-py-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.2.5
+Version: 0.3.0
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.2.5 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.3.0 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
    [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
                                    logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
```

### Comparing `domino-py-0.2.5/README.md` & `domino-py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/base_piece.py` & `domino-py-0.3.0/domino/base_piece.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import abc
 import json
 import os
 import ast
 from datetime import datetime
 from pathlib import Path
+from typing import Union
 import pydantic
 import pickle
+import time
+import subprocess
+import base64
+
 from domino.logger import get_configured_logger
 from domino.schemas.deploy_mode import DeployModeType
+from domino.schemas.display_result import DisplayResultFileType
 from domino.exceptions.exceptions import InvalidPieceOutputError
-import time
-import subprocess
 
 
 class BasePiece(metaclass=abc.ABCMeta):
 
     @classmethod
     def set_metadata(cls, metadata):
         """
@@ -52,28 +56,32 @@
         self.task_id = task_id
         self.dag_id = dag_id
         self.deploy_mode = deploy_mode
 
         # Logger
         self.logger = get_configured_logger(f"{self.__class__.__name__ }-{self.task_id}")
 
+        self.display_result = None
+
 
     def start_logger(self):
         """
         Start logger.
         """
         self.logger.info(f"Started {self.task_id} of type {self.__class__.__name__} at {str(datetime.now().isoformat())}")
 
+
     def _wait_for_sidecar_paths(self):
         # Wait for sidecar create directories
         while True:
             if Path(self.report_path).is_dir():
                 break
             time.sleep(2)
 
+
     def generate_paths(self):
         """
         Generates paths for shared storage.
         """
         # Base path for fetching and storing runs results
         if not Path(self.workflow_shared_storage).is_dir():
             Path(self.workflow_shared_storage).mkdir(parents=True, exist_ok=True)
@@ -174,14 +182,29 @@
                     v_type = v["type"]
             elif "anyOf" in v:
                 if "$ref" in v["anyOf"][0]:
                     type_model = v["anyOf"][0]["$ref"].split("/")[-1]
                     v_type = output_schema["definitions"][type_model]["type"]
             xcom_obj[f"{k}_type"] = v_type
 
+        # Serialize self.display_result and add it to XCOM
+        if isinstance(self.display_result, dict):
+            if "file_type" not in self.display_result:
+                raise Exception("display_result must have 'file_type' key")
+            if "base64_content" not in self.display_result:
+                if "file_path" not in self.display_result:
+                    raise Exception("self.display_result dict must have either 'file_path' or 'base64_content' keys")
+                self.display_result["base64_content"] = self.serialize_display_result_file(
+                    file_path=self.display_result["file_path"],
+                    file_type=self.display_result["file_type"]
+                )
+            self.display_result["file_path"] = str(self.display_result["file_path"])
+            self.display_result["file_type"] = str(self.display_result["file_type"])
+            xcom_obj["display_result"] = self.display_result
+
         # Update XCOM with extra metadata
         xcom_obj.update(
             piece_name=self.__class__.__name__,
             piece_metadata=self._metadata_
         )
         return xcom_obj
 
@@ -194,39 +217,42 @@
             xcom_obj (dict): Formatted XCOM object as a dictionary
 
         Raises:
             NotImplementedError: _description_
         """
         if self.deploy_mode in ["local-python"]:
             self.airflow_context['ti'].xcom_push(key=self.task_id, value=xcom_obj)
+
         elif self.deploy_mode == "local-compose":
             file_path = Path('/airflow/xcom/return.out')
             file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(str(file_path), 'wb') as fp:
                 pickle.dump(xcom_obj, fp)
 
         elif self.deploy_mode == "local-bash":
             # For our extended BashOperator, return XCom must be stored in /opt/mnt/fs/tmp/xcom_output.json
             file_path = Path("/opt/mnt/fs/tmp/xcom_output.json")
             file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(str(file_path), 'w') as fp:
                 json.dump(xcom_obj, fp, indent=4)
+
         elif self.deploy_mode in ["k8s", "local-k8s", "local-k8s-dev"]:
             # In Kubernetes, return XCom must be stored in /airflow/xcom/return.json
             # https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/stable/pieces.html#how-does-xcom-work
             file_path = Path('/airflow/xcom/return.json')
             file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(str(file_path), 'w') as fp:
                 json.dump(xcom_obj, fp)
 
             # Also store it at /home/workflow_shared_data/{self.task_id}/xcom/return.json for convenience
             file_path = self.xcom_path + "/return.json"
             with open(file_path, 'w') as fp:
                 json.dump(xcom_obj, fp)
             #time.sleep(120)
+
         else:
             raise NotImplementedError("deploy mode not accepted for xcom push")
     
 
     def run_piece_function(
         self, 
         airflow_context: dict,
@@ -317,48 +343,52 @@
             secrets=secrets_model_obj,
             results_path=results_path
         )
 
         # Run piece function
         return cls.piece_function(self=dry_instance, input_model=input_model_obj)
 
+
     @staticmethod
     def get_container_cpu_limit() -> float:
         """
         Get the CPU limit of the container in millicores.
         reference: https://stackoverflow.com/questions/65551215/get-docker-cpu-memory-limit-inside-container/65554131#65554131
         """
         with open("/sys/fs/cgroup/cpu/cpu.cfs_quota_us") as fp:
             cfs_quota_us = int(fp.read())
         with open("/sys/fs/cgroup/cpu/cpu.cfs_period_us") as fp:
             cfs_period_us = int(fp.read())
 
         container_cpus = float(cfs_quota_us / cfs_period_us)
         return container_cpus
 
+
     @staticmethod
     def get_nvidia_smi_output() -> str:
         """
         Get the output of nvidia-smi command.
         """
         try:
             nvidia_smi_output = subprocess.check_output(["nvidia-smi", "-q"])
             return nvidia_smi_output
         except Exception as e:
             raise Exception(f"Error while running nvidia-smi: {e}")
 
+
     @staticmethod
     def get_container_memory_limit() -> int:
         """
         Get the memory limit of the container in bytes.
         """
         with open("/sys/fs/cgroup/memory/memory.limit_in_bytes") as fp:
             container_memory_limit = int(fp.read())
         return container_memory_limit
 
+
     @staticmethod
     def get_container_memory_usage() -> int:
         """
         Get the memory usage of the container in bytes.
         """
         with open("/sys/fs/cgroup/memory/memory.usage_in_bytes") as fp:
             container_memory_usage = int(fp.read())
@@ -370,11 +400,36 @@
         """
         This function carries the relevant code for the Piece run.
         It should have all the necessary content for auto-generating json schemas.
         All arguments should be type annotated and docstring should carry description for each argument.
         """
         raise NotImplementedError("This method must be implemented in the child class!")        
 
-    
-    def generate_report(self):
-        """This function carries the relevant code for the Piece report."""
-        raise NotImplementedError("This method must be implemented in the child class!")
+
+    def serialize_display_result_file(self, file_path: Union[str, Path], file_type: DisplayResultFileType) -> dict:
+        """
+        Serializes the content of 'display_result_file' into base64 string, to fit Airflow XCOM.
+
+        Args:
+            file_path (Union[str, Path]): The path to the file.
+            file_type (DisplayResultFileType): The type of the file.
+
+        Returns:
+            dict: A dictionary containing the base64-encoded content and the file type.
+        """
+        if not Path(file_path).exists():
+            print(f"File {file_path} does not exist. Skipping serialization...")
+            return None
+        if not Path(file_path).is_file():
+            print(f"Path {file_path} is not a file. Skipping serialization...")
+            return None
+        # Read file content as bytes and encode content into base64
+        with open(file_path, "rb") as f:
+            content_bytes = f.read()
+        encoded_content = base64.b64encode(content_bytes).decode('utf-8')
+        return encoded_content
+
+
+    # @abc.abstractmethod
+    # def generate_report(self):
+    #     """This function carries the relevant code for the Piece report."""
+    #     raise NotImplementedError("This method must be implemented in the child class!")
```

### Comparing `domino-py-0.2.5/domino/cli/cli.py` & `domino-py-0.3.0/domino/cli/cli.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/cli/utils/pieces_repository.py` & `domino-py-0.3.0/domino/cli/utils/pieces_repository.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/cli/utils/platform.py` & `domino-py-0.3.0/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/client/airflow_client.py` & `domino-py-0.3.0/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/client/domino_backend_client.py` & `domino-py-0.3.0/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/client/fs_client.py` & `domino-py-0.3.0/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/client/github_rest_client.py` & `domino-py-0.3.0/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/client/local_files_client.py` & `domino-py-0.3.0/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/client/s3_client.py` & `domino-py-0.3.0/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/custom_operators/docker_operator.py` & `domino-py-0.3.0/domino/custom_operators/docker_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,19 @@
         self._set_base_env_vars()
         docker_url = 'tcp://docker-proxy:2375'
     
         shared_storage_host_path = os.environ.get('LOCAL_DOMINO_SHARED_DATA_PATH', '')
         shared_storage_container_path = '/home/shared_storage'
         mounts = []
         # # TODO remove
-        # mounts=[
-        #     # TODO remove
-        #     Mount(source='/home/vinicius/Documents/work/tauffer/flowui/domino', target='/home/domino/domino_py/domino', type='bind', read_only=True),
-        # ]
+        mounts=[
+            # TODO remove
+            # Mount(source='/media/luiz/storage2/Github/domino/domino', target='/home/domino/domino_py/domino', type='bind', read_only=True),
+            # Mount(source='/media/luiz/storage2/Github/default_domino_pieces', target='/home/domino/pieces_repository/', type='bind', read_only=True),
+        ]
         if self.workflow_shared_storage and str(self.workflow_shared_storage.source.value).lower() == str(getattr(StorageSource, 'local').value).lower():
             mounts.append(
                 Mount(source=shared_storage_host_path, target=shared_storage_container_path, type='bind', read_only=False),
             )
 
         super().__init__(
             **kwargs,
```

### Comparing `domino-py-0.2.5/domino/custom_operators/external_python_operator.py` & `domino-py-0.3.0/domino/custom_operators/external_python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/custom_operators/k8s_operator.py` & `domino-py-0.3.0/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/custom_operators/python_operator.py` & `domino-py-0.3.0/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/custom_operators/sidecar/logger.py` & `domino-py-0.3.0/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/custom_operators/sidecar/mount.py` & `domino-py-0.3.0/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/exceptions/exceptions.py` & `domino-py-0.3.0/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/logger.py` & `domino-py-0.3.0/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/schemas/piece_metadata.py` & `domino-py-0.3.0/domino/schemas/piece_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 class OutputSchema(BaseModel):
     title: str
     description: str
     type: str
     properties: Dict
 
 
+class SecretsSchema(BaseModel):
+    title: str
+    description: str
+    type: str
+    properties: Dict
+
+
 class PieceMetadata(BaseModel):
     name: str = Field(
         description="Piece name", 
         example="ExamplePiece", 
         # regex=    # TODO - regex for *Operator  
     )
     description: str = Field(
@@ -46,8 +53,10 @@
         example="This Piece executes ABCDEFG function.", 
     )
     dependency: Dependency = None
     container_resources: Dict = None # TODO - add model for the container_resources dictionary
     tags: List[str] = None
     style: Dict = None # TODO - add model for the style dictionary
     input_schema: InputSchema = None
-    output_schema: OutputSchema = None
+    output_schema: OutputSchema = None
+    secrets_schema: SecretsSchema = None
+    source_url: str = None
```

### Comparing `domino-py-0.2.5/domino/schemas/shared_storage.py` & `domino-py-0.3.0/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.3.0/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/create_docker_compose_file.py` & `domino-py-0.3.0/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/docker_compose_constants.py` & `domino-py-0.3.0/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/docker_compose_scripts.py` & `domino-py-0.3.0/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/load_piece.py` & `domino-py-0.3.0/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/piece_dry_run.py` & `domino-py-0.3.0/domino/scripts/piece_dry_run.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/run_piece_bash.py` & `domino-py-0.3.0/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/run_piece_docker.py` & `domino-py-0.3.0/domino/scripts/run_piece_docker.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/scripts/run_piece_k8s.py` & `domino-py-0.3.0/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/task.py` & `domino-py-0.3.0/domino/task.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino/utils/piece_generator.py` & `domino-py-0.3.0/domino/utils/piece_generator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.5/domino_py.egg-info/PKG-INFO` & `domino-py-0.3.0/domino_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.2.5
+Version: 0.3.0
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.2.5 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.3.0 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
    [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
                                    logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
```

### Comparing `domino-py-0.2.5/domino_py.egg-info/SOURCES.txt` & `domino-py-0.3.0/domino_py.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 domino/custom_operators/sidecar/logger.py
 domino/custom_operators/sidecar/mount.py
 domino/exceptions/__init__.py
 domino/exceptions/exceptions.py
 domino/schemas/__init__.py
 domino/schemas/container_resources.py
 domino/schemas/deploy_mode.py
+domino/schemas/display_result.py
 domino/schemas/from_upstream.py
 domino/schemas/piece_metadata.py
 domino/schemas/shared_storage.py
 domino/scripts/__init__.py
 domino/scripts/build_docker_images_pieces.py
 domino/scripts/create_docker_compose_file.py
 domino/scripts/docker_compose_constants.py
```

### Comparing `domino-py-0.2.5/setup.py` & `domino-py-0.3.0/setup.py`

 * *Files identical despite different names*

