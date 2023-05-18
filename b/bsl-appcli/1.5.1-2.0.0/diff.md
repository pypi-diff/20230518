# Comparing `tmp/bsl-appcli-1.5.1.tar.gz` & `tmp/bsl-appcli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-appcli-1.5.1.tar", last modified: Thu Apr 20 02:16:52 2023, max compression
+gzip compressed data, was "bsl-appcli-2.0.0.tar", last modified: Thu May 18 03:23:35 2023, max compression
```

## Comparing `bsl-appcli-1.5.1.tar` & `bsl-appcli-2.0.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.822760 bsl-appcli-1.5.1/appcli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.822760 bsl-appcli-1.5.1/appcli/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/backup_manager/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/backup_manager/remote_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/cli_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.822760 bsl-appcli-1.5.1/appcli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/appcli_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/backup_manager_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/configure_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/configure_template_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/debug_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/encrypt_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/init_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/install_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/launcher_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/migrate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/service_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/task_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/commands/version_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.822760 bsl-appcli-1.5.1/appcli/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/common/data_class_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.822760 bsl-appcli-1.5.1/appcli/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/configuration/configuration_dir_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.822760 bsl-appcli-1.5.1/appcli/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/crypto/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/crypto/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/appcli/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/git_repositories/git_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/keycloak_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/appcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/models/cli_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/orchestrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/appcli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/templates/installer.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/templates/launcher.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/appcli/variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/bsl_appcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-04-20 02:16:52.000000 bsl-appcli-1.5.1/bsl_appcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-20 02:16:52.000000 bsl-appcli-1.5.1/bsl_appcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 02:16:52.000000 bsl-appcli-1.5.1/bsl_appcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 02:16:52.000000 bsl-appcli-1.5.1/bsl_appcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 02:16:52.000000 bsl-appcli-1.5.1/bsl_appcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.818760 bsl-appcli-1.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/backup_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/backup_manager/test_backup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/cipher/test_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.814760 bsl-appcli-1.5.1/tests/commands/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.814760 bsl-appcli-1.5.1/tests/commands/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.814760 bsl-appcli-1.5.1/tests/commands/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/commands/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/commands/test_install_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/commands_task/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.814760 bsl-appcli-1.5.1/tests/commands_task/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.814760 bsl-appcli-1.5.1/tests/commands_task/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.814760 bsl-appcli-1.5.1/tests/commands_task/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/commands_task/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/commands_task/test_commands_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/configuration/test_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/configuration_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.818760 bsl-appcli-1.5.1/tests/configuration_manager/expected_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/configuration_manager/expected_generated/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.818760 bsl-appcli-1.5.1/tests/configuration_manager/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.818760 bsl-appcli-1.5.1/tests/configuration_manager/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.818760 bsl-appcli-1.5.1/tests/configuration_manager/resources/templates/baseline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/configuration_manager/resources/templates/baseline/nesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/configuration_manager/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/configuration_state/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/configuration_state/test_configuration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/crypto/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/git_repositories/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/git_repositories/test_git_repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/string_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/string_transformer/test_string_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/variables_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/variables_manager/test_variables_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:16:52.826760 bsl-appcli-1.5.1/tests/version/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-20 02:15:57.000000 bsl-appcli-1.5.1/tests/version/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/cli_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/init_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/install_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/service_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/task_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/commands/version_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/common/data_class_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/keycloak_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/models/cli_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/orchestrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/appcli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/templates/installer.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/templates/launcher.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/appcli/variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/bsl_appcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 03:23:35.000000 bsl-appcli-2.0.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/backup_manager/test_backup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/cipher/test_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands/test_install_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands_task/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands_task/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands_task/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/commands_task/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/commands_task/test_commands_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/expected_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.627364 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.631364 bsl-appcli-2.0.0/tests/configuration_state/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/configuration_state/test_configuration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/crypto/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/git_repositories/test_git_repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/string_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/string_transformer/test_string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/variables_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/variables_manager/test_variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:23:35.635365 bsl-appcli-2.0.0/tests/version/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-18 03:22:45.000000 bsl-appcli-2.0.0/tests/version/test_version.py
```

### Comparing `bsl-appcli-1.5.1/LICENSE` & `bsl-appcli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/PKG-INFO` & `bsl-appcli-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 1.5.1
+Version: 2.0.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `bsl-appcli-1.5.1/README.md` & `bsl-appcli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/backup_manager/backup_manager.py` & `bsl-appcli-2.0.0/appcli/backup_manager/backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/backup_manager/remote_strategy.py` & `bsl-appcli-2.0.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/cli_builder.py` & `bsl-appcli-2.0.0/appcli/cli_builder.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/appcli_command.py` & `bsl-appcli-2.0.0/appcli/commands/appcli_command.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/backup_manager_cli.py` & `bsl-appcli-2.0.0/appcli/commands/backup_manager_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/configure_cli.py` & `bsl-appcli-2.0.0/appcli/commands/configure_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/configure_template_cli.py` & `bsl-appcli-2.0.0/appcli/commands/configure_template_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/debug_cli.py` & `bsl-appcli-2.0.0/appcli/commands/debug_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/encrypt_cli.py` & `bsl-appcli-2.0.0/appcli/commands/encrypt_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/init_cli.py` & `bsl-appcli-2.0.0/appcli/commands/init_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/install_cli.py` & `bsl-appcli-2.0.0/appcli/commands/install_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/launcher_cli.py` & `bsl-appcli-2.0.0/appcli/commands/launcher_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/migrate_cli.py` & `bsl-appcli-2.0.0/appcli/commands/migrate_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/service_cli.py` & `bsl-appcli-2.0.0/appcli/commands/service_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/task_cli.py` & `bsl-appcli-2.0.0/appcli/commands/task_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/commands/version_cli.py` & `bsl-appcli-2.0.0/appcli/commands/version_cli.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/common/data_class_extensions.py` & `bsl-appcli-2.0.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/configuration/configuration_dir_state.py` & `bsl-appcli-2.0.0/appcli/configuration/configuration_dir_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             error_and_exit(self.disallowed_command[command])
         if command in self.disallowed_command_unless_forced and not force:
             error_and_exit(
                 f"{self.disallowed_command_unless_forced[command]}"
                 " If this command supports it, use '--force' to ignore error."
             )
         logger.debug(
-            f"Allowed command [{command}] with current configuration state [{self}], where force is [{force}]."
+            f"Allowed command [{command}] with current configuration state [{self.__class__.__name__}], where force is [{force}]."
         )
 
 
 class ConfigurationDirStateFactory:
     """Factory class to get the current ConfigurationDirState state class"""
 
     def get_state(
```

### Comparing `bsl-appcli-1.5.1/appcli/configuration_manager.py` & `bsl-appcli-2.0.0/appcli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/crypto/cipher.py` & `bsl-appcli-2.0.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/crypto/crypto.py` & `bsl-appcli-2.0.0/appcli/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/functions.py` & `bsl-appcli-2.0.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/git_repositories/git_repositories.py` & `bsl-appcli-2.0.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/keycloak_manager.py` & `bsl-appcli-2.0.0/appcli/keycloak_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/logger.py` & `bsl-appcli-2.0.0/appcli/logger.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/models/cli_context.py` & `bsl-appcli-2.0.0/appcli/models/cli_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,17 @@
             ConfigurationDirStateFactory.get_state(
                 self.configuration_dir,
                 generated_configuration_dir,
                 self.app_version,
                 self.backup_dir,
             )
         )
-        logger.debug(f"Derived configuration state [{configuration_dir_state}]")
+        logger.debug(
+            f"Derived configuration state [{configuration_dir_state.__class__.__name__}]"
+        )
         return configuration_dir_state
 
     def get_key_file(self) -> Path:
         """Get the location of the key file for decrypting secrets
 
         Returns:
             Path: location of the key file
```

### Comparing `bsl-appcli-1.5.1/appcli/models/configuration.py` & `bsl-appcli-2.0.0/appcli/models/configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/orchestrators.py` & `bsl-appcli-2.0.0/appcli/orchestrators.py`

 * *Files 0% similar despite different names*

```diff
@@ -743,15 +743,15 @@
             logger.error(
                 "Command failed - stdout:\n%s",
                 textwrap.indent(result.stdout.decode("utf-8"), "    "),
             )
         if result.stderr:
             logger.error(
                 "Command failed - stderr:\n%s",
-                textwrap.indent(result.stdout.decode("utf-8"), "    "),
+                textwrap.indent(result.stderr.decode("utf-8"), "    "),
             )
     # For normal exits, just debug log the stdout if present.
     elif result.stdout:
         logger.debug(
             "Command output:\n%s",
             textwrap.indent(result.stdout.decode("utf-8"), "    "),
         )
```

### Comparing `bsl-appcli-1.5.1/appcli/string_transformer.py` & `bsl-appcli-2.0.0/appcli/string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/templates/installer.j2` & `bsl-appcli-2.0.0/appcli/templates/installer.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/templates/launcher.j2` & `bsl-appcli-2.0.0/appcli/templates/launcher.j2`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/appcli/variables_manager.py` & `bsl-appcli-2.0.0/appcli/variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/bsl_appcli.egg-info/PKG-INFO` & `bsl-appcli-2.0.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 1.5.1
+Version: 2.0.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `bsl-appcli-1.5.1/bsl_appcli.egg-info/SOURCES.txt` & `bsl-appcli-2.0.0/bsl_appcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/setup.py` & `bsl-appcli-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,23 +53,23 @@
     license="MIT License",
     author="brightSPARK Labs",
     author_email="enquire@brightsparklabs.com",
     url="https://www.brightsparklabs.com",
     packages=find_namespace_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "boto3==1.26.104",
+        "boto3==1.26.123",
         "click==8.1.3",
         "coloredlogs==15.0.1",
         "cronex==0.1.3.1",
         "dataclasses-json==0.5.7",
         "deepdiff==6.3.0",
         "GitPython==3.1.31",
         "jinja2==3.1.2",
-        "pre-commit==3.2.1",
+        "pre-commit==3.2.2",
         "pycryptodome==3.17",
         "pydantic==1.10.7",
         "python-keycloak==0.22.0",
         "python-slugify==8.0.1",
         "ruamel-yaml==0.17.21",
         "tabulate==0.9.0",
         "wheel==0.40.0",
```

### Comparing `bsl-appcli-1.5.1/tests/backup_manager/test_backup_manager.py` & `bsl-appcli-2.0.0/tests/backup_manager/test_backup_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/cipher/test_cipher.py` & `bsl-appcli-2.0.0/tests/cipher/test_cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/commands/test_commands.py` & `bsl-appcli-2.0.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/commands/test_install_script.py` & `bsl-appcli-2.0.0/tests/commands/test_install_script.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/commands_task/test_commands_task.py` & `bsl-appcli-2.0.0/tests/commands_task/test_commands_task.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/configuration/test_configuration.py` & `bsl-appcli-2.0.0/tests/configuration/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/configuration_manager/test_configuration_manager.py` & `bsl-appcli-2.0.0/tests/configuration_manager/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/configuration_state/test_configuration_state.py` & `bsl-appcli-2.0.0/tests/configuration_state/test_configuration_state.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/crypto/test_crypto.py` & `bsl-appcli-2.0.0/tests/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/git_repositories/test_git_repositories.py` & `bsl-appcli-2.0.0/tests/git_repositories/test_git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/string_transformer/test_string_transformer.py` & `bsl-appcli-2.0.0/tests/string_transformer/test_string_transformer.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/variables_manager/test_variables_manager.py` & `bsl-appcli-2.0.0/tests/variables_manager/test_variables_manager.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.5.1/tests/version/test_version.py` & `bsl-appcli-2.0.0/tests/version/test_version.py`

 * *Files identical despite different names*

