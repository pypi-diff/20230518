# Comparing `tmp/ha-services-0.2.0rc1.tar.gz` & `tmp/ha-services-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-services-0.2.0rc1.tar", last modified: Wed May 17 15:25:02 2023, max compression
+gzip compressed data, was "ha-services-0.2.0rc2.tar", last modified: Thu May 18 06:34:09 2023, max compression
```

## Comparing `ha-services-0.2.0rc1.tar` & `ha-services-0.2.0rc2.tar`

### file list

```diff
@@ -1,87 +1,98 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.281539 ha-services-0.2.0rc1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.281539 ha-services-0.2.0rc1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc1/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/
--rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-17 15:21:29.000000 ha-services-0.2.0rc1/ha_services/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     8343 2023-05-17 15:18:45.000000 ha-services-0.2.0rc1/ha_services/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/cli/dev.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli_tools/
--rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc1/ha_services/cli_tools/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc1/ha_services/cli_tools/path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc1/ha_services/cli_tools/richt_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1042 2023-05-11 07:10:26.000000 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/assertion.py
--rw-rw-r--   0 jens      (1000) users      (100)      649 2023-05-11 07:16:45.000000 ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/environment_fixtures.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/cli_tools/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/cli_tools/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_environ_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc1/ha_services/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     3437 2023-05-17 15:17:40.000000 ha-services-0.2.0rc1/ha_services/example.py
--rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/log_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     4083 2023-05-11 19:00:09.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/test_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/utilities/string_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/systemd/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     7253 2023-05-17 15:14:11.000000 ha-services-0.2.0rc1/ha_services/systemd/api.py
--rw-rw-r--   0 jens      (1000) users      (100)     3185 2023-05-17 15:08:18.000000 ha-services-0.2.0rc1/ha_services/systemd/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc1/ha_services/systemd/defaults.py
--rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.2.0rc1/ha_services/systemd/service_template.txt
--rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/systemd/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3266 2023-05-17 15:21:16.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1439 2023-05-17 15:21:02.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/test_data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/test_template.py
--rw-rw-r--   0 jens      (1000) users      (100)     1934 2023-05-17 15:16:21.000000 ha-services-0.2.0rc1/ha_services/systemd/tests/utilities.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/tests/test_project_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/toml_settings/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4305 2023-05-11 20:06:55.000000 ha-services-0.2.0rc1/ha_services/toml_settings/api.py
--rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc1/ha_services/toml_settings/data_class_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc1/ha_services/toml_settings/debug.py
--rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc1/ha_services/toml_settings/deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1647 2023-05-09 20:53:17.000000 ha-services-0.2.0rc1/ha_services/toml_settings/serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services/toml_settings/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1229 2023-05-09 20:53:54.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_demo_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     5607 2023-05-09 17:48:29.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     2758 2023-05-09 19:41:27.000000 ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/ha_services.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2405 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-17 15:25:02.000000 ha-services-0.2.0rc1/ha_services.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53002 2023-05-09 17:59:29.000000 ha-services-0.2.0rc1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-09 17:59:13.000000 ha-services-0.2.0rc1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-17 15:25:02.285539 ha-services-0.2.0rc1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc2/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/
+-rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-18 06:02:39.000000 ha-services-0.2.0rc2/ha_services/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8343 2023-05-17 15:18:45.000000 ha-services-0.2.0rc2/ha_services/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli_tools/
+-rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc2/ha_services/cli_tools/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.2.0rc2/ha_services/cli_tools/dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc2/ha_services/cli_tools/path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc2/ha_services/cli_tools/rich_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1041 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/assertion.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/environment_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)      820 2023-05-18 04:17:28.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/mock_rich.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli_tools/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_environ_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc2/ha_services/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3437 2023-05-17 15:17:40.000000 ha-services-0.2.0rc2/ha_services/example.py
+-rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/log_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4082 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/test_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/utilities/string_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/systemd/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7252 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/systemd/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3184 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/systemd/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc2/ha_services/systemd/defaults.py
+-rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.2.0rc2/ha_services/systemd/service_template.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/systemd/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.2.0rc2/ha_services/systemd/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.2.0rc2/ha_services/systemd/test_utils/mock_systemd_info.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/systemd/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3387 2023-05-18 05:56:02.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1482 2023-05-18 05:56:47.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_mock_systemd_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
+-rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/tests/test_project_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/toml_settings/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.2.0rc2/ha_services/toml_settings/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc2/ha_services/toml_settings/data_class_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc2/ha_services/toml_settings/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc2/ha_services/toml_settings/deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.2.0rc2/ha_services/toml_settings/serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/toml_settings/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.2.0rc2/ha_services/toml_settings/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      973 2023-05-18 05:40:38.000000 ha-services-0.2.0rc2/ha_services/toml_settings/test_utils/data_class_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/toml_settings/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_demo_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5606 2023-05-18 06:01:57.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_serialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1370 2023-05-18 05:44:11.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_test_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2868 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc2/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53004 2023-05-18 06:04:30.000000 ha-services-0.2.0rc2/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-18 06:04:13.000000 ha-services-0.2.0rc2/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/setup.cfg
```

### Comparing `ha-services-0.2.0rc1/.github/workflows/tests.yml` & `ha-services-0.2.0rc2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/PKG-INFO` & `ha-services-0.2.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.2.0rc1/README.md` & `ha-services-0.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/cli.py` & `ha-services-0.2.0rc2/cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/dev-cli.py` & `ha-services-0.2.0rc2/dev-cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/cli/cli_app.py` & `ha-services-0.2.0rc2/ha_services/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/cli/dev.py` & `ha-services-0.2.0rc2/ha_services/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/cli_tools/path_utils.py` & `ha-services-0.2.0rc2/ha_services/cli_tools/path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/cli_tools/richt_utils.py` & `ha-services-0.2.0rc2/ha_services/cli_tools/rich_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/cli_tools/test_utils/assertion.py` & `ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/assertion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from click._compat import strip_ansi as strip_ansi_codes
 from rich.console import Console
 
-from ha_services.cli_tools.richt_utils import PanelPrinter
+from ha_services.cli_tools.rich_utils import PanelPrinter
 
 
 def assert_in(content: str, parts: tuple[str, ...], strip_ansi=True) -> None:
     """
     Check if all parts exist in content
     """
     if strip_ansi:
```

### Comparing `ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_environ_fixtures.py` & `ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_environ_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/cli_tools/tests/test_path_utils.py` & `ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/example.py` & `ha-services-0.2.0rc2/ha_services/example.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/converter.py` & `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/data_classes.py` & `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/mqtt.py` & `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import paho.mqtt.client as mqtt
 from bx_py_utils.anonymize import anonymize
 from rich import print
 from rich.pretty import pprint
 
 from ha_services import __version__
-from ha_services.cli_tools.richt_utils import human_error
+from ha_services.cli_tools.rich_utils import human_error
 from ha_services.mqtt4homeassistant.data_classes import HaMqttPayload, MqttSettings
 
 
 logger = logging.getLogger(__name__)
 
 
 def get_client_id():
```

### Comparing `ha-services-0.2.0rc1/ha_services/mqtt4homeassistant/tests/test_converter.py` & `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/systemd/api.py` & `ha-services-0.2.0rc2/ha_services/systemd/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from subprocess import CalledProcessError
 
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from rich import print  # noqa
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 
-from ha_services.cli_tools.richt_utils import PanelPrinter, human_error, print_code, print_unified_diff
+from ha_services.cli_tools.rich_utils import PanelPrinter, human_error, print_code, print_unified_diff
 from ha_services.systemd.data_classes import BaseSystemdServiceInfo
 
 
 logger = logging.getLogger(__name__)
 
 
 class SystemdServiceError(RuntimeError):
```

### Comparing `ha-services-0.2.0rc1/ha_services/systemd/data_classes.py` & `ha-services-0.2.0rc2/ha_services/systemd/data_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 from pathlib import Path
 from string import Template
 
 from bx_py_utils.path import assert_is_dir, assert_is_file
 
-from ha_services.cli_tools.richt_utils import human_error
+from ha_services.cli_tools.rich_utils import human_error
 from ha_services.mqtt4homeassistant.utilities.string_utils import slugify
 from ha_services.systemd.defaults import (
     get_demo_exec_start,
     get_template_path,
     get_user_group,
     get_user_name,
     get_work_directory,
```

### Comparing `ha-services-0.2.0rc1/ha_services/systemd/template.py` & `ha-services-0.2.0rc2/ha_services/systemd/template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/systemd/tests/test_api.py` & `ha-services-0.2.0rc2/ha_services/systemd/tests/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,43 +6,45 @@
 from manageprojects.test_utils.subprocess import SubprocessCallMock
 from manageprojects.utilities import subprocess_utils
 
 
 from ha_services.cli_tools.test_utils.assertion import assert_in
 from ha_services.example import SystemdServiceInfo
 from ha_services.systemd.api import ServiceControl
-from ha_services.systemd.tests.utilities import MockedSystemdServiceInfo
+from ha_services.systemd.test_utils.mock_systemd_info import MockSystemdServiceInfo
 
 
 class MockedShutilWhich:
     def which(self, command, path=None):
         return f'/usr/bin/{command}'
 
 
 class SystemdApiTestCase(TestCase):
     def test_print_systemd_file(self):
-        with MockedSystemdServiceInfo(
+        with MockSystemdServiceInfo(
             prefix='test_print_systemd_file_', SystemdServiceInfoClass=SystemdServiceInfo
-        ) as info, RedirectOut() as buffer:
-            ServiceControl(info=info).debug_systemd_config()
+        ) as cm, RedirectOut() as buffer:
+            systemd_info = cm.systemd_info
+            ServiceControl(info=systemd_info).debug_systemd_config()
 
         self.assertEqual(buffer.stderr, '')
         assert_in(
             content=buffer.stdout,
             parts=(
                 '[Unit]',
                 'Description=HaServices Demo',
                 'ExecStart=/mocked/.venv/bin/python3 -m ha_services_app publish-loop',
                 'SyslogIdentifier=haservices_demo',
             ),
         )
 
     def test_service_control(self):
-        with MockedSystemdServiceInfo(prefix='test_', SystemdServiceInfoClass=SystemdServiceInfo) as info:
-            service_control = ServiceControl(info=info)
+        with MockSystemdServiceInfo(prefix='test_', SystemdServiceInfoClass=SystemdServiceInfo) as cm:
+            systemd_info = cm.systemd_info
+            service_control = ServiceControl(info=systemd_info)
 
             for func_name in ('enable', 'restart', 'stop', 'status', 'remove_systemd_service'):
                 with self.subTest(func_name):
                     service_control_func = getattr(service_control, func_name)
                     with RedirectOut() as buffer, self.assertRaises(SystemExit):
                         service_control_func()
                     assert_in(
@@ -57,22 +59,22 @@
                 subprocess_utils, 'shutil', MockedShutilWhich()
             ), RedirectOut() as buffer:
                 service_control.setup_and_restart_systemd_service()
 
             assert_in(
                 content=buffer.stdout,
                 parts=(
-                    f'Write "{info.service_file_path}"...',
+                    f'Write "{systemd_info.service_file_path}"...',
                     'systemctl daemon-reload',
                     'systemctl enable haservices_demo.service',
                     'systemctl restart haservices_demo.service',
                     'systemctl status haservices_demo.service',
                 ),
             )
-            assert_is_file(info.service_file_path)
+            assert_is_file(systemd_info.service_file_path)
 
             self.assertEqual(
                 mock.get_popenargs(),
                 [
                     ['/usr/bin/systemctl', 'daemon-reload'],
                     ['/usr/bin/systemctl', 'enable', 'haservices_demo.service'],
                     ['/usr/bin/systemctl', 'restart', 'haservices_demo.service'],
```

### Comparing `ha-services-0.2.0rc1/ha_services/systemd/tests/test_data_classes.py` & `ha-services-0.2.0rc2/ha_services/systemd/tests/test_data_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import tempfile
 from pathlib import Path
 from unittest import TestCase
 
 from ha_services.example import SystemdServiceInfo
-from ha_services.systemd.tests.utilities import MockedSystemdServiceInfo
+from ha_services.systemd.test_utils.mock_systemd_info import MockSystemdServiceInfo
 
 
 class SystemdDataClassesTestCase(TestCase):
     def test_systemd_service_info(self):
         info = SystemdServiceInfo()
 
         # Check some samples:
         self.assertEqual(info.template_context.verbose_service_name, 'HaServices Demo')
         self.assertEqual(info.service_slug, 'haservices_demo')
         self.assertEqual(info.template_context.syslog_identifier, 'haservices_demo')
         self.assertEqual(info.service_file_path, Path('/etc/systemd/system/haservices_demo.service'))
 
-        with MockedSystemdServiceInfo(
+        with MockSystemdServiceInfo(
             prefix='test_systemd_service_info_', SystemdServiceInfoClass=SystemdServiceInfo
-        ) as info:
+        ) as cm:
+            info = cm.systemd_info
+
             self.assertIsInstance(info, SystemdServiceInfo)
             self.assertEqual(info.template_context.user, 'MockedUserName')
             self.assertEqual(info.template_context.group, 'MockedUserName')
             self.assertEqual(
                 info.template_context.exec_start, '/mocked/.venv/bin/python3 -m ha_services_app publish-loop'
             )
```

### Comparing `ha-services-0.2.0rc1/ha_services/systemd/tests/test_template.py` & `ha-services-0.2.0rc2/ha_services/systemd/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/tests/test_project_setup.py` & `ha-services-0.2.0rc2/ha_services/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/api.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import tomlkit
 from rich import print  # noqa
 from rich.console import Console
 from tomlkit import TOMLDocument
 
 from ha_services.cli_tools.path_utils import backup, expand_user
-from ha_services.cli_tools.richt_utils import human_error
+from ha_services.cli_tools.rich_utils import human_error
 from ha_services.toml_settings.debug import print_dataclasses
 from ha_services.toml_settings.deserialize import toml2dataclass
 from ha_services.toml_settings.exceptions import UserSettingsNotFound
 from ha_services.toml_settings.sensible_editor import open_editor_for
-from ha_services.toml_settings.serialize import dataclass2toml
+from ha_services.toml_settings.serialize import dataclass2toml_str
 
 
 logger = logging.getLogger(__name__)
 
 
 class TomlSettings:
     settings_directories = (  # Path candidates where setting files will be stored
@@ -59,16 +59,15 @@
         if not settings_path.exists():
             settings_path.mkdir(parents=False, exist_ok=False)
         return settings_path / f'{file_name}.toml'
 
     def open_in_editor(self) -> None:
         if not self.file_path.is_file():
             logger.info('Settings file "%s" not exist -> create default', self.file_path)
-            document: TOMLDocument = dataclass2toml(instance=self.settings_dataclass)
-            doc_str = tomlkit.dumps(document, sort_keys=False)
+            doc_str = dataclass2toml_str(instance=self.settings_dataclass)
             self.file_path.write_text(doc_str, encoding='UTF-8')
 
         open_editor_for(self.file_path)
 
     def get_user_settings(self, *, debug: bool = False) -> dataclasses:
         if debug:
             print(f'Use user settings file: {self.file_path}', end='...')
```

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/debug.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/debug.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/deserialize.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/sensible_editor.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/serialize.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/serialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 
     item.add(field_name, value)
 
 
 def add_dataclass(document: TOMLDocument, name, instance):
     assert dataclasses.is_dataclass(instance), f'No dataclass: {instance!r}'
 
-    document.add(tomlkit.nl())  # Add new line
-
     table = tomlkit.table()
     add_docstring(table, instance)
 
     for field_name, field_value in iter_dataclass(instance):
         if dataclasses.is_dataclass(field_value):
             add_dataclass(table, field_name, field_value)
         else:
@@ -51,7 +49,16 @@
     for field_name, field_value in iter_dataclass(instance):
         if dataclasses.is_dataclass(field_value):
             add_dataclass(document, field_name, field_value)
         else:
             add_value(field_name=field_name, item=document, value=field_value)
 
     return document
+
+
+def dataclass2toml_str(instance) -> str:
+    """
+    Serialize a dataclass to a toml string.
+    """
+    document: TOMLDocument = dataclass2toml(instance=instance)
+    doc_str = tomlkit.dumps(document, sort_keys=False)
+    return doc_str.strip()
```

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/tests/fixtures.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/tests/fixtures.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 
 @dataclasses.dataclass
 class PathExample:
     path: Path = Path('/foo/bar')
 
 
+@dataclasses.dataclass
+class PathExample2:
+    path: Path = Path('/foo/baz')
+    sub_path: PathExample = dataclasses.field(default_factory=PathExample)
+
+
 ###########################################################################################
 
 
 @dataclasses.dataclass
 class SubClass1:
     """
     This is SubClass ONE on second level of FirstLevel
```

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_demo_settings.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_demo_settings.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_deserialize.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_deserialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,14 @@
                 '''
                 foo = "bar"
                 [sub_class_one]
                 number = 123
 
                 [sub_class_two]
                 something = 123.456
-
                 [sub_class_three]
                 # SubClass3(one_value: bool = True)
                 one_value = true
                 '''
             ),
         )
```

### Comparing `ha-services-0.2.0rc1/ha_services/toml_settings/tests/test_serialize.py` & `ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 import inspect
 from unittest import TestCase
 
 import tomlkit
 from tomlkit import TOMLDocument
 
-from ha_services.toml_settings.serialize import dataclass2toml
+from ha_services.toml_settings.serialize import dataclass2toml, dataclass2toml_str
 from ha_services.toml_settings.tests.fixtures import ComplexExample, PathExample, SimpleExample
 
 
 class SerializeTestCase(TestCase):
     def test_dataclass2toml_simple(self):
         document = dataclass2toml(instance=SimpleExample())
         self.assertIsInstance(document, TOMLDocument)
@@ -21,14 +21,29 @@
             inspect.cleandoc(
                 '''
                 # A simple example
                 one = "foo"
                 two = "bar"
                 three = ""
                 number = 123
+                '''
+            ),
+        )
+
+    def test_dataclass2toml_str(self):
+        toml_str = dataclass2toml_str(instance=SimpleExample())
+        self.assertEqual(
+            toml_str,
+            inspect.cleandoc(
+                '''
+                # A simple example
+                one = "foo"
+                two = "bar"
+                three = ""
+                number = 123
                 '''
             ),
         )
 
     def test_dataclass2toml_path(self):
         document = dataclass2toml(instance=PathExample())
         self.assertIsInstance(document, TOMLDocument)
```

### Comparing `ha-services-0.2.0rc1/ha_services.egg-info/PKG-INFO` & `ha-services-0.2.0rc2/ha_services.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.2.0rc1/ha_services.egg-info/SOURCES.txt` & `ha-services-0.2.0rc2/ha_services.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,23 @@
 ha_services.egg-info/entry_points.txt
 ha_services.egg-info/requires.txt
 ha_services.egg-info/top_level.txt
 ha_services/cli/__init__.py
 ha_services/cli/cli_app.py
 ha_services/cli/dev.py
 ha_services/cli_tools/__init__.py
+ha_services/cli_tools/dict_utils.py
 ha_services/cli_tools/path_utils.py
-ha_services/cli_tools/richt_utils.py
+ha_services/cli_tools/rich_utils.py
 ha_services/cli_tools/test_utils/__init__.py
 ha_services/cli_tools/test_utils/assertion.py
 ha_services/cli_tools/test_utils/environment_fixtures.py
+ha_services/cli_tools/test_utils/mock_rich.py
 ha_services/cli_tools/tests/__init__.py
+ha_services/cli_tools/tests/test_dict_utils.py
 ha_services/cli_tools/tests/test_environ_fixtures.py
 ha_services/cli_tools/tests/test_path_utils.py
 ha_services/mqtt4homeassistant/__init__.py
 ha_services/mqtt4homeassistant/converter.py
 ha_services/mqtt4homeassistant/data_classes.py
 ha_services/mqtt4homeassistant/mqtt.py
 ha_services/mqtt4homeassistant/tests/__init__.py
@@ -41,28 +44,34 @@
 ha_services/mqtt4homeassistant/utilities/string_utils.py
 ha_services/systemd/__init__.py
 ha_services/systemd/api.py
 ha_services/systemd/data_classes.py
 ha_services/systemd/defaults.py
 ha_services/systemd/service_template.txt
 ha_services/systemd/template.py
+ha_services/systemd/test_utils/__init__.py
+ha_services/systemd/test_utils/mock_systemd_info.py
 ha_services/systemd/tests/__init__.py
 ha_services/systemd/tests/test_api.py
 ha_services/systemd/tests/test_data_classes.py
+ha_services/systemd/tests/test_mock_systemd_info.py
+ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
 ha_services/systemd/tests/test_template.py
-ha_services/systemd/tests/utilities.py
 ha_services/tests/__init__.py
 ha_services/tests/test_doctests.py
 ha_services/tests/test_project_setup.py
 ha_services/toml_settings/__init__.py
 ha_services/toml_settings/api.py
 ha_services/toml_settings/data_class_utils.py
 ha_services/toml_settings/debug.py
 ha_services/toml_settings/deserialize.py
 ha_services/toml_settings/exceptions.py
 ha_services/toml_settings/sensible_editor.py
 ha_services/toml_settings/serialize.py
+ha_services/toml_settings/test_utils/__init__.py
+ha_services/toml_settings/test_utils/data_class_utils.py
 ha_services/toml_settings/tests/__init__.py
 ha_services/toml_settings/tests/fixtures.py
 ha_services/toml_settings/tests/test_demo_settings.py
 ha_services/toml_settings/tests/test_deserialize.py
-ha_services/toml_settings/tests/test_serialize.py
+ha_services/toml_settings/tests/test_serialize.py
+ha_services/toml_settings/tests/test_test_utils.py
```

### Comparing `ha-services-0.2.0rc1/pyproject.toml` & `ha-services-0.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc1/requirements.dev.txt` & `ha-services-0.2.0rc2/requirements.dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     --hash=sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414 \
     --hash=sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4
     # via readme-renderer
 build==0.10.0 \
     --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
     --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
     # via pip-tools
-bx-py-utils==80 \
-    --hash=sha256:34c4f5e4e1199014a83139aa4285a85f84274a982f9a9a8eae056fd9848a42f7 \
-    --hash=sha256:59f3d641c516fdf75d47ea86cd84fe6405d07fc7761074dcbbb967b6962dcc09
+bx-py-utils==81 \
+    --hash=sha256:5c2e189cccbeb852b058078bc7b0a8976f5f691ee7de657a87eef43fc89fa59a \
+    --hash=sha256:fd282f9e4ed8ed2842154ffe3fdd2ca56c428023021afc5b8ff765a53c02cddb
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
 cachetools==5.3.0 \
     --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
     --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
     # via tox
@@ -319,17 +319,17 @@
     --hash=sha256:cf4173be4ad2982e5b2ebab7e08bd0d27173f2459ec1b1cf66aec9290da80cce \
     --hash=sha256:d72126418194871aeaf1e8aa620ad06edc5472848bef71c4d393c22b65571878
     # via ha-services (pyproject.toml)
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
-docutils==0.19 \
-    --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
-    --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
+docutils==0.20.1 \
+    --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
+    --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
     # via readme-renderer
 dparse==0.6.2 \
     --hash=sha256:8097076f1dd26c377f30d4745e6ec18fef42f3bf493933b842ac5bafad8c345f \
     --hash=sha256:d45255bda21f998bc7ddf2afd5e62505ba6134756ba2d42a84c56b0826614dfe
     # via safety
 editorconfig==0.12.3 \
     --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
@@ -383,17 +383,17 @@
     --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
     --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
 keyring==23.13.1 \
     --hash=sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd \
     --hash=sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678
     # via twine
-manageprojects==0.9.10 \
-    --hash=sha256:5f6aac8e660cc8bc72548afbc300be8d3096f4afd715e1549a4bebedba105c75 \
-    --hash=sha256:be59603525d1f27519bd65717d5dcfe4d81eb75c34df71bb86a3fc4fbe15f0b5
+manageprojects==0.10.0 \
+    --hash=sha256:939d9cf9c629be755c2ab6f8ccd4019dfa1c7e39564c25f6087ec2f63867133a \
+    --hash=sha256:db457b77e52a73e3ec5fd4889e056df01926ec0c9b1476ab28c79db254d0465f
     # via ha-services (pyproject.toml)
 markdown-it-py==2.2.0 \
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via rich
 markupsafe==2.1.2 \
     --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
@@ -455,72 +455,72 @@
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
 more-itertools==9.1.0 \
     --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
     --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
     # via jaraco-classes
-msgspec==0.14.2 \
-    --hash=sha256:03ddc8c518afbea4fb89afb587d77f11d00909f003966d437f31fb8fffdfac28 \
-    --hash=sha256:1c8f7e631fad9d5a33fcfb0f2a27eb86dc0390e91d6b51c95a604b7ccbc264f1 \
-    --hash=sha256:1fc99f0929fa91cc53fa35f59be366d67f116c2b7f0f3b29dc60e3179f6fb205 \
-    --hash=sha256:2039451b22813af2fd5cbe99eaecfc318d64fcee5af0ce5b3d5cce12427d24cd \
-    --hash=sha256:26bcb3a69b348be2757ab19e86038e586920522a99d49d358c12890fbcfb6aa8 \
-    --hash=sha256:3288b65ee7c78d08f32003a8b5ca72fff12c6a7400bd35f9d65630c9d58efce2 \
-    --hash=sha256:4f13e47803aedbb32c9375317fedbd20af3397dc024d311eebdc635c07f6f908 \
-    --hash=sha256:57a79cfa306fda2c66f4fc7eb72836c0f78fd9a6d748d028960b387797f0381b \
-    --hash=sha256:580464c7ca5c47a1422973c853301bbfd3d1a4184bdb6bddb73b5df094d8fc55 \
-    --hash=sha256:587371a65798a0f0182d0a7a4b7c4b87a5f46e25e8821c6474b3f717dcfcad14 \
-    --hash=sha256:59491de3566c7789bdb0a152f305e150a6ba3e825af471680b05a029a664a89a \
-    --hash=sha256:78361dadef4b993b8c4a887d3d267b89b0ea0846259eadf2fe993659e4dbf9c8 \
-    --hash=sha256:7e50885274e2041e49ec5d7cce8e59768f599c27dfb4c046edaf9ab25b1fddc2 \
-    --hash=sha256:87c4cd1bb197be11f89ad779038c8989d6ffcb8b360705107f034e4d2783c0a6 \
-    --hash=sha256:8927efaf506e5a8f9ffe76602e08d30a80c19b38d50a7e783887c317573ecd80 \
-    --hash=sha256:8b8a766b9f3e7f87946965a8ffc6e72f7a3ec8d031b3168df16762bfd3d03205 \
-    --hash=sha256:8ed61cad6b20f0218a8d239294c4b30b4e82854871ba0434cf0d54497043bffe \
-    --hash=sha256:907ed4305a97b50248e6b86e79ddc8edcf9b718eab0c93a6b46d673c5edbe3a4 \
-    --hash=sha256:94fc3d9a8835f18c18b48fdf49f7d445184061bfbc457a6623a4eb1f74ebe806 \
-    --hash=sha256:a0a3908309581e4e632457fac1938fec7fd84121396ddab6ddca37784e6db068 \
-    --hash=sha256:a12e704786256431d559c2027d6135a64f2339f009118d97906709cd8409e7ac \
-    --hash=sha256:b965c14851f146537f1b732cd2ed16c38e0c59662f23b72d396aee21e81aed4f \
-    --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
-    --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
-    --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
-    --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
-    --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
-    --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
-    --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
-    # via ha-services (pyproject.toml)
-mypy==1.2.0 \
-    --hash=sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521 \
-    --hash=sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140 \
-    --hash=sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48 \
-    --hash=sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128 \
-    --hash=sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336 \
-    --hash=sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a \
-    --hash=sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41 \
-    --hash=sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f \
-    --hash=sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e \
-    --hash=sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8 \
-    --hash=sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238 \
-    --hash=sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119 \
-    --hash=sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb \
-    --hash=sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d \
-    --hash=sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed \
-    --hash=sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9 \
-    --hash=sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e \
-    --hash=sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a \
-    --hash=sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5 \
-    --hash=sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950 \
-    --hash=sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937 \
-    --hash=sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394 \
-    --hash=sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6 \
-    --hash=sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602 \
-    --hash=sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1 \
-    --hash=sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba
+msgspec==0.15.0 \
+    --hash=sha256:05fc603508e0c8021249d3e531fa4bb72d167bdfa76d869d48f96a5b8f9b50bf \
+    --hash=sha256:07ee1d1a15e3b319dcd7326470216928a7b58d47460b253577ccd0ab5dcf5c3c \
+    --hash=sha256:0c75fd847709e30265f050375c408fec1c07797694162834aa86ab3b3cf055da \
+    --hash=sha256:1b5b7c1b69416eab3ab2ad1c9593b749226b80555532292fae5fe9d154794089 \
+    --hash=sha256:20bf8018bff6bb85f5315ba6fd47b2f9373ab67e8bb59b0d7a7def22bbbf9f70 \
+    --hash=sha256:22713a1f618b4094c0268c6fbeef530397e5f3fa5292e4afd51caddad645843f \
+    --hash=sha256:2b57b6869ef1717c0343465198e19284d1e6aa5f292af2726284e4dfedfedeef \
+    --hash=sha256:346960762d648a6512b51f30be7c1267630e0bbc6fd65e8b23a3f54e5f562656 \
+    --hash=sha256:381c7a891adcc741e617956ba987912bc21864f9dd27b8cfb03bfb0aded5e1fd \
+    --hash=sha256:415519f68cd3f1a224f87ed415459ac3b86e4f6e82815a036e4238c62006f696 \
+    --hash=sha256:42c2f9fe0b58dc6f2b15720490c67554b5ba0007d3ee94340ca4448bda917287 \
+    --hash=sha256:490c88d76d573cce16653434ace3d9a8a8675ef6e350f114752fe60e69b6a232 \
+    --hash=sha256:4d3cde786110a92f764666b9f963b4389d5d1798bf1aca2422a59931d8d1f694 \
+    --hash=sha256:550b359c49562d52849103b87b4f7381fbc0adf958afa316599befb9a3e3379e \
+    --hash=sha256:8a46a9818570362d4022161684cdb97ecd102953043059ee4902862940f48f8d \
+    --hash=sha256:8b7e0354c37b742e1c02fe0cd3ced97db516c8da62ac5a408609e9f5858aaf24 \
+    --hash=sha256:8cee590163788fce21c5998d09198ef08ec06c1ca68ef50f2d5ed9e54d308538 \
+    --hash=sha256:9178a7550a5516295c682e6e5c143782503719b4c816496349a4a0f1b62397ef \
+    --hash=sha256:9d61de44b248feef82c8979a1e9912c923527cfb1d01c93b7bb5d6ca93ed09d6 \
+    --hash=sha256:beb3789519253b22338cca48053ba5ac8b442633e3af8f58e264d776a98ff6d0 \
+    --hash=sha256:bf3ab3f8d5752dbe68babc77d21b42575b916793515442e3890aef680e212154 \
+    --hash=sha256:c4c7e0abfac3a67f3e1d51e1d1313fd4205528e17663ff264b1945c3370b18bd \
+    --hash=sha256:cc253e4ad51d360590358ab2cee5a6139f04ad994e0fcbff52e7f61fca475c3e \
+    --hash=sha256:cd198ed4445914ebc25a24b6cc6020902bb6b888fc9b39500ef4500841b1b437 \
+    --hash=sha256:d760ff747165d84965791bfcd14588f61f111708036d80f1980387e3760035e7 \
+    --hash=sha256:ddef8fdc06676dd1bec9fe67b3128f84079469ee6424384cbb29a90c9033b559 \
+    --hash=sha256:f77cc91d3cb8a7bccfba28fe4aec537178384509bfce222f8eca287b7e5d0214 \
+    --hash=sha256:ff80bd40469915cc61686086a2503b901e17040f8a191099d8ccaa45dc72df8c \
+    --hash=sha256:fffa7ec85f27577f7f5471b390bf902d58ccd89b3612cf40bfb92f4ba75e6c95
+    # via ha-services (pyproject.toml)
+mypy==1.3.0 \
+    --hash=sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703 \
+    --hash=sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf \
+    --hash=sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4 \
+    --hash=sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85 \
+    --hash=sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd \
+    --hash=sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae \
+    --hash=sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd \
+    --hash=sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca \
+    --hash=sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305 \
+    --hash=sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409 \
+    --hash=sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c \
+    --hash=sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb \
+    --hash=sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee \
+    --hash=sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a \
+    --hash=sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228 \
+    --hash=sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897 \
+    --hash=sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d \
+    --hash=sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f \
+    --hash=sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152 \
+    --hash=sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf \
+    --hash=sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8 \
+    --hash=sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11 \
+    --hash=sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017 \
+    --hash=sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929 \
+    --hash=sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e \
+    --hash=sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a
     # via ha-services (pyproject.toml)
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
@@ -545,17 +545,17 @@
     --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
     --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
     # via ha-services (pyproject.toml)
 pkginfo==1.9.6 \
     --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
     --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
     # via twine
-platformdirs==3.5.0 \
-    --hash=sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4 \
-    --hash=sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335
+platformdirs==3.5.1 \
+    --hash=sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f \
+    --hash=sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5
     # via
     #   black
     #   tox
     #   virtualenv
 pluggy==1.0.0 \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
@@ -675,17 +675,17 @@
     #   twine
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
-ruamel-yaml==0.17.24 \
-    --hash=sha256:90e398ee24524ebe20fc48cd1861cedd25520457b9a36cfb548613e57fde30a0 \
-    --hash=sha256:f251bd9096207af604af69d6495c3c650a3338d0493d27b04bc55477d7a884ed
+ruamel-yaml==0.17.26 \
+    --hash=sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693 \
+    --hash=sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059
     # via safety
 ruamel-yaml-clib==0.2.7 \
     --hash=sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e \
     --hash=sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3 \
     --hash=sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5 \
     --hash=sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497 \
     --hash=sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f \
```

### Comparing `ha-services-0.2.0rc1/requirements.txt` & `ha-services-0.2.0rc2/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     --hash=sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1 \
     --hash=sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2
     # via jinja2-time
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-bx-py-utils==80 \
-    --hash=sha256:34c4f5e4e1199014a83139aa4285a85f84274a982f9a9a8eae056fd9848a42f7 \
-    --hash=sha256:59f3d641c516fdf75d47ea86cd84fe6405d07fc7761074dcbbb967b6962dcc09
+bx-py-utils==81 \
+    --hash=sha256:5c2e189cccbeb852b058078bc7b0a8976f5f691ee7de657a87eef43fc89fa59a \
+    --hash=sha256:fd282f9e4ed8ed2842154ffe3fdd2ca56c428023021afc5b8ff765a53c02cddb
     # via
     #   ha-services (pyproject.toml)
     #   manageprojects
 certifi==2023.5.7 \
     --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
     --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via requests
@@ -125,17 +125,17 @@
     # via
     #   cookiecutter
     #   jinja2-time
 jinja2-time==0.2.0 \
     --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
     --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
-manageprojects==0.9.10 \
-    --hash=sha256:5f6aac8e660cc8bc72548afbc300be8d3096f4afd715e1549a4bebedba105c75 \
-    --hash=sha256:be59603525d1f27519bd65717d5dcfe4d81eb75c34df71bb86a3fc4fbe15f0b5
+manageprojects==0.10.0 \
+    --hash=sha256:939d9cf9c629be755c2ab6f8ccd4019dfa1c7e39564c25f6087ec2f63867133a \
+    --hash=sha256:db457b77e52a73e3ec5fd4889e056df01926ec0c9b1476ab28c79db254d0465f
     # via ha-services (pyproject.toml)
 markdown-it-py==2.2.0 \
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via rich
 markupsafe==2.1.2 \
     --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
@@ -189,44 +189,44 @@
     --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
     --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
     # via jinja2
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
-msgspec==0.14.2 \
-    --hash=sha256:03ddc8c518afbea4fb89afb587d77f11d00909f003966d437f31fb8fffdfac28 \
-    --hash=sha256:1c8f7e631fad9d5a33fcfb0f2a27eb86dc0390e91d6b51c95a604b7ccbc264f1 \
-    --hash=sha256:1fc99f0929fa91cc53fa35f59be366d67f116c2b7f0f3b29dc60e3179f6fb205 \
-    --hash=sha256:2039451b22813af2fd5cbe99eaecfc318d64fcee5af0ce5b3d5cce12427d24cd \
-    --hash=sha256:26bcb3a69b348be2757ab19e86038e586920522a99d49d358c12890fbcfb6aa8 \
-    --hash=sha256:3288b65ee7c78d08f32003a8b5ca72fff12c6a7400bd35f9d65630c9d58efce2 \
-    --hash=sha256:4f13e47803aedbb32c9375317fedbd20af3397dc024d311eebdc635c07f6f908 \
-    --hash=sha256:57a79cfa306fda2c66f4fc7eb72836c0f78fd9a6d748d028960b387797f0381b \
-    --hash=sha256:580464c7ca5c47a1422973c853301bbfd3d1a4184bdb6bddb73b5df094d8fc55 \
-    --hash=sha256:587371a65798a0f0182d0a7a4b7c4b87a5f46e25e8821c6474b3f717dcfcad14 \
-    --hash=sha256:59491de3566c7789bdb0a152f305e150a6ba3e825af471680b05a029a664a89a \
-    --hash=sha256:78361dadef4b993b8c4a887d3d267b89b0ea0846259eadf2fe993659e4dbf9c8 \
-    --hash=sha256:7e50885274e2041e49ec5d7cce8e59768f599c27dfb4c046edaf9ab25b1fddc2 \
-    --hash=sha256:87c4cd1bb197be11f89ad779038c8989d6ffcb8b360705107f034e4d2783c0a6 \
-    --hash=sha256:8927efaf506e5a8f9ffe76602e08d30a80c19b38d50a7e783887c317573ecd80 \
-    --hash=sha256:8b8a766b9f3e7f87946965a8ffc6e72f7a3ec8d031b3168df16762bfd3d03205 \
-    --hash=sha256:8ed61cad6b20f0218a8d239294c4b30b4e82854871ba0434cf0d54497043bffe \
-    --hash=sha256:907ed4305a97b50248e6b86e79ddc8edcf9b718eab0c93a6b46d673c5edbe3a4 \
-    --hash=sha256:94fc3d9a8835f18c18b48fdf49f7d445184061bfbc457a6623a4eb1f74ebe806 \
-    --hash=sha256:a0a3908309581e4e632457fac1938fec7fd84121396ddab6ddca37784e6db068 \
-    --hash=sha256:a12e704786256431d559c2027d6135a64f2339f009118d97906709cd8409e7ac \
-    --hash=sha256:b965c14851f146537f1b732cd2ed16c38e0c59662f23b72d396aee21e81aed4f \
-    --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
-    --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
-    --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
-    --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
-    --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
-    --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
-    --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
+msgspec==0.15.0 \
+    --hash=sha256:05fc603508e0c8021249d3e531fa4bb72d167bdfa76d869d48f96a5b8f9b50bf \
+    --hash=sha256:07ee1d1a15e3b319dcd7326470216928a7b58d47460b253577ccd0ab5dcf5c3c \
+    --hash=sha256:0c75fd847709e30265f050375c408fec1c07797694162834aa86ab3b3cf055da \
+    --hash=sha256:1b5b7c1b69416eab3ab2ad1c9593b749226b80555532292fae5fe9d154794089 \
+    --hash=sha256:20bf8018bff6bb85f5315ba6fd47b2f9373ab67e8bb59b0d7a7def22bbbf9f70 \
+    --hash=sha256:22713a1f618b4094c0268c6fbeef530397e5f3fa5292e4afd51caddad645843f \
+    --hash=sha256:2b57b6869ef1717c0343465198e19284d1e6aa5f292af2726284e4dfedfedeef \
+    --hash=sha256:346960762d648a6512b51f30be7c1267630e0bbc6fd65e8b23a3f54e5f562656 \
+    --hash=sha256:381c7a891adcc741e617956ba987912bc21864f9dd27b8cfb03bfb0aded5e1fd \
+    --hash=sha256:415519f68cd3f1a224f87ed415459ac3b86e4f6e82815a036e4238c62006f696 \
+    --hash=sha256:42c2f9fe0b58dc6f2b15720490c67554b5ba0007d3ee94340ca4448bda917287 \
+    --hash=sha256:490c88d76d573cce16653434ace3d9a8a8675ef6e350f114752fe60e69b6a232 \
+    --hash=sha256:4d3cde786110a92f764666b9f963b4389d5d1798bf1aca2422a59931d8d1f694 \
+    --hash=sha256:550b359c49562d52849103b87b4f7381fbc0adf958afa316599befb9a3e3379e \
+    --hash=sha256:8a46a9818570362d4022161684cdb97ecd102953043059ee4902862940f48f8d \
+    --hash=sha256:8b7e0354c37b742e1c02fe0cd3ced97db516c8da62ac5a408609e9f5858aaf24 \
+    --hash=sha256:8cee590163788fce21c5998d09198ef08ec06c1ca68ef50f2d5ed9e54d308538 \
+    --hash=sha256:9178a7550a5516295c682e6e5c143782503719b4c816496349a4a0f1b62397ef \
+    --hash=sha256:9d61de44b248feef82c8979a1e9912c923527cfb1d01c93b7bb5d6ca93ed09d6 \
+    --hash=sha256:beb3789519253b22338cca48053ba5ac8b442633e3af8f58e264d776a98ff6d0 \
+    --hash=sha256:bf3ab3f8d5752dbe68babc77d21b42575b916793515442e3890aef680e212154 \
+    --hash=sha256:c4c7e0abfac3a67f3e1d51e1d1313fd4205528e17663ff264b1945c3370b18bd \
+    --hash=sha256:cc253e4ad51d360590358ab2cee5a6139f04ad994e0fcbff52e7f61fca475c3e \
+    --hash=sha256:cd198ed4445914ebc25a24b6cc6020902bb6b888fc9b39500ef4500841b1b437 \
+    --hash=sha256:d760ff747165d84965791bfcd14588f61f111708036d80f1980387e3760035e7 \
+    --hash=sha256:ddef8fdc06676dd1bec9fe67b3128f84079469ee6424384cbb29a90c9033b559 \
+    --hash=sha256:f77cc91d3cb8a7bccfba28fe4aec537178384509bfce222f8eca287b7e5d0214 \
+    --hash=sha256:ff80bd40469915cc61686086a2503b901e17040f8a191099d8ccaa45dc72df8c \
+    --hash=sha256:fffa7ec85f27577f7f5471b390bf902d58ccd89b3612cf40bfb92f4ba75e6c95
     # via ha-services (pyproject.toml)
 paho-mqtt==1.6.1 \
     --hash=sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f
     # via ha-services (pyproject.toml)
 pygments==2.15.1 \
     --hash=sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c \
     --hash=sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1
```

