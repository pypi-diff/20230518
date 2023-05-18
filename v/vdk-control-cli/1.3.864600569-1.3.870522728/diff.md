# Comparing `tmp/vdk-control-cli-1.3.864600569.tar.gz` & `tmp/vdk-control-cli-1.3.870522728.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.864600569.tar", last modified: Thu May 11 15:33:38 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.870522728.tar", last modified: Thu May 18 10:11:44 2023, max compression
```

## Comparing `vdk-control-cli-1.3.864600569.tar` & `vdk-control-cli-1.3.870522728.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    11236 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14329 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5115 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12198 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-05-11 15:33:21.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-11 15:33:25.000000 vdk-control-cli-1.3.864600569/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2371 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-11 15:33:38.000000 vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-11 15:33:25.000000 vdk-control-cli-1.3.864600569/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    11236 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14329 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12200 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9834 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-18 10:11:33.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-18 10:11:33.000000 vdk-control-cli-1.3.870522728/version.txt
```

### Comparing `vdk-control-cli-1.3.864600569/PKG-INFO` & `vdk-control-cli-1.3.870522728/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.864600569
+Version: 1.3.870522728
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.864600569/README.md` & `vdk-control-cli-1.3.870522728/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/setup.cfg` & `vdk-control-cli-1.3.870522728/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 install_requires = 
 	click==8.*
 	click-log==0.*
 	click-spinner==0.*
 	requests>=2.25
 	setuptools>=47.0
 	pluggy
-	vdk-control-service-api==1.0.9
+	vdk-control-service-api==1.0.10
 	tabulate
 	requests_oauthlib>=1.0
 	urllib3>=1.26.5
 	vdk-control-api-auth
 python_requires = >=3.7, <4
 
 [options.packages.find]
```

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import os
 
 import click
 import click_spinner
-from urllib3 import HTTPResponse
+from taurus_datajob_api import ApiResponse
 from vdk.internal.control.configuration.defaults_config import load_default_team_name
 from vdk.internal.control.exception.vdk_exception import VDKException
 from vdk.internal.control.job.job_archive import JobArchive
 from vdk.internal.control.rest_lib.factory import ApiClientFactory
 from vdk.internal.control.rest_lib.rest_client_errors import ApiClientErrorDecorator
 from vdk.internal.control.utils import cli_utils
 
@@ -25,31 +25,31 @@
     def download(self, team: str, name: str, path: str):
         log.debug(f"Download job {name} of team {team} into parent {path}")
         self.__validate_job_path(path, name)
         job_archive_path = os.path.join(path, f"{name}.zip")
         try:
             log.info(f"Downloading data job {name} in {path}/{name} ...")
             with click_spinner.spinner():
-                response: HTTPResponse = self.sources_api.data_job_sources_download(
+                response = self.sources_api.data_job_sources_download_with_http_info(
                     team_name=team, job_name=name, _preload_content=False
                 )
                 self.__write_response_to_archive(job_archive_path, response)
                 self.__job_archive.unarchive_data_job(
                     job_name=name, job_archive_path=job_archive_path, job_directory=path
                 )
 
             log.info(f"Downloaded Data Job in {path}/{name}")
         finally:
             self.__cleanup_archive(job_archive_path)
 
     @staticmethod
-    def __write_response_to_archive(job_archive_path: str, response: HTTPResponse):
+    def __write_response_to_archive(job_archive_path: str, response: ApiResponse):
         log.debug(f"Write data job source to {job_archive_path}")
         with open(job_archive_path, "wb") as w:
-            w.write(response.data)
+            w.write(response.raw_data)
 
     @staticmethod
     def __validate_job_path(path: str, name: str):
         job_path = os.path.join(path, name)
         if os.path.exists(job_path):
             raise VDKException(
                 what=f"Cannot download data job source at given job path: {path}",
```

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 class JobDownloadKey:
     def __init__(self, rest_api_url: str):
         self.jobs_api = ApiClientFactory(rest_api_url).get_jobs_api()
 
     @ApiClientErrorDecorator()
     def download(self, team: str, name: str, path: str):
         keytab_file_path = os.path.join(path, f"{name}.keytab")
-        response: HTTPResponse = self.jobs_api.data_job_keytab_download(
+        response = self.jobs_api.data_job_keytab_download_with_http_info(
             team_name=team, job_name=name, _preload_content=False
         )
         with open(keytab_file_path, "wb") as w:
-            w.write(response.data)
+            w.write(response.raw_data)
         log.info(f"Saved keytab in {keytab_file_path}")
 
 
 # Below is the definition of the CLI API/UX users will be interacting
 # Above is the actual implementation of the operations
```

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,20 @@
         self, name: str, team: str, output_format: OutputFormat, arguments: str
     ) -> None:
         execution_request = DataJobExecutionRequest(
             started_by=f"vdk-control-cli",
             args=self.__validate_and_parse_args(arguments),
         )
         log.debug(f"Starting job with request {execution_request}")
-        _, _, headers = self.__execution_api.data_job_execution_start_with_http_info(
+        headers = self.__execution_api.data_job_execution_start_with_http_info(
             team_name=team,
             job_name=name,
             deployment_id="production",  # TODO
             data_job_execution_request=execution_request,
-        )
+        ).headers
         log.debug(f"Received headers: {headers}")
 
         location = headers["Location"]
         execution_id = os.path.basename(location)
         if output_format == OutputFormat.TEXT.value:
             click.echo(
                 f"Execution of Data Job {name} started. "
```

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.864600569
+Version: 1.3.870522728
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.864600569/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

