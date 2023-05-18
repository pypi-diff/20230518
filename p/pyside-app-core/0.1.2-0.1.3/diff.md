# Comparing `tmp/pyside-app-core-0.1.2.tar.gz` & `tmp/pyside-app-core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside-app-core-0.1.2.tar", last modified: Thu May 18 15:01:36 2023, max compression
+gzip compressed data, was "pyside-app-core-0.1.3.tar", last modified: Thu May 18 15:20:28 2023, max compression
```

## Comparing `pyside-app-core-0.1.2.tar` & `pyside-app-core-0.1.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.253706 pyside-app-core-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.253706 pyside-app-core-0.1.2/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/generate_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.253706 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/spin-down/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/spin-up/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/util/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/util/s_color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.257706 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/error_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/param_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/param_spin.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/application_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.261706 pyside-app-core-0.1.2/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 15:01:22.000000 pyside-app-core-0.1.2/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:01:36.253706 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:01:36.000000 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 15:01:36.000000 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:01:36.000000 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:01:36.000000 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:01:36.000000 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:01:36.000000 pyside-app-core-0.1.2/src/pyside_app_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.203589 pyside-app-core-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.207589 pyside-app-core-0.1.3/src/pyside_app_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/serial_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/generate_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.203589 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-down/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-up/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/standard_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/style_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/pixel_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/s_color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.215590 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/error_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.215590 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/window_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_spin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/application_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/platform_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/serial_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/float_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/types/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.207589 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/top_level.txt
```

### Comparing `pyside-app-core-0.1.2/LICENSE` & `pyside-app-core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/PKG-INFO` & `pyside-app-core-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pyside-app-core-0.1.2/README.md` & `pyside-app-core-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/pyproject.toml` & `pyside-app-core-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyside-app-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "Framework for PySide Applications"
 readme = "README.md"
 authors = [{ name = "Leo Covarrubias", email = "leo@leocov.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Development Status :: 2 - Pre-Alpha",
@@ -60,15 +60,15 @@
     "src.pyside_app_core",
 ]
 forbidden_modules = [
     "examples.simple_app",
 ]
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/constants.py` & `pyside-app-core-0.1.3/src/pyside_app_core/constants.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/errors/excepthook.py` & `pyside-app-core-0.1.3/src/pyside_app_core/errors/excepthook.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/errors/serial_errors.py` & `pyside-app-core-0.1.3/src/pyside_app_core/errors/serial_errors.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/__main__.py` & `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/generate_resources.py` & `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/generate_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/standard_resources.py` & `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/standard_resources.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,42 @@
+from pathlib import Path
 from typing import List
 
 from pyside_app_core.generator_utils.style_types import QtResourceFile, QtResourceGroup
 
+__root = Path(__file__).parent
+
 STANDARD_RESOURCES: List[QtResourceGroup] = [
     QtResourceGroup(files=[QtResourceFile("style.qss")]),
     QtResourceGroup(
         prefix="std/",
         files=[
-            QtResourceFile("icons/console.svg", alias="icons/console"),
-            QtResourceFile("icons/down-arrow.svg", alias="icons/down-arrow"),
-            QtResourceFile("icons/grab-corner.svg", alias="icons/grab-corner"),
-            QtResourceFile("icons/reload.svg", alias="icons/reload"),
-            QtResourceFile("icons/save.svg", alias="icons/save"),
             QtResourceFile(
-                "icons/spin-down/normal.svg", alias="icons/spin-down/normal"
+                str(__root / "icons" / "console.svg"), alias="icons/console"
+            ),
+            QtResourceFile(
+                str(__root / "icons" / "down-arrow.svg"), alias="icons/down-arrow"
+            ),
+            QtResourceFile(
+                str(__root / "icons" / "grab-corner.svg"), alias="icons/grab-corner"
+            ),
+            QtResourceFile(str(__root / "icons" / "reload.svg"), alias="icons/reload"),
+            QtResourceFile(str(__root / "icons" / "save.svg"), alias="icons/save"),
+            QtResourceFile(
+                str(__root / "icons" / "spin-down/normal.svg"),
+                alias="icons/spin-down/normal",
+            ),
+            QtResourceFile(
+                str(__root / "icons" / "spin-down/disabled.svg"),
+                alias="icons/spin-down/disabled",
             ),
             QtResourceFile(
-                "icons/spin-down/disabled.svg", alias="icons/spin-down/disabled"
+                str(__root / "icons" / "spin-up/normal.svg"),
+                alias="icons/spin-up/normal",
             ),
-            QtResourceFile("icons/spin-up/normal.svg", alias="icons/spin-up/normal"),
             QtResourceFile(
-                "icons/spin-up/disabled.svg", alias="icons/spin-up/disabled"
+                str(__root / "icons" / "spin-up/disabled.svg"),
+                alias="icons/spin-up/disabled",
             ),
         ],
     ),
 ]
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/generator_utils/templates/style.qss.jinja2` & `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/style.qss.jinja2`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/log/__init__.py` & `pyside-app-core-0.1.3/src/pyside_app_core/log/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 __logger_cache: Dict[str, logging.Logger] = {}
 
 logging.setLoggerClass(PACLogger)
 
 __pac_name = "pyside_app_core"
 
+
 def _get_caller_name():
     try:
         stack = inspect.stack()
         frame = stack[2][0]
         module = inspect.getmodule(frame)
         if not module:
             return __pac_name
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/log/logger.py` & `pyside-app-core-0.1.3/src/pyside_app_core/log/logger.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/style.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/style.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/util/s_color.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/util/s_color.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/about_dialog.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/about_dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QLabel
 
-from pyside_app_core.qt.widgets.frameless.base_dialog import FramelessBaseDialog, StandardButton
+from pyside_app_core.qt.widgets.frameless.base_dialog import (
+    FramelessBaseDialog,
+    StandardButton,
+)
 from pyside_app_core.services import application_service
 
 
 class AboutDialog(FramelessBaseDialog):
-
     def __init__(self):
         super().__init__(icon=QIcon(":/std/icons/console"))
 
         self.setFixedSize(500, 300)
         self.setWindowTitle(f"About {application_service.get_app_name()}")
 
         self.setStandardButtons(StandardButton.Close)
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/error_dialog.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/error_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from PySide6.QtGui import QClipboard
 from PySide6.QtWidgets import QApplication, QLabel, QPlainTextEdit
 
-from pyside_app_core.qt.widgets.frameless.base_dialog import FramelessBaseDialog, StandardButton
+from pyside_app_core.qt.widgets.frameless.base_dialog import (
+    FramelessBaseDialog,
+    StandardButton,
+)
 
 
 class ErrorDialog(FramelessBaseDialog):
-
-    def __init__(
-        self,
-        message: str,
-        detailed: str | None = None
-    ):
+    def __init__(self, message: str, detailed: str | None = None):
         super().__init__()
 
         self.setWindowTitle("Encountered An Unexpected Error")
         self.setMinimumWidth(640)
 
         self._clipboard = QClipboard(parent=self)
 
-        self.setStandardButtons(StandardButton.Ignore | StandardButton.Reset | StandardButton.Abort)
+        self.setStandardButtons(
+            StandardButton.Ignore | StandardButton.Reset | StandardButton.Abort
+        )
         self.setDefaultButton(StandardButton.Ignore)
 
         self.setButtonText(StandardButton.Ignore, "Ignore")
         self.setButtonText(StandardButton.Reset, "Copy")
         self.setButtonText(StandardButton.Abort, "Quit")
 
         _copy_btn = self.button(StandardButton.Reset)
@@ -43,10 +43,12 @@
             self.addWidget(_t_lab)
             self._trace_box = QPlainTextEdit(detailed, parent=self)
             self._trace_box.setReadOnly(True)
             self.addWidget(self._trace_box)
 
     def _copy_to_clipboard(self):
         if self._trace_box:
-            self._clipboard.setText(f"{self._message_box.toPlainText()}\n\n{self._trace_box.toPlainText()}")
+            self._clipboard.setText(
+                f"{self._message_box.toPlainText()}\n\n{self._trace_box.toPlainText()}"
+            )
         else:
             self._clipboard.setText(self._message_box.toPlainText())
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/application.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/application.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/base_dialog.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/base_window.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_window.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/border.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/border.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/main_window.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/main_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from pyside_app_core.qt.widgets.menu_ctx import MenuBarContext
 from pyside_app_core.qt.widgets.tool_bar_ctx import ToolBarContext
 from pyside_app_core.qt.widgets.window_settings_mixin import WindowSettingsMixin
 from pyside_app_core.services import platform_service
 
 
 class FramelessMainWindow(WindowSettingsMixin, FramelessBaseMixin, QMainWindow):
-
     def __init__(self):
         super(FramelessMainWindow, self).__init__(parent=None)
 
         self._about_dialog = AboutDialog()
 
         self._central = QWidget(parent=self)
         self.setCentralWidget(self._central)
 
         # must in order to show grab handle
         self.statusBar().show()
 
         self._menu_bar = MenuBarContext(
             self,
-            border_width=0 if platform_service.is_macos else self._theme.win_divider_width,
+            border_width=0
+            if platform_service.is_macos
+            else self._theme.win_divider_width,
             border_color=self._theme.win_divider_color,
         )
 
         self._menu_bar.setNativeMenuBar(platform_service.is_macos)
         self.setMenuWidget(self._menu_bar)
 
         with self._menu_bar.add_menu(self.tr("File")) as file_menu:
@@ -42,17 +43,15 @@
                 about_action.setMenuRole(QAction.MenuRole.AboutRole)
 
                 def _show_about():
                     self._about_dialog.exec()
 
                 about_action.triggered.connect(_show_about)
 
-        self._tool_bar = ToolBarContext(
-            area="top", parent=self, movable=False
-        )
+        self._tool_bar = ToolBarContext(area="top", parent=self, movable=False)
         self._tool_bar.setToolButtonStyle(Qt.ToolButtonStyle.ToolButtonIconOnly)
 
         if platform_service.is_macos:
             spacer = QWidget(self)
             spacer.setFixedWidth(self._window_actions.container_width + 5)
             spacer.setFixedHeight(28)
             self._tool_bar.addWidget(spacer)
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/frameless/window_actions.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/window_actions.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/menu_ctx.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/menu_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/param_list_widget.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_list_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pyqtgraph import SpinBox
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtWidgets import QHBoxLayout, QLabel, QSizePolicy, QVBoxLayout, QWidget
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core import log
 
+
 class ParamConfig(NamedTuple):
     label: str
     init_val: int | float
     min_val: int | float
     max_val: int | float
     step: int | float
     unit: str | None
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/param_spin.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_spin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
 from pyside_app_core.services import application_service
 
 ToolBarArea = Literal["top", "bottom", "left", "right"]
 
 _TOOL_BAR_AREA_MAP = {
-    "top":    Qt.ToolBarArea.TopToolBarArea,
+    "top": Qt.ToolBarArea.TopToolBarArea,
     "bottom": Qt.ToolBarArea.BottomToolBarArea,
-    "right":  Qt.ToolBarArea.RightToolBarArea,
-    "left":   Qt.ToolBarArea.LeftToolBarArea,
+    "right": Qt.ToolBarArea.RightToolBarArea,
+    "left": Qt.ToolBarArea.LeftToolBarArea,
 }
 
 
 class ToolBarContext(ObjectNameMixin, QToolBar):
-    def __init__(
-        self, area: ToolBarArea, parent: QMainWindow, movable=False
-    ):
+    def __init__(self, area: ToolBarArea, parent: QMainWindow, movable=False):
         self._area = area
         self._theme = application_service.get_app_theme()
 
         _margins = [1, 1, 1, 1]
 
         if area == "left":
             self._border_side = "right"
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/services/application_service.py` & `pyside-app-core-0.1.3/src/pyside_app_core/services/application_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/serial_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     SerialConnectionError,
     SerialDisconnectedError,
     SerialReadError,
     SerialUnknownError,
     SerialWriteError,
 )
 from pyside_app_core.qt.widgets.object_name_mixin import ObjectNameMixin
-from pyside_app_core.services.serial_service.utils.abstract_decoder import DecoderInterface
+from pyside_app_core.services.serial_service.utils.abstract_decoder import (
+    DecoderInterface,
+)
 
 log.set_level(lvl=logging.DEBUG)
 
 
 class CanRegister(Protocol):
     def bind_serial_service(self, serial_service: "SerialService"):
         ...
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/float_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import struct
 from decimal import Decimal
 from typing import Any, Iterator, Mapping, Self, TypeVar
 
-from pyside_app_core.constants import DATA_STRUCT_ENDIAN, FLOAT_PRECISION, STRUCT_FLOAT_FMT
+from pyside_app_core.constants import (
+    DATA_STRUCT_ENDIAN,
+    FLOAT_PRECISION,
+    STRUCT_FLOAT_FMT,
+)
 
 K = TypeVar("K", bound=int)
 
 
 class FloatMap(Mapping[K, float]):
     def __init__(self, data: Mapping[K, float]):
         self._data = data
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core.egg-info/PKG-INFO` & `pyside-app-core-0.1.3/src/pyside_app_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pyside-app-core-0.1.2/src/pyside_app_core.egg-info/SOURCES.txt` & `pyside-app-core-0.1.3/src/pyside_app_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

