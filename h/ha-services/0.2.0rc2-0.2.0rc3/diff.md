# Comparing `tmp/ha-services-0.2.0rc2.tar.gz` & `tmp/ha-services-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha-services-0.2.0rc2.tar", last modified: Thu May 18 06:34:09 2023, max compression
+gzip compressed data, was "ha-services-0.2.0rc3.tar", last modified: Thu May 18 08:39:12 2023, max compression
```

## Comparing `ha-services-0.2.0rc2.tar` & `ha-services-0.2.0rc3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc2/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/
--rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-18 06:02:39.000000 ha-services-0.2.0rc2/ha_services/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     8343 2023-05-17 15:18:45.000000 ha-services-0.2.0rc2/ha_services/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/cli/dev.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli_tools/
--rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc2/ha_services/cli_tools/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.2.0rc2/ha_services/cli_tools/dict_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc2/ha_services/cli_tools/path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc2/ha_services/cli_tools/rich_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1041 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/assertion.py
--rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/environment_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)      820 2023-05-18 04:17:28.000000 ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/mock_rich.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/cli_tools/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_dict_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_environ_fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_path_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc2/ha_services/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     3437 2023-05-17 15:17:40.000000 ha-services-0.2.0rc2/ha_services/example.py
--rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/log_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     4082 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/test_converter.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/utilities/string_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/systemd/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     7252 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/systemd/api.py
--rw-rw-r--   0 jens      (1000) users      (100)     3184 2023-05-18 04:39:33.000000 ha-services-0.2.0rc2/ha_services/systemd/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc2/ha_services/systemd/defaults.py
--rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.2.0rc2/ha_services/systemd/service_template.txt
--rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/systemd/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.2.0rc2/ha_services/systemd/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.2.0rc2/ha_services/systemd/test_utils/mock_systemd_info.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/systemd/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3387 2023-05-18 05:56:02.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1482 2023-05-18 05:56:47.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_mock_systemd_info.py
--rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
--rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc2/ha_services/systemd/tests/test_template.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/tests/test_project_setup.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/toml_settings/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.2.0rc2/ha_services/toml_settings/api.py
--rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc2/ha_services/toml_settings/data_class_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc2/ha_services/toml_settings/debug.py
--rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc2/ha_services/toml_settings/deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/sensible_editor.py
--rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.2.0rc2/ha_services/toml_settings/serialize.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/toml_settings/test_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.2.0rc2/ha_services/toml_settings/test_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      973 2023-05-18 05:40:38.000000 ha-services-0.2.0rc2/ha_services/toml_settings/test_utils/data_class_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services/toml_settings/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_demo_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     5606 2023-05-18 06:01:57.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_deserialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_serialize.py
--rw-rw-r--   0 jens      (1000) users      (100)     1370 2023-05-18 05:44:11.000000 ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_test_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/ha_services.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2868 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-18 06:34:09.000000 ha-services-0.2.0rc2/ha_services.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc2/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53004 2023-05-18 06:04:30.000000 ha-services-0.2.0rc2/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-18 06:04:13.000000 ha-services-0.2.0rc2/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-18 06:34:09.892654 ha-services-0.2.0rc2/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)      823 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-11 18:48:55.000000 ha-services-0.2.0rc3/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3052 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/
+-rw-rw-r--   0 jens      (1000) users      (100)      168 2023-05-18 08:36:49.000000 ha-services-0.2.0rc3/ha_services/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      195 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8343 2023-05-17 15:18:45.000000 ha-services-0.2.0rc3/ha_services/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7880 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/cli/dev.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli_tools/
+-rw-rw-r--   0 jens      (1000) users      (100)      120 2023-05-11 06:15:16.000000 ha-services-0.2.0rc3/ha_services/cli_tools/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1364 2023-05-18 05:57:33.000000 ha-services-0.2.0rc3/ha_services/cli_tools/dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2529 2023-05-11 17:34:50.000000 ha-services-0.2.0rc3/ha_services/cli_tools/path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3729 2023-05-11 20:05:42.000000 ha-services-0.2.0rc3/ha_services/cli_tools/rich_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1041 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/assertion.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1261 2023-05-18 04:14:32.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/environment_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)      820 2023-05-18 04:17:28.000000 ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/mock_rich.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/cli_tools/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      432 2023-05-18 05:10:52.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_dict_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      693 2023-05-11 07:38:00.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_environ_fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1918 2023-05-11 07:37:29.000000 ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_path_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)      164 2023-05-09 16:59:30.000000 ha-services-0.2.0rc3/ha_services/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3437 2023-05-17 15:17:40.000000 ha-services-0.2.0rc3/ha_services/example.py
+-rw-rw-r--   0 jens      (1000) users      (100)      240 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/log_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1898 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1061 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4082 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2142 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/test_converter.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/utilities/string_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/systemd/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7252 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/systemd/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3184 2023-05-18 04:39:33.000000 ha-services-0.2.0rc3/ha_services/systemd/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)      505 2023-05-10 07:16:49.000000 ha-services-0.2.0rc3/ha_services/systemd/defaults.py
+-rw-rw-r--   0 jens      (1000) users      (100)      320 2023-05-17 15:08:38.000000 ha-services-0.2.0rc3/ha_services/systemd/service_template.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1794 2023-05-09 19:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/systemd/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 04:08:42.000000 ha-services-0.2.0rc3/ha_services/systemd/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2012 2023-05-18 05:54:08.000000 ha-services-0.2.0rc3/ha_services/systemd/test_utils/mock_systemd_info.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/systemd/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3387 2023-05-18 05:56:02.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1482 2023-05-18 05:56:47.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3000 2023-05-18 06:02:23.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)      595 2023-05-18 06:01:09.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml
+-rw-rw-r--   0 jens      (1000) users      (100)     2471 2023-05-09 19:43:34.000000 ha-services-0.2.0rc3/ha_services/systemd/tests/test_template.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      262 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      217 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2579 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/tests/test_project_setup.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/toml_settings/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4234 2023-05-18 05:57:51.000000 ha-services-0.2.0rc3/ha_services/toml_settings/api.py
+-rw-rw-r--   0 jens      (1000) users      (100)      220 2023-05-09 20:53:17.000000 ha-services-0.2.0rc3/ha_services/toml_settings/data_class_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1352 2023-05-11 19:53:35.000000 ha-services-0.2.0rc3/ha_services/toml_settings/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3059 2023-05-09 20:53:17.000000 ha-services-0.2.0rc3/ha_services/toml_settings/deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)       56 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      728 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/sensible_editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1847 2023-05-18 06:01:57.000000 ha-services-0.2.0rc3/ha_services/toml_settings/serialize.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-18 05:26:41.000000 ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3092 2023-05-18 08:32:52.000000 ha-services-0.2.0rc3/ha_services/toml_settings/test_utils/data_class_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/ha_services/toml_settings/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-05-09 16:39:25.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1383 2023-05-18 05:43:52.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1044 2023-05-17 15:20:34.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_demo_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5606 2023-05-18 06:01:57.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_deserialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3172 2023-05-18 05:24:56.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_serialize.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3205 2023-05-18 08:31:32.000000 ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_test_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-18 08:39:12.683547 ha-services-0.2.0rc3/ha_services.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)     1239 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     2868 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      105 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      283 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       12 2023-05-18 08:39:12.000000 ha-services-0.2.0rc3/ha_services.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4934 2023-05-09 17:58:58.000000 ha-services-0.2.0rc3/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53004 2023-05-18 06:04:30.000000 ha-services-0.2.0rc3/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22054 2023-05-18 06:04:13.000000 ha-services-0.2.0rc3/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-18 08:39:12.687547 ha-services-0.2.0rc3/setup.cfg
```

### Comparing `ha-services-0.2.0rc2/.github/workflows/tests.yml` & `ha-services-0.2.0rc3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/PKG-INFO` & `ha-services-0.2.0rc3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.2.0rc2/README.md` & `ha-services-0.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/cli.py` & `ha-services-0.2.0rc3/cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/dev-cli.py` & `ha-services-0.2.0rc3/dev-cli.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli/cli_app.py` & `ha-services-0.2.0rc3/ha_services/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli/dev.py` & `ha-services-0.2.0rc3/ha_services/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/dict_utils.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/dict_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/path_utils.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/rich_utils.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/rich_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/assertion.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/assertion.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/environment_fixtures.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/environment_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/test_utils/mock_rich.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/test_utils/mock_rich.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_environ_fixtures.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_environ_fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/cli_tools/tests/test_path_utils.py` & `ha-services-0.2.0rc3/ha_services/cli_tools/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/example.py` & `ha-services-0.2.0rc3/ha_services/example.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/converter.py` & `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/data_classes.py` & `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/mqtt.py` & `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/mqtt4homeassistant/tests/test_converter.py` & `ha-services-0.2.0rc3/ha_services/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/api.py` & `ha-services-0.2.0rc3/ha_services/systemd/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/data_classes.py` & `ha-services-0.2.0rc3/ha_services/systemd/data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/template.py` & `ha-services-0.2.0rc3/ha_services/systemd/template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/test_utils/mock_systemd_info.py` & `ha-services-0.2.0rc3/ha_services/systemd/test_utils/mock_systemd_info.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/tests/test_api.py` & `ha-services-0.2.0rc3/ha_services/systemd/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/tests/test_data_classes.py` & `ha-services-0.2.0rc3/ha_services/systemd/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/tests/test_mock_systemd_info.py` & `ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml` & `ha-services-0.2.0rc3/ha_services/systemd/tests/test_mock_systemd_info_mock_1.snapshot.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/systemd/tests/test_template.py` & `ha-services-0.2.0rc3/ha_services/systemd/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/tests/test_project_setup.py` & `ha-services-0.2.0rc3/ha_services/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/api.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/api.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/debug.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/debug.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/deserialize.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/sensible_editor.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/sensible_editor.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/serialize.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/tests/fixtures.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_demo_settings.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_demo_settings.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_deserialize.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services/toml_settings/tests/test_serialize.py` & `ha-services-0.2.0rc3/ha_services/toml_settings/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/ha_services.egg-info/PKG-INFO` & `ha-services-0.2.0rc3/ha_services.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-services
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Helpers to send periodic information via MQTT to Home Assistant
 Author-email: Jens Diemer <github@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/ha_services
 Project-URL: Source, https://github.com/jedie/ha_services
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `ha-services-0.2.0rc2/ha_services.egg-info/SOURCES.txt` & `ha-services-0.2.0rc3/ha_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/pyproject.toml` & `ha-services-0.2.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/requirements.dev.txt` & `ha-services-0.2.0rc3/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `ha-services-0.2.0rc2/requirements.txt` & `ha-services-0.2.0rc3/requirements.txt`

 * *Files identical despite different names*

