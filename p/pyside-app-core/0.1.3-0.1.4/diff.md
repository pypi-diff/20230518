# Comparing `tmp/pyside-app-core-0.1.3.tar.gz` & `tmp/pyside-app-core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyside-app-core-0.1.3.tar", last modified: Thu May 18 15:20:28 2023, max compression
+gzip compressed data, was "pyside-app-core-0.1.4.tar", last modified: Thu May 18 15:26:56 2023, max compression
```

## Comparing `pyside-app-core-0.1.3.tar` & `pyside-app-core-0.1.4.tar`

### file list

```diff
@@ -1,89 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.203589 pyside-app-core-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.207589 pyside-app-core-0.1.3/src/pyside_app_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/basic_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/encode_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/errors/serial_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/generate_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.203589 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-down/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-up/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/standard_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/style_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/log/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.211590 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/pixel_val.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/util/s_color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.215590 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/error_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.215590 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/window_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/menu_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/multi_combo_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/object_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_spin.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/settings_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/window_settings_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/application_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/debug_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/platform_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/serial_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/float_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.219590 pyside-app-core-0.1.3/src/pyside_app_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 15:20:11.000000 pyside-app-core-0.1.3/src/pyside_app_core/types/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:20:28.207589 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:20:28.000000 pyside-app-core-0.1.3/src/pyside_app_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.714057 pyside-app-core-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:26:56.714057 pyside-app-core-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:26:56.714057 pyside-app-core-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.686055 pyside-app-core-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.694056 pyside-app-core-0.1.4/src/pyside_app_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.698056 pyside-app-core-0.1.4/src/pyside_app_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/errors/basic_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/errors/encode_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/errors/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/errors/serial_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.698056 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/generate_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.698056 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/down-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/grab-corner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/reload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.698056 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/spin-down/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.702056 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/spin-up/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/standard_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/style_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.702056 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/templates/style.qss.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.702056 pyside-app-core-0.1.4/src/pyside_app_core/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.702056 pyside-app-core-0.1.4/src/pyside_app_core/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.702056 pyside-app-core-0.1.4/src/pyside_app_core/qt/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/util/pixel_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/util/s_color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.706056 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/error_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.710056 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/base_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/window_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/menu_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/multi_combo_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/object_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/param_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/param_spin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/settings_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/tool_bar_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/tool_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/tool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/window_settings_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.710056 pyside-app-core-0.1.4/src/pyside_app_core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/application_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/debug_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/platform_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.710056 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/serial_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.710056 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/abstract_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/float_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.710056 pyside-app-core-0.1.4/src/pyside_app_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 15:26:40.000000 pyside-app-core-0.1.4/src/pyside_app_core/types/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:26:56.694056 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-05-18 15:26:56.000000 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-18 15:26:56.000000 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:26:56.000000 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 15:26:56.000000 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 15:26:56.000000 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:26:56.000000 pyside-app-core-0.1.4/src/pyside_app_core.egg-info/top_level.txt
```

### Comparing `pyside-app-core-0.1.3/LICENSE` & `pyside-app-core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/PKG-INFO` & `pyside-app-core-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pyside-app-core-0.1.3/README.md` & `pyside-app-core-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/pyproject.toml` & `pyside-app-core-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyside-app-core"
-version = "0.1.3"
+version = "0.1.4"
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
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/constants.py` & `pyside-app-core-0.1.4/src/pyside_app_core/constants.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/errors/excepthook.py` & `pyside-app-core-0.1.4/src/pyside_app_core/errors/excepthook.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/errors/serial_errors.py` & `pyside-app-core-0.1.4/src/pyside_app_core/errors/serial_errors.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/__main__.py` & `pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/generate_resources.py` & `pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/generate_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/standard_resources.py` & `pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/standard_resources.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/generator_utils/templates/style.qss.jinja2` & `pyside-app-core-0.1.4/src/pyside_app_core/generator_utils/templates/style.qss.jinja2`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/log/__init__.py` & `pyside-app-core-0.1.4/src/pyside_app_core/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/log/logger.py` & `pyside-app-core-0.1.4/src/pyside_app_core/log/logger.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/style.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/style.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/util/s_color.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/util/s_color.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/about_dialog.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/about_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/dynamic_stacked_widget.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/error_dialog.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/error_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/application.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/application.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_dialog.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/base_dialog.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/base_window.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/base_window.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/border.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/border.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/main_window.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/main_window.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/frameless/window_actions.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/frameless/window_actions.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/menu_ctx.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/menu_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/multi_combo_box.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/multi_combo_box.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/object_name_mixin.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/object_name_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_list_widget.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/param_list_widget.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/param_spin.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/param_spin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/settings_mixin.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_bar_ctx.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/tool_bar_ctx.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_button.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/tool_button.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/tool_stack.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/tool_stack.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/qt/widgets/window_settings_mixin.py` & `pyside-app-core-0.1.4/src/pyside_app_core/qt/widgets/window_settings_mixin.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/services/application_service.py` & `pyside-app-core-0.1.4/src/pyside_app_core/services/application_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/serial_service.py` & `pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/serial_service.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/conversion_utils.py` & `pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core/services/serial_service/utils/float_map.py` & `pyside-app-core-0.1.4/src/pyside_app_core/services/serial_service/utils/float_map.py`

 * *Files identical despite different names*

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core.egg-info/PKG-INFO` & `pyside-app-core-0.1.4/src/pyside_app_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyside-app-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework for PySide Applications
 Author-email: Leo Covarrubias <leo@leocov.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pyside-app-core-0.1.3/src/pyside_app_core.egg-info/SOURCES.txt` & `pyside-app-core-0.1.4/src/pyside_app_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 src/pyside_app_core/errors/excepthook.py
 src/pyside_app_core/errors/serial_errors.py
 src/pyside_app_core/generator_utils/__init__.py
 src/pyside_app_core/generator_utils/__main__.py
 src/pyside_app_core/generator_utils/generate_resources.py
 src/pyside_app_core/generator_utils/standard_resources.py
 src/pyside_app_core/generator_utils/style_types.py
+src/pyside_app_core/generator_utils/icons/console.svg
+src/pyside_app_core/generator_utils/icons/down-arrow.svg
+src/pyside_app_core/generator_utils/icons/grab-corner.svg
+src/pyside_app_core/generator_utils/icons/reload.svg
+src/pyside_app_core/generator_utils/icons/save.svg
 src/pyside_app_core/generator_utils/icons/spin-down/disabled.svg
 src/pyside_app_core/generator_utils/icons/spin-down/normal.svg
 src/pyside_app_core/generator_utils/icons/spin-up/disabled.svg
 src/pyside_app_core/generator_utils/icons/spin-up/normal.svg
 src/pyside_app_core/generator_utils/templates/resources.qrc.jinja2
 src/pyside_app_core/generator_utils/templates/style.qss.jinja2
 src/pyside_app_core/log/__init__.py
```

