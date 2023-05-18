# Comparing `tmp/dagster_cloud_cli-1.3.4.tar.gz` & `tmp/dagster_cloud_cli-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_cli-1.3.4.tar", last modified: Thu May 11 17:10:52 2023, max compression
+gzip compressed data, was "dagster_cloud_cli-1.3.5.tar", last modified: Thu May 18 20:49:53 2023, max compression
```

## Comparing `dagster_cloud_cli-1.3.4.tar` & `dagster_cloud_cli-1.3.5.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.447464 dagster_cloud_cli-1.3.4/
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-11 17:10:52.447464 dagster_cloud_cli-1.3.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.651465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.655465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.655465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.767465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    20512 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.815465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.883465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.931465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.947465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.947465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.951465 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.991464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    17767 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.051464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11997 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18291 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.163464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.199464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.219464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.279464 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9467 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13847 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)     5976 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5384 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6700 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:51.655465 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2807 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-11 17:10:51.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:10:52.383464 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3745 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    15025 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 17:10:52.447464 dagster_cloud_cli-1.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-11 16:59:00.000000 dagster_cloud_cli-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.253681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    24628 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.253681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.261681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.261681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    17755 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.261681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    11997 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18291 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.269681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.269681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.269681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.281681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13847 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6700 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    15513 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/setup.py
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,18 +26,24 @@
     dagster_cloud_options,
     get_location_document,
     get_org_url,
 )
 from dagster_cloud_cli.core import pex_builder, pydantic_yaml
 
 from .. import metrics
-from . import checks, state
+from . import checks, report, state
 
 app = Typer(hidden=True, help="CI/CD agnostic commands")
-from dagster_cloud_cli.core.pex_builder import code_location, deps, github_context, parse_workspace
+from dagster_cloud_cli.core.pex_builder import (
+    code_location,
+    deps,
+    github_context,
+    gitlab_context,
+    parse_workspace,
+)
 from dagster_cloud_cli.types import CliEventTags
 
 
 @app.command(help="Print json information about current CI/CD environment")
 def inspect(project_dir: str):
     project_dir = os.path.abspath(project_dir)
     source = metrics.get_source()
@@ -62,42 +68,69 @@
         " DAGSTER_CLOUD_API_TOKEN environment variables."
     )
 )
 def branch_deployment(
     project_dir: str,
     organization: Optional[str] = ORGANIZATION_OPTION,
     dagster_env: Optional[str] = DAGSTER_ENV_OPTION,
+    mark_closed: bool = False,
 ):
     try:
         if organization:
             url = get_org_url(organization, dagster_env)
         else:
             url = os.environ[URL_ENV_VAR_NAME]
-        print(get_deployment_from_context(url, project_dir))
+        print(get_deployment_from_context(url, project_dir, mark_closed))
     except ValueError as err:
         logging.error(
             f"cannot determine branch deployment: {err}",
         )
         sys.exit(1)
 
 
-def get_deployment_from_context(url, project_dir: str) -> str:
+def get_deployment_from_context(url, project_dir: str, mark_closed=False) -> str:
     source = metrics.get_source()
     if source == CliEventTags.source.github:
         event = github_context.get_github_event(project_dir)
         api_token = os.environ[TOKEN_ENV_VAR_NAME]
         deployment_name = code_location.create_or_update_branch_deployment_from_github_context(
-            url, api_token, event
+            url, api_token, event, mark_closed
         )
         if not deployment_name:
             raise ValueError(
                 f"could not determine branch deployment for PR {event.pull_request_id}"
             )
 
         return deployment_name
+    elif source == CliEventTags.source.gitlab:
+        event = gitlab_context.get_gitlab_event(project_dir)
+        if not event.merge_request_iid:
+            raise ValueError("no merge request id")
+        with gql.graphql_client_from_url(url, os.environ[TOKEN_ENV_VAR_NAME]) as client:
+            deployment_name = gql.create_or_update_branch_deployment(
+                client,
+                repo_name=event.project_name,
+                branch_name=event.branch_name,
+                commit_hash=event.commit_sha,
+                timestamp=float(event.git_metadata.timestamp),
+                branch_url=event.branch_url,
+                pull_request_url=event.merge_request_url,
+                pull_request_status=("CLOSED" if mark_closed else "OPEN"),
+                pull_request_number=event.merge_request_iid,
+                author_name=event.git_metadata.name,
+                author_email=event.git_metadata.email,
+                commit_message=event.git_metadata.message,
+            )
+            logging.info(
+                "Got branch deployment %r for branch %r",
+                deployment_name,
+                event.branch_name,
+            )
+            return deployment_name
+
     else:
         raise ValueError(f"unsupported for {source}")
 
 
 @app.command(help="Validate configuration")
 def check(
     organization: Optional[str] = ORGANIZATION_OPTION,
@@ -164,14 +197,15 @@
     project_dir: str = typer.Option("."),
     dagster_cloud_yaml_path: str = "dagster_cloud.yaml",
     statedir: str = STATEDIR_OPTION,
     clean_statedir: bool = typer.Option(True, help="Delete any existing files in statedir"),
     location_name: List[str] = typer.Option([]),
     git_url: Optional[str] = None,
     commit_hash: Optional[str] = None,
+    status_url: Optional[str] = None,
 ):
     yaml_path = pathlib.Path(project_dir) / dagster_cloud_yaml_path
     locations_def = pydantic_yaml.load_dagster_cloud_yaml(yaml_path.read_text())
     locations = locations_def.locations
     if location_name:
         selected_locations = set(location_name)
         unknown = selected_locations - set(location.location_name for location in locations)
@@ -211,32 +245,65 @@
             deployment_name=deployment,
             location_file=str(yaml_path.absolute()),
             location_name=location.location_name,
             build=state.BuildMetadata(
                 git_url=git_url, commit_hash=commit_hash, build_config=location.build
             ),
             build_output=None,
+            status_url=status_url,
         )
+        location_state.add_status_change(state.LocationStatus.pending, "initialized")
         state_store.save(location_state)
 
     ui.print(
         f"Initialized {statedir} to build and deploying following locations for directory"
         f" {project_dir}:"
     )
     for location in state_store.list_locations():
         ui.print(f"- {location.location_name}")
 
 
+class StatusOutputFormat(Enum):
+    json = "json"
+    markdown = "markdown"
+
+
 @app.command(help="Show status of the current build session")
 def status(
     statedir: str = STATEDIR_OPTION,
+    output_format: StatusOutputFormat = typer.Option("json", help="Output format for build status"),
 ):
     state_store = state.FileStore(statedir=statedir)
-    for location in state_store.list_locations():
-        ui.print(location.json())
+    location_states = state_store.list_locations()
+    if output_format == StatusOutputFormat.json:
+        for location in location_states:
+            ui.print(location.json())
+    elif output_format == StatusOutputFormat.markdown:
+        ui.print(report.markdown_report(location_states))
+
+
+@app.command(help="Update the PR comment with the latest status for branch deployments in Github.")
+def notify(
+    statedir: str = STATEDIR_OPTION,
+    project_dir: str = typer.Option("."),
+):
+    state_store = state.FileStore(statedir=statedir)
+    location_states = state_store.list_locations()
+
+    source = metrics.get_source()
+    if source == CliEventTags.source.github:
+        event = github_context.get_github_event(project_dir)
+        msg = "Your pull request is automatically being deployed to Dagster Cloud."
+        event.update_pr_comment(
+            msg + "\n\n" + report.markdown_report(location_states),
+            orig_author="github-actions[bot]",
+            orig_text=msg,
+        )
+    else:
+        raise ui.error("'dagster-cloud ci notify' is only available within Github actions.")
 
 
 @app.command(help="List locations in the current build session")
 def locations_list(
     statedir: str = STATEDIR_OPTION,
 ):
     state_store = state.FileStore(statedir=statedir)
@@ -341,95 +408,107 @@
     state_store = state.FileStore(statedir=statedir)
     locations = _get_selected_locations(state_store, location_name)
     ui.print("Going to build the following locations:")
     for name in locations:
         ui.print(f"- {name}")
 
     for name, location_state in locations.items():
-        configured_build_directory = (
-            location_state.build.build_config.directory
-            if (location_state.build.build_config and location_state.build.build_config.directory)
-            else None
-        )
-        if build_directory and configured_build_directory:
-            ui.warn(
-                f"Overriding configured build:directory:{configured_build_directory!r} with"
-                f" cmdline provided --build-directory={build_directory!r}"
-            )
-            location_build_dir = build_directory
-        elif (not build_directory) and configured_build_directory:
-            location_build_dir = configured_build_directory
-        elif build_directory and (not configured_build_directory):
-            location_build_dir = build_directory
-        else:
-            location_build_dir = "."
-
-        if build_strategy == BuildStrategy.docker:
-            if not docker_base_image:
-                docker_base_image = f"python:{python_version}-slim"
-
-            ui.print(
-                f"Building docker image for location {name} using base image {docker_base_image}"
-            )
-            docker_utils.verify_docker()
-            registry_info = utils.get_registry_info(location_state.url)
-
-            docker_image_tag = docker_utils.default_image_tag(
-                location_state.deployment_name, name, location_state.build.commit_hash
-            )
-
-            retval = docker_utils.build_image(
-                location_build_dir,
-                docker_image_tag,
-                registry_info,
-                env_vars=docker_env,
-                base_image=docker_base_image,
-            )
-            if retval != 0:
-                raise ui.error(f"Failed to build docker image for location {name}")
-
-            retval = docker_utils.upload_image(docker_image_tag, registry_info)
-            if retval != 0:
-                raise ui.error(f"Failed to upload docker image for location {name}")
-
-            image = f'{registry_info["registry_url"]}:{docker_image_tag}'
-
-            # Update and save build state
-            location_state.build_output = state.DockerBuildOutput(image=image)
+        try:
+            configured_build_directory = (
+                location_state.build.build_config.directory
+                if (
+                    location_state.build.build_config
+                    and location_state.build.build_config.directory
+                )
+                else None
+            )
+            if build_directory and configured_build_directory:
+                ui.warn(
+                    f"Overriding configured build:directory:{configured_build_directory!r} with"
+                    f" cmdline provided --build-directory={build_directory!r}"
+                )
+                location_build_dir = build_directory
+            elif (not build_directory) and configured_build_directory:
+                location_build_dir = configured_build_directory
+            elif build_directory and (not configured_build_directory):
+                location_build_dir = build_directory
+            else:
+                location_build_dir = "."
+
+            if build_strategy == BuildStrategy.docker:
+                if not docker_base_image:
+                    docker_base_image = f"python:{python_version}-slim"
+
+                ui.print(
+                    f"Building docker image for location {name} using base image"
+                    f" {docker_base_image}"
+                )
+                docker_utils.verify_docker()
+                registry_info = utils.get_registry_info(location_state.url)
+
+                docker_image_tag = docker_utils.default_image_tag(
+                    location_state.deployment_name, name, location_state.build.commit_hash
+                )
+
+                retval = docker_utils.build_image(
+                    location_build_dir,
+                    docker_image_tag,
+                    registry_info,
+                    env_vars=docker_env,
+                    base_image=docker_base_image,
+                )
+                if retval != 0:
+                    raise ui.error(f"Failed to build docker image for location {name}")
+
+                retval = docker_utils.upload_image(docker_image_tag, registry_info)
+                if retval != 0:
+                    raise ui.error(f"Failed to upload docker image for location {name}")
+
+                image = f'{registry_info["registry_url"]}:{docker_image_tag}'
+
+                # Update and save build state
+                location_state.build_output = state.DockerBuildOutput(image=image)
+                state_store.save(location_state)
+                ui.print(f"Built and uploaded image {image} for location {name}")
+            elif build_strategy == BuildStrategy.pex:
+                pex_location = parse_workspace.Location(
+                    name,
+                    directory=location_build_dir,
+                    build_folder=location_build_dir,
+                    location_file=location_state.location_file,
+                )
+                location_kwargs = pex_utils.build_upload_pex(
+                    url=location_state.url,
+                    api_token=os.environ[TOKEN_ENV_VAR_NAME],
+                    location=pex_location,
+                    build_method=pex_build_method,
+                    kwargs={
+                        "python_version": python_version,
+                        "base_image_tag": pex_base_image_tag,
+                        "deps_cache_from": pex_deps_cache_from,
+                        "deps_cache_to": pex_deps_cache_to,
+                    },
+                )
+                location_state.build_output = state.PexBuildOutput(
+                    python_version=python_version,
+                    image=location_kwargs["image"],
+                    pex_tag=location_kwargs["pex_tag"],
+                )
+                state_store.save(location_state)
+                ui.print(
+                    "Built and uploaded python executable"
+                    f" {location_state.build_output.pex_tag} for location {name}"
+                )
+        except:
+            location_state.add_status_change(state.LocationStatus.failed, "build failed")
             state_store.save(location_state)
-            ui.print(f"Built and uploaded image {image} for location {name}")
-        elif build_strategy == BuildStrategy.pex:
-            pex_location = parse_workspace.Location(
-                name,
-                directory=location_build_dir,
-                build_folder=location_build_dir,
-                location_file=location_state.location_file,
-            )
-            location_kwargs = pex_utils.build_upload_pex(
-                url=location_state.url,
-                api_token=os.environ[TOKEN_ENV_VAR_NAME],
-                location=pex_location,
-                build_method=pex_build_method,
-                kwargs={
-                    "python_version": python_version,
-                    "base_image_tag": pex_base_image_tag,
-                    "deps_cache_from": pex_deps_cache_from,
-                    "deps_cache_to": pex_deps_cache_to,
-                },
-            )
-            location_state.build_output = state.PexBuildOutput(
-                python_version=python_version,
-                image=location_kwargs["image"],
-                pex_tag=location_kwargs["pex_tag"],
-            )
+            raise
+        else:
+            location_state.add_status_change(state.LocationStatus.pending, "build successful")
             state_store.save(location_state)
-            ui.print(
-                f"Build and uploaded python executable {location_state.build_output.pex_tag} for"
-                f" location {name}"
-            )
 
 
 @app.command(help="Update the current build session for an externally built docker image.")
 def set_build_output(
     statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
     location_name: List[str] = typer.Option([]),
     image_tag: str = typer.Option(
@@ -480,15 +559,15 @@
     location_load_timeout: int = LOCATION_LOAD_TIMEOUT_OPTION,
     agent_heartbeat_timeout: int = AGENT_HEARTBEAT_TIMEOUT_OPTION,
 ):
     state_store = state.FileStore(statedir=statedir)
     locations = _get_selected_locations(state_store, location_name)
     ui.print("Going deploy the following locations:")
 
-    built_locations = []
+    built_locations: List[state.LocationState] = []
     for name, location_state in locations.items():
         if location_state.build_output:
             status = "Ready to deploy"
             built_locations.append(location_state)
         else:
             status = "Not ready to deploy"
         ui.print(f"- {name} [{status}]")
@@ -500,14 +579,17 @@
         )
 
     if not built_locations:
         ui.print("No locations to deploy")
         return
 
     for location_state in built_locations:
+        if not location_state.build_output:  # not necessary but keep type checker happy
+            continue
+
         location_args = {
             "image": location_state.build_output.image,
             "location_file": location_state.location_file,
             "git_url": location_state.build.git_url,
             "commit_hash": location_state.build.commit_hash,
         }
         if location_state.build_output.strategy == "python-executable":
@@ -517,16 +599,27 @@
             gql.add_or_update_code_location(client, location_document)
             ui.print(f"Updated code location {location_state.location_name} in dagster-cloud")
 
     url = built_locations[0].url + "/" + built_locations[0].deployment_name
     with utils.client_from_env(
         built_locations[0].url, deployment=built_locations[0].deployment_name
     ) as client:
-        wait_for_load(
-            client,
-            [location.location_name for location in built_locations],
-            location_load_timeout=location_load_timeout,
-            agent_heartbeat_timeout=agent_heartbeat_timeout,
-            url=url,
-        )
+        try:
+            wait_for_load(
+                client,
+                [location.location_name for location in built_locations],
+                location_load_timeout=location_load_timeout,
+                agent_heartbeat_timeout=agent_heartbeat_timeout,
+                url=url,
+            )
+        except:
+            # unfortunately we do not know if only a subset of locations failed to deploy
+            for location_state in built_locations:
+                location_state.add_status_change(state.LocationStatus.failed, "deploy failed")
+                state_store.save(location_state)
+            raise
+        else:
+            for location_state in built_locations:
+                location_state.add_status_change(state.LocationStatus.success, "deploy successful")
+                state_store.save(location_state)
 
     ui.print(f"View the status of your locations at {url}/locations.")
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/checks.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/ci/state.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import datetime
 import json
 import os
 from abc import ABCMeta, abstractmethod
+from enum import Enum
 from typing import List, Literal, Optional, Union
 
 from pydantic import BaseModel, Extra, Field
 
 from dagster_cloud_cli.core import pydantic_yaml
 
 
@@ -23,25 +25,48 @@
 
 class BuildMetadata(BaseModel):
     git_url: Optional[str]
     commit_hash: Optional[str]
     build_config: Optional[pydantic_yaml.Build]  # copied from dagster_cloud.yaml
 
 
+class LocationStatus(Enum):
+    success = "success"
+    pending = "pending"
+    failed = "failed"
+
+
+class StatusChange(BaseModel):
+    timestamp: datetime.datetime
+    status: LocationStatus
+    log: str
+
+
 class LocationState(BaseModel, extra=Extra.forbid):
     # we intentionally don't save api_token here for security reasons
     url: str
     deployment_name: str
     location_file: str
     location_name: str
     selected: bool = True
     build: BuildMetadata
     build_output: Optional[Union[DockerBuildOutput, PexBuildOutput]] = Field(
         None, discriminator="strategy"
     )
+    status_url: Optional[str]  # link to cicd run url when building and dagster cloud url when done
+    history: List[StatusChange] = []
+
+    def add_status_change(self, status: LocationStatus, log: str):
+        self.history.append(
+            StatusChange(
+                timestamp=datetime.datetime.now(datetime.timezone.utc),
+                status=status,
+                log=log,
+            )
+        )
 
 
 class Store(metaclass=ABCMeta):
     @abstractmethod
     def load(self, location_name: str) -> LocationState:
         ...
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/config.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/job/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/metrics.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/run/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,19 +207,17 @@
     env_vars = kwargs.get("env", [])
     base_image = kwargs.get("base_image")
 
     with gql.graphql_client_from_url(url, api_token) as client:
         ecr_info = gql.get_ecr_info(client)
         registry = ecr_info["registry_url"]
 
-        image_tag = kwargs.get(
-            "image",
-            docker_utils.default_image_tag(deployment, location_name, kwargs.get("commit_hash")),
+        image_tag = kwargs.get("image") or docker_utils.default_image_tag(
+            deployment, location_name, kwargs.get("commit_hash")
         )
-
         retval = docker_utils.build_image(
             source_directory, image_tag, ecr_info, env_vars, base_image
         )
         if retval != 0:
             return
 
         retval = docker_utils.upload_image(image_tag, ecr_info)
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/config_utils.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/docker_runner.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/errors.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/graphql_client.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/headers/impl.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from . import github_context
 
 
 def create_or_update_branch_deployment_from_github_context(
     dagster_cloud_org_url: str,
     dagster_cloud_api_token: str,
     github_event: github_context.GithubEvent,
+    mark_closed: bool,
 ) -> Optional[str]:
     """Return the branch deployment associated with the github PR."""
     event = github_event
     logging.debug("Read github event GithubEvent(%r)", event.__dict__)
     if not event.branch_name:
         logging.info("Not in a branch, not creating branch deployment")
         return None
@@ -24,15 +25,15 @@
                 client,
                 repo_name=event.repo_name,
                 branch_name=event.branch_name,
                 commit_hash=event.github_sha,
                 timestamp=event.timestamp,
                 branch_url=event.branch_url,
                 pull_request_url=event.pull_request_url,
-                pull_request_status=event.pull_request_status,
+                pull_request_status="CLOSED" if mark_closed else event.pull_request_status,
                 pull_request_number=event.pull_request_id,
                 author_name=event.author_name,
                 author_email=event.author_email,
                 commit_message=event.commit_msg,
                 author_avatar_url=github_event.get_github_avatar_url(),
             )
         logging.info(
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,26 +57,57 @@
 
         git_metadata = get_git_commit_metadata(project_dir)
         self.timestamp = float(git_metadata["timestamp"])
         self.commit_msg = git_metadata["message"]
         self.author_name = git_metadata["name"]
         self.author_email = git_metadata["email"]
 
-    def get_github_avatar_url(self) -> Optional[str]:
+    def get_github_repo(self):
         import github3
 
         token = os.getenv("GITHUB_TOKEN")
         if not token:
             return None
         gh = github3.login(token=token)
         repo_owner, repo_name = self.github_repository.split("/", 1)
-        repo = gh.repository(repo_owner, repo_name)
+        return gh.repository(repo_owner, repo_name)
+
+    def get_github_avatar_url(self) -> Optional[str]:
+        repo = self.get_github_repo()
+        if not repo:
+            return
         commit = repo.commit(self.github_sha)
         return commit.author.get("avatar_url") if commit.author else None
 
+    def update_pr_comment(
+        self, body: str, orig_author: Optional[str] = None, orig_text: Optional[str] = None
+    ):
+        # orig_author and orig_text are used to identify an existing comment which is updated.
+        # if not provided, or not found, a new comment is created
+        import github3.exceptions
+
+        if not self.pull_request_id:
+            return
+
+        try:
+            repo = self.get_github_repo()
+            if not repo:
+                return
+            pr = repo.pull_request(int(self.pull_request_id))
+
+            for comment in pr.issue_comments():
+                if comment.user.login == orig_author and orig_text in comment.body:
+                    comment.edit(body)
+                    return
+
+            pr.create_comment(body)
+
+        except github3.exceptions.GitHubException:
+            logging.exception("Ignoring error when updating PR comment")
+
 
 def get_git_commit_metadata(project_dir: str) -> Dict[str, str]:
     commands = {
         "timestamp": f"git -C {project_dir} log -1 --format=%cd --date=unix".split(),
         "message": f"git -C {project_dir} log -1 --format=%s".split(),
         "email": f"git -C {project_dir} log -1 --format=%ae".split(),
         "name": f"git -C {project_dir} log -1 --format=%an".split(),
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/source.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pex_builder/util.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/core/workspace.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/docker_utils.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/entrypoint.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/gql.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/pex_utils.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/types.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/ui.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli/utils.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 dagster_cloud_cli.egg-info/top_level.txt
 dagster_cloud_cli/commands/__init__.py
 dagster_cloud_cli/commands/config.py
 dagster_cloud_cli/commands/metrics.py
 dagster_cloud_cli/commands/branch_deployment/__init__.py
 dagster_cloud_cli/commands/ci/__init__.py
 dagster_cloud_cli/commands/ci/checks.py
+dagster_cloud_cli/commands/ci/report.py
 dagster_cloud_cli/commands/ci/state.py
 dagster_cloud_cli/commands/ci/utils.py
 dagster_cloud_cli/commands/deployment/__init__.py
 dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
 dagster_cloud_cli/commands/deployment/alert_policies/commands.py
 dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
 dagster_cloud_cli/commands/job/__init__.py
@@ -49,15 +50,17 @@
 dagster_cloud_cli/core/headers/impl.py
 dagster_cloud_cli/core/headers/versioning/__init__.py
 dagster_cloud_cli/core/headers/versioning/constants.py
 dagster_cloud_cli/core/pex_builder/__init__.py
 dagster_cloud_cli/core/pex_builder/code_location.py
 dagster_cloud_cli/core/pex_builder/deploy.py
 dagster_cloud_cli/core/pex_builder/deps.py
+dagster_cloud_cli/core/pex_builder/git_context.py
 dagster_cloud_cli/core/pex_builder/github_context.py
+dagster_cloud_cli/core/pex_builder/gitlab_context.py
 dagster_cloud_cli/core/pex_builder/parse_workspace.py
 dagster_cloud_cli/core/pex_builder/pex_registry.py
 dagster_cloud_cli/core/pex_builder/selftest.py
 dagster_cloud_cli/core/pex_builder/source.py
 dagster_cloud_cli/core/pex_builder/util.py
 dagster_cloud_cli_tests/__init__.py
 dagster_cloud_cli_tests/conftest.py
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_check.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,36 +61,41 @@
                 [
                     "ci",
                     "init",
                     f"--project-dir={project_dir}",
                     "--deployment=prod",
                     "--commit-hash=hash-1234",
                     "--git-url=http://some-git-url",
+                    "--status-url=http://github/run-url",
                 ],
             )
             assert not result.exit_code
 
             # 'status' should return a list of code locations
             result = runner.invoke(app, ["ci", "status"])
             assert not result.exit_code
             locations = [json.loads(line) for line in result.output.splitlines()]
             assert ["a", "b", "c"] == [loc["location_name"] for loc in locations]
             location_a = locations[0]
+            # overwrite test timestamp
+            location_a["history"][0]["timestamp"] = "-"
             assert location_a == {
                 "build": {
                     "build_config": None,
                     "commit_hash": "hash-1234",
                     "git_url": "http://some-git-url",
                 },
                 "build_output": None,
                 "location_name": "a",
                 "deployment_name": "prod",
                 "location_file": f"{project_dir}/dagster_cloud.yaml",
                 "selected": True,
                 "url": "https://some-org.dagster.cloud",
+                "history": [{"log": "initialized", "status": "pending", "timestamp": "-"}],
+                "status_url": "http://github/run-url",
             }
 
         with with_dagster_yaml(DAGSTER_CLOUD_YAML) as project_dir:
             runner = CliRunner()
             monkeypatch.setenv("DAGSTER_BUILD_STATEDIR", statedir)
             result = runner.invoke(
                 app,
@@ -283,14 +288,19 @@
         "location_name": "c",
         "working_directory": "c",
     }
     (_, wait_location_args), wait_kwargs = wait_for_load.call_args_list[0]
     assert wait_location_args == ["b", "c"]
     assert wait_kwargs["url"] == f"https://some-org.dagster.cloud/{deployment_name}"
 
+    # first location (a) is deselected
+    assert [
+        location["history"][-1]["status"] for location in get_locations(initialized_runner)
+    ] == ["pending", "success", "success"]
+
 
 def test_ci_set_build_output(initialized_runner: CliRunner):
     result = initialized_runner.invoke(app, ["ci", "set-build-output", "--image-tag=1234"])
     assert result.exit_code
     assert "Error: No build:registry:" in result.output
 
     initialized_runner.invoke(app, ["ci", "locations-deselect", "a", "b"])
```

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_gql.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/dagster_cloud_cli_tests/test_metrics.py` & `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.4/setup.py` & `dagster_cloud_cli-1.3.5/setup.py`

 * *Files identical despite different names*

