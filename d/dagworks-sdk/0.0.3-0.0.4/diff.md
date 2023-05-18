# Comparing `tmp/dagworks-sdk-0.0.3.tar.gz` & `tmp/dagworks-sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks-sdk-0.0.3.tar", last modified: Mon May 15 06:50:14 2023, max compression
+gzip compressed data, was "dagworks-sdk-0.0.4.tar", last modified: Thu May 18 05:40:33 2023, max compression
```

## Comparing `dagworks-sdk-0.0.3.tar` & `dagworks-sdk-0.0.4.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.794219 dagworks-sdk-0.0.3/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-05-06 22:02:15.000000 dagworks-sdk-0.0.3/LICENSE
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-15 06:50:14.793932 dagworks-sdk-0.0.3/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-05-11 21:36:24.000000 dagworks-sdk-0.0.3/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-09 05:21:02.000000 dagworks-sdk-0.0.3/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        7 2023-05-06 23:25:38.000000 dagworks-sdk-0.0.3/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      159 2023-05-12 05:33:31.000000 dagworks-sdk-0.0.3/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-05-15 06:50:14.794346 dagworks-sdk-0.0.3/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-05-06 22:26:36.000000 dagworks-sdk-0.0.3/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.728571 dagworks-sdk-0.0.3/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.731438 dagworks-sdk-0.0.3/src/dagworks/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.734625 dagworks-sdk-0.0.3/src/dagworks/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.738502 dagworks-sdk-0.0.3/src/dagworks/api/api_client/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.739193 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.741953 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3379 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2926 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5383 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4111 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4813 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.746467 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3035 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5855 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4711 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5053 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4516 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4994 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8029 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5693 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5511 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5779 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6327 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.748537 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4421 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5087 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6058 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6286 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5367 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2817 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/client.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      470 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/errors.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.767729 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4237 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/dependency.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2706 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1285 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3019 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1268 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_function.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/organization_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/phone_home_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4499 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5339 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5848 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/python_type.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_data.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5416 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1185 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_inputs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_run_log.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6517 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_inputs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7054 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run_result_summary.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run_status.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3189 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2916 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/user_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_full.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3802 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/who_am_i_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      993 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/api/api_client/types.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9750 2023-05-15 05:04:41.000000 dagworks-sdk-0.0.3/src/dagworks/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1168 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.768718 dagworks-sdk-0.0.3/src/dagworks/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2025 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6513 2023-05-12 05:36:10.000000 dagworks-sdk-0.0.3/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.769149 dagworks-sdk-0.0.3/src/dagworks/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.771162 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-05-08 21:41:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-05-08 21:39:25.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-05-12 05:13:34.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.771717 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.773165 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-05-06 23:33:53.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-05-12 05:09:58.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.773587 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.774685 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-05-12 05:13:41.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.775068 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.775570 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2023-05-14 22:17:33.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.776330 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.776604 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.778683 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-05-04 05:23:39.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-05-12 05:08:52.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-05-12 05:09:11.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.779266 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.781436 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-05-08 17:20:15.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.781755 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    14062 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/src/dagworks/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.786514 dagworks-sdk-0.0.3/src/dagworks/parsing/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/parsing/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/parsing/dagtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/parsing/parse.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.788478 dagworks-sdk-0.0.3/src/dagworks/telemetry/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.790021 dagworks-sdk-0.0.3/src/dagworks/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    10840 2023-05-12 23:31:41.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-05-08 17:27:33.000000 dagworks-sdk-0.0.3/src/dagworks/tracking/trackingtypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.791561 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8551 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      177 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-05-15 06:50:14.000000 dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-05-15 06:50:14.793291 dagworks-sdk-0.0.3/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-05-06 23:49:00.000000 dagworks-sdk-0.0.3/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5497 2023-05-06 22:02:08.000000 dagworks-sdk-0.0.3/tests/test_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-02-13 05:18:55.000000 dagworks-sdk-0.0.3/tests/test_telemetry.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6081 2023-05-14 22:17:24.000000 dagworks-sdk-0.0.3/tests/test_tracking.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.483263 dagworks-sdk-0.0.4/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2212 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/LICENSE
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4695 2023-05-18 05:40:33.483050 dagworks-sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3655 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/README.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/pyproject.toml
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        7 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/requirements-test.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      159 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/requirements.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2023-05-18 05:40:33.483314 dagworks-sdk-0.0.4/setup.cfg
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      115 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/setup.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.449028 dagworks-sdk-0.0.4/src/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.450319 dagworks-sdk-0.0.4/src/dagworks/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1092 2023-05-18 05:39:43.000000 dagworks-sdk-0.0.4/src/dagworks/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.451402 dagworks-sdk-0.0.4/src/dagworks/api/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.452261 dagworks-sdk-0.0.4/src/dagworks/api/api_client/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      152 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.452408 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.453378 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3379 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2926 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5383 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4111 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4813 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.455238 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3035 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5855 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4711 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5053 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4516 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4994 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8029 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5693 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5511 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5779 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6327 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.456052 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4421 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5087 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6058 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6286 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5367 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2817 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/client.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      470 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/errors.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.468853 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4237 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2443 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/api_key_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1982 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/dependency.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2706 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1285 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3019 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1268 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2766 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2480 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_function.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3778 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_node.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1692 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1175 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_node_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/organization_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/paged_api_key_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2238 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/paged_project_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/paged_run_log_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1649 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/phone_home_result.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1977 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1179 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_in_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4499 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1165 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_out_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3909 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_in_git.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_in_git_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1243 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_in_git_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5339 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1203 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_version_info.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5848 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_with_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1244 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1282 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1422 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/python_type.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1791 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_data.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5416 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1185 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1171 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_run_log.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6517 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1163 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7054 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3710 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/task_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1198 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/task_run_result_summary.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      226 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/task_run_status.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3189 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2916 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1586 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/user_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4362 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/visibility_full.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3802 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/visibility_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2306 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/who_am_i_result.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      993 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/api_client/types.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9750 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/api/clients.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1168 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/constants.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1311 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.469307 dagworks-sdk-0.0.4/src/dagworks/cli/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2025 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/cli.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6513 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.471653 dagworks-sdk-0.0.4/src/dagworks/cli/templates/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.472970 dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      123 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      307 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       51 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2698 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      697 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.473207 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.473816 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      351 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      520 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2528 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.473966 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       26 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.474449 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      232 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      480 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      309 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      678 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.474599 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.474865 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1577 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.475210 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      157 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      149 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      674 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.475356 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.476445 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      488 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3736 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      598 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2531 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1402 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      477 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.476609 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.477604 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1447 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      369 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      710 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      931 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      744 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.477768 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)   991302 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      679 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    14135 2023-05-18 05:39:43.000000 dagworks-sdk-0.0.4/src/dagworks/driver.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.480286 dagworks-sdk-0.0.4/src/dagworks/parsing/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/parsing/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2394 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/parsing/dagtypes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7810 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/parsing/parse.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.480636 dagworks-sdk-0.0.4/src/dagworks/telemetry/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7465 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.481289 dagworks-sdk-0.0.4/src/dagworks/tracking/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5969 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    10840 2023-05-18 05:35:23.000000 dagworks-sdk-0.0.4/src/dagworks/tracking/runs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2411 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/src/dagworks/tracking/trackingtypes.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.482030 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4695 2023-05-18 05:40:33.000000 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8551 2023-05-18 05:40:33.000000 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2023-05-18 05:40:33.000000 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       50 2023-05-18 05:40:33.000000 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      177 2023-05-18 05:40:33.000000 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        9 2023-05-18 05:40:33.000000 dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-05-18 05:40:33.482701 dagworks-sdk-0.0.4/tests/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2970 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/tests/test_driver.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5497 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/tests/test_runs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3343 2023-05-18 05:34:46.000000 dagworks-sdk-0.0.4/tests/test_telemetry.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6099 2023-05-18 05:39:43.000000 dagworks-sdk-0.0.4/tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.3/LICENSE` & `dagworks-sdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/PKG-INFO` & `dagworks-sdk-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.3/README.md` & `dagworks-sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/pyproject.toml` & `dagworks-sdk-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 0, 3)
+__version__ = (0, 0, 4)
```

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/client.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/client.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/api_key_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/dependency.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/dependency.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_in.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_dag.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_function.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_function.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_node.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_dependencies.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_node_dependencies.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/hamilton_node_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/hamilton_node_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/organization_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/organization_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_api_key_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/paged_api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_project_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/paged_project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/paged_run_log_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/paged_run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/phone_home_result.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/phone_home_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_in_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_out_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_in_git.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_dag.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_in_git_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_in_git_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_in_git_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_version_info.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_with_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/python_type.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/python_type.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_data.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_data.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_config.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_inputs.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_run_log.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_run_log.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_in_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_config.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_inputs.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_config.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/task_run_result_summary.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/task_run_result_summary.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/user_out.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/user_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_full.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/visibility_full.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/visibility_in.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/visibility_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/models/who_am_i_result.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/models/who_am_i_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/api_client/types.py` & `dagworks-sdk-0.0.4/src/dagworks/api/api_client/types.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/clients.py` & `dagworks-sdk-0.0.4/src/dagworks/api/clients.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/constants.py` & `dagworks-sdk-0.0.4/src/dagworks/api/constants.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/api/projecttypes.py` & `dagworks-sdk-0.0.4/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/cli.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/initialize.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/common/run.sh.jinja2` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/iris_loader.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks-sdk-0.0.4/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/driver.py` & `dagworks-sdk-0.0.4/src/dagworks/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,25 +147,29 @@
         commit_hash=commit.hexsha,
         committed=not repo.is_dirty(),
         repository=repo_url,
         local_repo_base_path=repo.working_dir,
     )
 
 
-def filter_config_to_json_serializable(config: Dict[str, Any], curr_result: Dict[str, Any] = None):
+def filter_json_dict_to_serializable(
+    dict_to_filter: Dict[str, Any], curr_result: Dict[str, Any] = None
+):
     if curr_result is None:
         curr_result = {}
-    for key, value in config.items():
+    if dict_to_filter is None:
+        dict_to_filter = {}
+    for key, value in dict_to_filter.items():
         try:
             json.dumps(value)
             curr_result[key] = value
         except TypeError:
             if isinstance(value, dict):
                 new_result = {}
-                filter_config_to_json_serializable(value, new_result)
+                filter_json_dict_to_serializable(value, new_result)
                 curr_result[key] = new_result
             else:
                 curr_result[key] = str(value)
     return curr_result
 
 
 def validate_tags(tags: Any):
@@ -337,12 +341,12 @@
             except Exception as e:
                 tracking_state.clock_end(status=Status.FAILURE)
                 raise e
             finally:
                 self.client.log_dag_run(
                     tracking_state.get(),
                     self.project_version.id,
-                    config=filter_config_to_json_serializable(self.config),
+                    config=filter_json_dict_to_serializable(self.config),
                     tags=self.run_tags,
-                    inputs=filter_config_to_json_serializable(inputs),
+                    inputs=filter_json_dict_to_serializable(inputs),
                     outputs=final_vars,
                 )
```

### Comparing `dagworks-sdk-0.0.3/src/dagworks/parsing/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/parsing/dagtypes.py` & `dagworks-sdk-0.0.4/src/dagworks/parsing/dagtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/parsing/parse.py` & `dagworks-sdk-0.0.4/src/dagworks/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/telemetry/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/telemetry/telemetry.py` & `dagworks-sdk-0.0.4/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/tracking/__init__.py` & `dagworks-sdk-0.0.4/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/tracking/example_tracking.py` & `dagworks-sdk-0.0.4/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/tracking/runs.py` & `dagworks-sdk-0.0.4/src/dagworks/tracking/runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks/tracking/trackingtypes.py` & `dagworks-sdk-0.0.4/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.3/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks-sdk-0.0.4/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/tests/test_driver.py` & `dagworks-sdk-0.0.4/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/tests/test_runs.py` & `dagworks-sdk-0.0.4/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/tests/test_telemetry.py` & `dagworks-sdk-0.0.4/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.3/tests/test_tracking.py` & `dagworks-sdk-0.0.4/tests/test_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,11 +185,12 @@
 @pytest.mark.parametrize(
     "config,expected",
     [
         ({"foo": "bar"}, {"foo": "bar"}),
         ({"foo": NonSerializable()}, {"foo": "non-serializable-string-rep"}),
         ({"foo": {"bar": "baz"}}, {"foo": {"bar": "baz"}}),
         ({"foo": {"bar": NonSerializable()}}, {"foo": {"bar": "non-serializable-string-rep"}}),
+        (None, {}),
     ],
 )
 def test_json_filter_config(config, expected):
-    assert driver.filter_config_to_json_serializable(config) == expected
+    assert driver.filter_json_dict_to_serializable(config) == expected
```

