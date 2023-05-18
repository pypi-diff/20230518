# Comparing `tmp/pydm-1.8.0.tar.gz` & `tmp/pydm-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydm-1.8.0.tar", last modified: Thu Nov 14 01:05:07 2019, max compression
+gzip compressed data, was "dist/pydm-1.9.0.tar", last modified: Tue Mar 24 19:25:57 2020, max compression
```

## Comparing `pydm-1.8.0.tar` & `pydm-1.9.0.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.306913 pydm-1.8.0/
--rw-r--r--   0 vsts      (1001) docker     (115)     2449 2019-11-14 01:05:02.000000 pydm-1.8.0/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (115)      280 2019-11-14 01:05:02.000000 pydm-1.8.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (115)     7023 2019-11-14 01:05:07.306913 pydm-1.8.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (115)     5246 2019-11-14 01:05:02.000000 pydm-1.8.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (115)       55 2019-11-14 01:05:02.000000 pydm-1.8.0/dev-requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.274913 pydm-1.8.0/examples/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:02.000000 pydm-1.8.0/examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.306913 pydm-1.8.0/pydm/
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.278913 pydm-1.8.0/pydm/PyQt/
--rw-r--r--   0 vsts      (1001) docker     (115)       22 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/Qt.py
--rw-r--r--   0 vsts      (1001) docker     (115)       25 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/QtCore.py
--rw-r--r--   0 vsts      (1001) docker     (115)       30 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/QtDesigner.py
--rw-r--r--   0 vsts      (1001) docker     (115)       93 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/QtGui.py
--rw-r--r--   0 vsts      (1001) docker     (115)       25 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/QtSvg.py
--rw-r--r--   0 vsts      (1001) docker     (115)       29 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/QtWidgets.py
--rw-r--r--   0 vsts      (1001) docker     (115)      165 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)       23 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/PyQt/uic.py
--rw-r--r--   0 vsts      (1001) docker     (115)      209 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)      497 2019-11-14 01:05:07.306913 pydm-1.8.0/pydm/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.278913 pydm-1.8.0/pydm/about_pydm/
--rw-r--r--   0 vsts      (1001) docker     (115)       30 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/about_pydm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3980 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/about_pydm/about.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5919 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/about_pydm/about_ui.py
--rw-r--r--   0 vsts      (1001) docker     (115)      285 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/about_pydm/contributors.txt
--rw-r--r--   0 vsts      (1001) docker     (115)    20209 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/application.py
--rw-r--r--   0 vsts      (1001) docker     (115)      345 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/config.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.278913 pydm-1.8.0/pydm/connection_inspector/
--rw-r--r--   0 vsts      (1001) docker     (115)       53 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/connection_inspector/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3228 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/connection_inspector/connection_inspector.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2811 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/connection_inspector/connection_table_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.278913 pydm-1.8.0/pydm/data_plugins/
--rw-r--r--   0 vsts      (1001) docker     (115)     6736 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1172 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/archiver_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1046 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/epics_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.282913 pydm-1.8.0/pydm/data_plugins/epics_plugins/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/epics_plugins/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7196 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/epics_plugins/caproto_plugin_component.py
--rw-r--r--   0 vsts      (1001) docker     (115)    15649 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/epics_plugins/psp_plugin_component.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7107 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/epics_plugins/pyepics_plugin_component.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1001 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/fake_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (115)    12561 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/local_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7050 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/data_plugins/plugin.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6289 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/default_stylesheet.qss
--rw-r--r--   0 vsts      (1001) docker     (115)     1632 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/display_module.py
--rw-r--r--   0 vsts      (1001) docker     (115)    19603 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/main_window.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10148 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/pydm_ui.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2252 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/qtdesigner.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.282913 pydm-1.8.0/pydm/tests/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2980 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (115)      199 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/test_about_screen.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1359 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/test_data_plugins_import.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1359 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/test_display.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5286 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/test_plugins_import.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.282913 pydm-1.8.0/pydm/tests/utilities/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)      786 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_colors.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1576 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_iconfont.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2014 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_macro.py
--rw-r--r--   0 vsts      (1001) docker     (115)      292 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_remove_protocol.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4196 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_stylesheet.py
--rw-r--r--   0 vsts      (1001) docker     (115)      956 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_units.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2281 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/utilities/test_utilities.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.290913 pydm-1.8.0/pydm/tests/widgets/
--rw-r--r--   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)    19838 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_base.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3665 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_baseplot.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1725 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_byte.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3865 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_channel.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2832 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1979 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_colormaps.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5283 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_display_format.py
--rw-r--r--   0 vsts      (1001) docker     (115)    38864 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_drawing.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8043 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_enum_button.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10814 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_enum_combo_box.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7540 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_frame.py
--rw-r--r--   0 vsts      (1001) docker     (115)    23374 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_label.py
--rw-r--r--   0 vsts      (1001) docker     (115)    26658 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_lineedit.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1529 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_logdisplay.py
--rw-r--r--   0 vsts      (1001) docker     (115)    22138 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_pushbutton.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4515 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_related_display_button.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3379 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_rules.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7824 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_rules_editor.py
--rw-r--r--   0 vsts      (1001) docker     (115)     9698 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_shell_command.py
--rw-r--r--   0 vsts      (1001) docker     (115)    22885 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_slider.py
--rw-r--r--   0 vsts      (1001) docker     (115)    11582 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_spinbox.py
--rw-r--r--   0 vsts      (1001) docker     (115)      902 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_template_repeater.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8626 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tests/widgets/test_timeplot.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.290913 pydm-1.8.0/pydm/tools/
--rw-r--r--   0 vsts      (1001) docker     (115)     5717 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3376 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/tools/tools.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.290913 pydm-1.8.0/pydm/utilities/
--rw-r--r--   0 vsts      (1001) docker     (115)     5292 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4720 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/color2hex.pkl
--rw-r--r--   0 vsts      (1001) docker     (115)     1563 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/colors.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1552 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/connection.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3318 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/display_loading.py
--rw-r--r--   0 vsts      (1001) docker     (115)    20580 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/fontawesome-charmap.json
--rw-r--r--   0 vsts      (1001) docker     (115)   165548 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/fontawesome.ttf
--rw-r--r--   0 vsts      (1001) docker     (115)     4720 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/hex2color.pkl
--rw-r--r--   0 vsts      (1001) docker     (115)     4789 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/iconfont.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3871 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/macro.py
--rw-r--r--   0 vsts      (1001) docker     (115)      962 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/remove_protocol.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3068 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/stylesheet.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3639 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/utilities/units.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.306913 pydm-1.8.0/pydm/widgets/
--rw-r--r--   0 vsts      (1001) docker     (115)     1026 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (115)    33614 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/base.py
--rw-r--r--   0 vsts      (1001) docker     (115)    24337 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/baseplot.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8151 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/baseplot_curve_editor.py
--rw-r--r--   0 vsts      (1001) docker     (115)     4903 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/baseplot_table_model.py
--rw-r--r--   0 vsts      (1001) docker     (115)    14920 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/byte.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6971 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/channel.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1512 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/checkbox.py
--rwxr-xr-x   0 vsts      (1001) docker     (115)    51720 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/colormaps.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2613 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/display_format.py
--rw-r--r--   0 vsts      (1001) docker     (115)    29252 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/drawing.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10983 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/embedded_display.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7426 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/enum_button.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6696 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/enum_combo_box.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1821 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/frame.py
--rw-r--r--   0 vsts      (1001) docker     (115)    19539 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/image.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3747 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/label.py
--rw-r--r--   0 vsts      (1001) docker     (115)    10366 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/line_edit.py
--rw-r--r--   0 vsts      (1001) docker     (115)     7181 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/logdisplay.py
--rw-r--r--   0 vsts      (1001) docker     (115)    11929 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/pushbutton.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5583 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/qtplugin_base.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3834 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/qtplugin_extensions.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8544 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/qtplugins.py
--rw-r--r--   0 vsts      (1001) docker     (115)     9543 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/related_display_button.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8992 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/rules.py
--rw-r--r--   0 vsts      (1001) docker     (115)    18926 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/rules_editor.py
--rw-r--r--   0 vsts      (1001) docker     (115)    34946 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/scale.py
--rw-r--r--   0 vsts      (1001) docker     (115)    18137 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/scatterplot.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3182 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/scatterplot_curve_editor.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3970 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/shell_command.py
--rw-r--r--   0 vsts      (1001) docker     (115)    19982 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/slider.py
--rw-r--r--   0 vsts      (1001) docker     (115)     6301 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/spinbox.py
--rw-r--r--   0 vsts      (1001) docker     (115)     8934 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/symbol.py
--rw-r--r--   0 vsts      (1001) docker     (115)    11747 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/tab_bar.py
--rw-r--r--   0 vsts      (1001) docker     (115)     1437 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/tab_bar_qtplugin.py
--rw-r--r--   0 vsts      (1001) docker     (115)    13787 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/template_repeater.py
--rw-r--r--   0 vsts      (1001) docker     (115)    29524 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/timeplot.py
--rw-r--r--   0 vsts      (1001) docker     (115)     2149 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/timeplot_curve_editor.py
--rw-r--r--   0 vsts      (1001) docker     (115)    19432 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/waveformplot.py
--rw-r--r--   0 vsts      (1001) docker     (115)     3006 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/waveformplot_curve_editor.py
--rw-r--r--   0 vsts      (1001) docker     (115)     5433 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm/widgets/waveformtable.py
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.278913 pydm-1.8.0/pydm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (115)     7023 2019-11-14 01:05:07.000000 pydm-1.8.0/pydm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (115)     4303 2019-11-14 01:05:07.000000 pydm-1.8.0/pydm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (115)        1 2019-11-14 01:05:07.000000 pydm-1.8.0/pydm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (115)       46 2019-11-14 01:05:07.000000 pydm-1.8.0/pydm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (115)      299 2019-11-14 01:05:07.000000 pydm-1.8.0/pydm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (115)       28 2019-11-14 01:05:07.000000 pydm-1.8.0/pydm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (115)        0 2019-11-14 01:05:07.306913 pydm-1.8.0/pydm_launcher/
--rw-r--r--   0 vsts      (1001) docker     (115)       48 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm_launcher/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (115)     3942 2019-11-14 01:05:02.000000 pydm-1.8.0/pydm_launcher/main.py
--rw-r--r--   0 vsts      (1001) docker     (115)       86 2019-11-14 01:05:02.000000 pydm-1.8.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (115)      167 2019-11-14 01:05:07.306913 pydm-1.8.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (115)     2724 2019-11-14 01:05:02.000000 pydm-1.8.0/setup.py
--rw-r--r--   0 vsts      (1001) docker     (115)    68611 2019-11-14 01:05:02.000000 pydm-1.8.0/versioneer.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2449 2020-01-09 05:06:31.000000 pydm-1.9.0/LICENSE.md
+-rw-r--r--   0 slepicka (1918637911) 1704612529      280 2019-10-07 22:54:10.000000 pydm-1.9.0/MANIFEST.in
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7001 2020-03-24 19:25:57.000000 pydm-1.9.0/PKG-INFO
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5246 2019-10-07 22:54:10.000000 pydm-1.9.0/README.md
+-rw-r--r--   0 slepicka (1918637911) 1704612529       55 2020-01-09 05:06:31.000000 pydm-1.9.0/dev-requirements.txt
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/examples/
+-rw-r--r--   0 slepicka (1918637911) 1704612529        0 2019-03-18 18:59:28.000000 pydm-1.9.0/examples/__init__.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/PyQt/
+-rw-r--r--   0 slepicka (1918637911) 1704612529       22 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/PyQt/Qt.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       25 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/PyQt/QtCore.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       30 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/PyQt/QtDesigner.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       93 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/PyQt/QtGui.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       25 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/PyQt/QtSvg.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       29 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/PyQt/QtWidgets.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      165 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/PyQt/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       23 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/PyQt/uic.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      202 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      497 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/_version.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/about_pydm/
+-rw-r--r--   0 slepicka (1918637911) 1704612529       30 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/about_pydm/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3980 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/about_pydm/about.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5919 2019-08-20 21:48:11.000000 pydm-1.9.0/pydm/about_pydm/about_ui.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      285 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/about_pydm/contributors.txt
+-rw-r--r--   0 slepicka (1918637911) 1704612529    11744 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/application.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      345 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/config.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/connection_inspector/
+-rw-r--r--   0 slepicka (1918637911) 1704612529       53 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/connection_inspector/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3228 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/connection_inspector/connection_inspector.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2811 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/connection_inspector/connection_table_model.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/data_plugins/
+-rw-r--r--   0 slepicka (1918637911) 1704612529     6736 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/data_plugins/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1172 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/data_plugins/archiver_plugin.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1046 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/data_plugins/epics_plugin.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/data_plugins/epics_plugins/
+-rw-r--r--   0 slepicka (1918637911) 1704612529        0 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/data_plugins/epics_plugins/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7196 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/data_plugins/epics_plugins/caproto_plugin_component.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    15649 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/data_plugins/epics_plugins/psp_plugin_component.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7107 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/data_plugins/epics_plugins/pyepics_plugin_component.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1001 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/data_plugins/fake_plugin.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    12561 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/data_plugins/local_plugin.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7050 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/data_plugins/plugin.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     6289 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/default_stylesheet.qss
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8274 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/display.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      398 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/display_module.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5861 2020-03-04 18:42:31.000000 pydm-1.9.0/pydm/exception.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    17444 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/main_window.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    10148 2019-08-20 21:48:11.000000 pydm-1.9.0/pydm/pydm_ui.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2252 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/qtdesigner.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/tests/
+-rw-r--r--   0 slepicka (1918637911) 1704612529        0 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/tests/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2980 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/conftest.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      199 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/test_about_screen.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1359 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/test_data_plugins_import.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1084 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/tests/test_display.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5286 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/test_plugins_import.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/tests/utilities/
+-rw-r--r--   0 slepicka (1918637911) 1704612529        0 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/tests/utilities/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      786 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/utilities/test_colors.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1576 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/utilities/test_iconfont.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2014 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/utilities/test_macro.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      292 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/utilities/test_remove_protocol.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4196 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/utilities/test_stylesheet.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      956 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/utilities/test_units.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1971 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/tests/utilities/test_utilities.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/tests/widgets/
+-rw-r--r--   0 slepicka (1918637911) 1704612529        0 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/tests/widgets/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    19838 2019-11-13 22:41:24.000000 pydm-1.9.0/pydm/tests/widgets/test_base.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3665 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/widgets/test_baseplot.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1725 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_byte.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3865 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_channel.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2832 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_checkbox.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1979 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/widgets/test_colormaps.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5283 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/widgets/test_display_format.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    38864 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_drawing.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8043 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_enum_button.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    10814 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_enum_combo_box.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7540 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_frame.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    23209 2020-03-02 22:56:13.000000 pydm-1.9.0/pydm/tests/widgets/test_label.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    26658 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_lineedit.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1529 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/tests/widgets/test_logdisplay.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    22138 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_pushbutton.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4515 2020-01-14 21:58:52.000000 pydm-1.9.0/pydm/tests/widgets/test_related_display_button.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3379 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/tests/widgets/test_rules.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7824 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/tests/widgets/test_rules_editor.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7708 2020-01-24 21:25:40.000000 pydm-1.9.0/pydm/tests/widgets/test_shell_command.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    22885 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/tests/widgets/test_slider.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    11582 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_spinbox.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      862 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/tests/widgets/test_template_repeater.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8626 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/tests/widgets/test_timeplot.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/tools/
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5717 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/tools/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3376 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/tools/tools.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/utilities/
+-rw-r--r--   0 slepicka (1918637911) 1704612529     9321 2020-03-04 18:42:31.000000 pydm-1.9.0/pydm/utilities/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4720 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/utilities/color2hex.pkl
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1563 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/utilities/colors.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1652 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/utilities/connection.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      259 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/utilities/display_loading.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    20580 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/utilities/fontawesome-charmap.json
+-rw-r--r--   0 slepicka (1918637911) 1704612529   165548 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/utilities/fontawesome.ttf
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4720 2019-03-18 18:59:28.000000 pydm-1.9.0/pydm/utilities/hex2color.pkl
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4789 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/utilities/iconfont.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3857 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/utilities/macro.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529      962 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/utilities/remove_protocol.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3068 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/utilities/stylesheet.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3639 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/utilities/units.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm/widgets/
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1026 2019-11-18 21:25:05.000000 pydm-1.9.0/pydm/widgets/__init__.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    33920 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/base.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    24337 2020-02-07 18:17:07.000000 pydm-1.9.0/pydm/widgets/baseplot.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8151 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/baseplot_curve_editor.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4903 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/widgets/baseplot_table_model.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    15663 2020-02-06 21:42:38.000000 pydm-1.9.0/pydm/widgets/byte.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7023 2020-03-19 00:16:45.000000 pydm-1.9.0/pydm/widgets/channel.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1512 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/checkbox.py
+-rwxr-xr-x   0 slepicka (1918637911) 1704612529    51720 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/colormaps.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2653 2020-02-24 19:41:42.000000 pydm-1.9.0/pydm/widgets/display_format.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    29152 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/drawing.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     9956 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/embedded_display.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8223 2020-02-06 21:42:38.000000 pydm-1.9.0/pydm/widgets/enum_button.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     6696 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/enum_combo_box.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1821 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/widgets/frame.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    19539 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/image.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3867 2020-03-02 22:56:13.000000 pydm-1.9.0/pydm/widgets/label.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    10366 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/line_edit.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8006 2020-02-06 21:42:38.000000 pydm-1.9.0/pydm/widgets/logdisplay.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    11929 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/pushbutton.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5692 2020-03-03 01:23:52.000000 pydm-1.9.0/pydm/widgets/qtplugin_base.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3834 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/qtplugin_extensions.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8544 2019-11-18 21:25:05.000000 pydm-1.9.0/pydm/widgets/qtplugins.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    10042 2020-02-14 00:53:22.000000 pydm-1.9.0/pydm/widgets/related_display_button.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     9543 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/rules.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    18953 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/rules_editor.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    34946 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/scale.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    18137 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/widgets/scatterplot.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3182 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/scatterplot_curve_editor.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7525 2020-01-24 21:25:40.000000 pydm-1.9.0/pydm/widgets/shell_command.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    19982 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/widgets/slider.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     6301 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/spinbox.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     8811 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/symbol.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    11747 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/widgets/tab_bar.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     1437 2019-05-20 21:17:37.000000 pydm-1.9.0/pydm/widgets/tab_bar_qtplugin.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    13989 2020-01-24 18:46:39.000000 pydm-1.9.0/pydm/widgets/template_repeater.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    29524 2020-01-09 05:06:31.000000 pydm-1.9.0/pydm/widgets/timeplot.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2149 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/timeplot_curve_editor.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    19432 2020-02-07 18:17:07.000000 pydm-1.9.0/pydm/widgets/waveformplot.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     3006 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/waveformplot_curve_editor.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529     5433 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm/widgets/waveformtable.py
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/
+-rw-r--r--   0 slepicka (1918637911) 1704612529     7001 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/PKG-INFO
+-rw-r--r--   0 slepicka (1918637911) 1704612529     4337 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/SOURCES.txt
+-rw-r--r--   0 slepicka (1918637911) 1704612529        1 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/dependency_links.txt
+-rw-r--r--   0 slepicka (1918637911) 1704612529       46 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/entry_points.txt
+-rw-r--r--   0 slepicka (1918637911) 1704612529      278 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/requires.txt
+-rw-r--r--   0 slepicka (1918637911) 1704612529       28 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm.egg-info/top_level.txt
+drwxr-xr-x   0 slepicka (1918637911) 1704612529        0 2020-03-24 19:25:57.000000 pydm-1.9.0/pydm_launcher/
+-rw-r--r--   0 slepicka (1918637911) 1704612529       48 2019-03-25 20:13:51.000000 pydm-1.9.0/pydm_launcher/__init__.py
+-rwxr-xr-x   0 slepicka (1918637911) 1704612529     3942 2019-10-07 22:54:10.000000 pydm-1.9.0/pydm_launcher/main.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529       86 2019-04-18 17:07:04.000000 pydm-1.9.0/requirements.txt
+-rw-r--r--   0 slepicka (1918637911) 1704612529      167 2020-03-24 19:25:57.000000 pydm-1.9.0/setup.cfg
+-rw-r--r--   0 slepicka (1918637911) 1704612529     2724 2020-03-24 19:25:45.000000 pydm-1.9.0/setup.py
+-rw-r--r--   0 slepicka (1918637911) 1704612529    68611 2019-03-18 18:59:28.000000 pydm-1.9.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pydm-1.8.0/LICENSE.md` & `pydm-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/PKG-INFO` & `pydm-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydm
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python Display Manager
 Home-page: https://github.com/slaclab/pydm
 Author: SLAC National Accelerator Laboratory
 License: BSD
 Description: [![Build Status](https://dev.azure.com/pydm/pydm/_apis/build/status/slaclab.pydm?branchName=master)](https://dev.azure.com/pydm/pydm/_build/latest?definitionId=1&branchName=master)
         [![codecov](https://codecov.io/gh/slaclab/pydm/branch/master/graph/badge.svg)](https://codecov.io/gh/slaclab/pydm)
         
@@ -148,13 +148,12 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Provides-Extra: perf
-Provides-Extra: PyQt5
 Provides-Extra: PySide
-Provides-Extra: all
 Provides-Extra: pyepics
+Provides-Extra: perf
 Provides-Extra: dev
+Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydm Version: 1.8.0 Summary: Python Display Manager
+Metadata-Version: 2.1 Name: pydm Version: 1.9.0 Summary: Python Display Manager
 Home-page: https://github.com/slaclab/pydm Author: SLAC National Accelerator
 Laboratory License: BSD Description: [![Build Status](https://dev.azure.com/
 pydm/pydm/_apis/build/status/slaclab.pydm?branchName=master)](https://
 dev.azure.com/pydm/pydm/_build/latest?definitionId=1&branchName=master) [!
 [codecov](https://codecov.io/gh/slaclab/pydm/branch/master/graph/badge.svg)]
 (https://codecov.io/gh/slaclab/pydm)
                   ****** PyDM: Python Display Manager ******
@@ -67,10 +67,9 @@
 version.svg)](https://anaconda.org/pydm-tag/pydm) [![Anaconda-Server Badge]
 (https://anaconda.org/pydm-tag/pydm/badges/downloads.svg)](https://
 anaconda.org/pydm-tag/pydm) ```sh conda install -c pydm-tag -c conda-forge pydm
 ``` Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Description-Content-Type: text/markdown Provides-Extra: perf Provides-
-Extra: PyQt5 Provides-Extra: PySide Provides-Extra: all Provides-Extra: pyepics
-Provides-Extra: dev
+:: 3.6 Description-Content-Type: text/markdown Provides-Extra: PySide Provides-
+Extra: pyepics Provides-Extra: perf Provides-Extra: dev Provides-Extra: all
```

### Comparing `pydm-1.8.0/README.md` & `pydm-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/about_pydm/about.py` & `pydm-1.9.0/pydm/about_pydm/about.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/about_pydm/about_ui.py` & `pydm-1.9.0/pydm/about_pydm/about_ui.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/connection_inspector/connection_inspector.py` & `pydm-1.9.0/pydm/connection_inspector/connection_inspector.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/connection_inspector/connection_table_model.py` & `pydm-1.9.0/pydm/connection_inspector/connection_table_model.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/__init__.py` & `pydm-1.9.0/pydm/data_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/archiver_plugin.py` & `pydm-1.9.0/pydm/data_plugins/archiver_plugin.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/epics_plugin.py` & `pydm-1.9.0/pydm/data_plugins/epics_plugin.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/epics_plugins/caproto_plugin_component.py` & `pydm-1.9.0/pydm/data_plugins/epics_plugins/caproto_plugin_component.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/epics_plugins/psp_plugin_component.py` & `pydm-1.9.0/pydm/data_plugins/epics_plugins/psp_plugin_component.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/epics_plugins/pyepics_plugin_component.py` & `pydm-1.9.0/pydm/data_plugins/epics_plugins/pyepics_plugin_component.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/fake_plugin.py` & `pydm-1.9.0/pydm/data_plugins/fake_plugin.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/local_plugin.py` & `pydm-1.9.0/pydm/data_plugins/local_plugin.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/data_plugins/plugin.py` & `pydm-1.9.0/pydm/data_plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/default_stylesheet.qss` & `pydm-1.9.0/pydm/default_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/main_window.py` & `pydm-1.9.0/pydm/main_window.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 from os import path
 from qtpy.QtWidgets import QApplication, QMainWindow, QFileDialog, QWidget, QAction
 from qtpy.QtCore import Qt, QTimer, Slot, QSize, QLibraryInfo
-from .utilities import IconFont, find_display_in_path
+from .utilities import (IconFont, find_file, establish_widget_connections,
+                        close_widget_connections)
 from .pydm_ui import Ui_MainWindow
-from .display_module import Display
+from .display import Display, ScreenTarget, load_file
 from .connection_inspector import ConnectionInspector
 from .about_pydm import AboutWindow
-from .widgets import rules
 from . import data_plugins
 from . import tools
+from .widgets.rules import register_widget_rules, unregister_widget_rules
 import subprocess
 import platform
 import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -27,29 +28,22 @@
         self.ui = Ui_MainWindow()
         self.ui.setupUi(self)
         self._display_widget = None
         self._showing_file_path_in_title_bar = False
         self.default_font_size = QApplication.instance().font().pointSizeF()
         self.ui.navbar.setIconSize(QSize(24, 24))
         self.ui.navbar.setToolButtonStyle(Qt.ToolButtonTextUnderIcon)
-        # No search bar for now, since there isn't really any capability to search yet.
-        # self.searchBar = QLineEdit(self)
-        # self.searchBar.setPlaceholderText("Search")
-        # self.searchBar.setMinimumWidth(150)
-        # self.searchAction = self.ui.navbar.insertWidget(self.ui.actionHome, self.searchBar)
-        self.ui.actionHome.triggered.connect(self.home)
+        self.ui.actionHome.triggered.connect(self.home_triggered)
         self.ui.actionHome.setIcon(self.iconFont.icon("home"))
         self.home_file = None
-        self.back_stack = []
-        self.forward_stack = []
-        self.ui.actionBack.triggered.connect(self.back)
+        self.home_widget = None
+        self.ui.actionBack.triggered.connect(self.back_triggered)
         self.ui.actionBack.setIcon(self.iconFont.icon("angle-left"))
-        self.ui.actionForward.triggered.connect(self.forward)
+        self.ui.actionForward.triggered.connect(self.forward_triggered)
         self.ui.actionForward.setIcon(self.iconFont.icon("angle-right"))
-        # self.ui.goButton.clicked.connect(self.go_button_pressed)
         self.ui.actionEdit_in_Designer.triggered.connect(self.edit_in_designer)
         self.ui.actionOpen_File.triggered.connect(self.open_file_action)
         self.ui.actionReload_Display.triggered.connect(self.reload_display)
         self.ui.actionIncrease_Font_Size.triggered.connect(self.increase_font_size)
         self.ui.actionDecrease_Font_Size.triggered.connect(self.decrease_font_size)
         self.ui.actionDefault_Font_Size.triggered.connect(self.reset_font_size)
         self.ui.actionEnter_Fullscreen.triggered.connect(self.enter_fullscreen)
@@ -85,192 +79,141 @@
             else:
                 designer_path = os.path.join(bin_path, 'designer.exe')
             if os.path.isfile(designer_path):
                 self.designer_path = designer_path
                 break
 
         self.update_tools_menu()
+        self.enable_disable_navigation()
+
+    def display_widget(self):
+        return self._display_widget
 
     def set_display_widget(self, new_widget):
         if new_widget == self._display_widget:
             return
         self.clear_display_widget()
         if not new_widget.layout():
             new_widget.setMinimumSize(new_widget.size())
         self._new_widget_size = new_widget.size()
+        new_widget.setVisible(True)
         self._display_widget = new_widget
         self.setCentralWidget(self._display_widget)
+        self.enable_disable_navigation()
         self.update_window_title()
         # Resizing to the new widget's dimensions needs to be
         # done on the event loop for some reason - you can't
         # just do it here.
         QTimer.singleShot(0, self.resizeForNewDisplayWidget)
 
     def clear_display_widget(self):
         if self._display_widget is not None:
-            self.setCentralWidget(QWidget())
-            rules.unregister_widget_rules(self._display_widget)
-            self._display_widget.deleteLater()
-            self._display_widget = None
+            close_widget_connections(self._display_widget)
+            unregister_widget_rules(self._display_widget)
+            self._display_widget.setVisible(False)
+            self._display_widget.setParent(None)
             self.ui.actionEdit_in_Designer.setEnabled(False)
 
-    def join_to_current_file_path(self, ui_file):
-        ui_file = str(ui_file)
-        # Expand user (~ or ~user) and environment variables.
-        ui_file = os.path.expanduser(os.path.expandvars(ui_file))
-        if path.isabs(ui_file) or len(self.back_stack) == 0:
-            return str(ui_file)
-        else:
-            return path.join(path.dirname(self.current_file()), ui_file)
-
-    def open_file(self, ui_file, macros=None, command_line_args=None):
-        filename = self.join_to_current_file_path(ui_file)
-        try:
-            if not os.path.exists(filename):
-                new_fname = find_display_in_path(ui_file)
-                if new_fname is None or new_fname == "":
-                    raise IOError("File {} not found".format(filename))
-                filename = new_fname
-            self.open_abs_file(filename, macros, command_line_args)
-        except (IOError, OSError, ValueError, ImportError) as e:
-            error_msg = "Cannot open file: '{0}'. Reason: '{1}'.".format(filename, e)
-            logger.error(error_msg)
-            self.statusBar().showMessage(error_msg, 5000)
-
-    def open_abs_file(self, filename, macros=None, command_line_args=None):
-        if command_line_args is None:
-            command_line_args = []
-        merged_macros = self.merge_with_current_macros(macros)
-        widget = self.app.open_file(filename, merged_macros, command_line_args, defer_connections=True)
-        if (len(self.back_stack) == 0) or (self.current_file() != filename) or (macros != self.current_macros()):
-            self.back_stack.append((filename, merged_macros, command_line_args))
-        self.set_display_widget(widget)
-        self.ui.actionForward.setEnabled(len(self.forward_stack) > 0)
-        self.ui.actionBack.setEnabled(len(self.back_stack) > 1)
-        if self.home_file is None:
-            self.home_file = (filename, merged_macros, command_line_args)
-        # Update here the Menu Editor text...
-        ui_file, py_file = self.get_files_in_display()
-        edit_in_text = "Open in "
-        editors = []
-        if ui_file is not None and ui_file != "":
-            editors.append("Designer")
-        if py_file is not None and py_file != "":
-            editors.append("Text Editor")
-        edit_in_text += ' and '.join(editors)
-        self.ui.actionEdit_in_Designer.setText(edit_in_text)
-        if self.designer_path:
-            self.ui.actionEdit_in_Designer.setEnabled(True)
-        data_plugins.establish_queued_connections()
-
-    def new_window(self, ui_file, macros=None, command_line_args=None):
-        filename = self.join_to_current_file_path(ui_file)
-        try:
-            if not os.path.exists(filename):
-                new_fname = find_display_in_path(ui_file)
-                if new_fname is None or new_fname == "":
-                    raise IOError("File {} not found".format(filename))
-                filename = new_fname
-            self.new_abs_window(filename, macros, command_line_args)
-        except (IOError, OSError, ValueError, ImportError) as e:
-            error_msg = "Cannot open file: '{0}'. Reason: '{1}'.".format(filename, e)
-            logger.error(error_msg)
-            self.statusBar().showMessage(error_msg, 5000)
-
-    def new_abs_window(self, filename, macros=None, command_line_args=None):
-        merged_macros = self.merge_with_current_macros(macros)
-        self.app.new_window(filename, merged_macros, command_line_args)
-
-    def go_button_pressed(self):
-        filename = str(self.ui.panelSearchLineEdit.text())
-        if not filename:
-            return
-        try:
-            if QApplication.keyboardModifiers() == Qt.ShiftModifier:
-                self.app.new_window(filename)
-            else:
-                self.go(filename)
-        except (IOError, OSError, ValueError, ImportError) as e:
-            self.handle_open_file_error(filename, e)
-
     def handle_open_file_error(self, filename, error):
         self.statusBar().showMessage("Cannot open file: '{0}', reason: '{1}'...".format(filename, error), 5000)
 
-    # Note: in go(), back(), and forward(), always do history stack manipulation *before* opening the file.
-    # That way, the navigation button enable/disable state will work correctly.  This is stupid, and will be fixed eventually.
-    def go(self, ui_file, macros=None, command_line_args=None):
-        self.forward_stack = []
-        self.open_file(ui_file, macros, command_line_args)
-
-    def go_abs(self, ui_file, macros=None, command_line_args=None):
-        self.forward_stack = []
-        self.open_abs_file(filename=ui_file, macros=macros, command_line_args=command_line_args)
-
-    def back(self):
-        if len(self.back_stack) > 1:
-            if QApplication.keyboardModifiers() == Qt.ShiftModifier:
-                stack_item = self.back_stack[-2]
-                self.new_abs_window(filename=stack_item[0], macros=stack_item[1], command_line_args=stack_item[2])
-            else:
-                self.forward_stack.append(self.back_stack.pop())
-                stack_item = self.back_stack[-1]
-                self.open_abs_file(filename=stack_item[0], macros=stack_item[1], command_line_args=stack_item[2])
-
-    def forward(self):
-        if len(self.forward_stack) > 0:
-            if QApplication.keyboardModifiers() == Qt.ShiftModifier:
-                stack_item = self.forward_stack[-1]
-                self.new_abs_window(filename=stack_item[0], macros=stack_item[1], command_line_args=stack_item[2])
-            else:
-                stack_item = self.forward_stack.pop()
-                self.open_abs_file(filename=stack_item[0], macros=stack_item[1], command_line_args=stack_item[2])
+    def back_triggered(self):
+        new_process = QApplication.keyboardModifiers() == Qt.ShiftModifier
+        self.back(open_in_new_process=new_process)
+
+    def back(self, open_in_new_process=False):
+        curr_display = self.display_widget()
+        prev_display = None
+        if curr_display:
+            prev_display = curr_display.previous_display
 
-    def home(self):
-        if self.home_file is None:
+        if not prev_display:
+            logger.error('No display history to execute back navigation.')
             return
 
-        if QApplication.keyboardModifiers() == Qt.ShiftModifier:
-            self.new_abs_window(filename=self.home_file[0], macros=self.home_file[1], command_line_args=self.home_file[2])
+        if open_in_new_process:
+            load_file(prev_display.loaded_file(),
+                      macros=prev_display.macros,
+                      args=prev_display.args,
+                      target=ScreenTarget.NEW_PROCESS)
         else:
-            self.go_abs(self.home_file[0], macros=self.home_file[1], command_line_args=self.home_file[2])
+            prev_display.next_display = curr_display
+            establish_widget_connections(prev_display)
+            register_widget_rules(prev_display)
+            self.set_display_widget(prev_display)
+
+    def forward_triggered(self):
+        new_process = QApplication.keyboardModifiers() == Qt.ShiftModifier
+        self.forward(open_in_new_process=new_process)
+
+    def forward(self, open_in_new_process=False):
+        curr_display = self.display_widget()
+        next_display = None
+        if curr_display:
+            next_display = curr_display.next_display
 
-    def current_stack_item(self):
-        if len(self.back_stack) == 0:
-            raise IndexError("The display manager does not have a display loaded.")
-        return self.back_stack[-1]
+        if not next_display:
+            logger.error('No display history to execute forward navigation.')
+            return
 
-    def current_file(self):
-        return self.current_stack_item()[0]
+        if open_in_new_process:
+            load_file(next_display.loaded_file(),
+                      macros=next_display.macros,
+                      args=next_display.args,
+                      target=ScreenTarget.NEW_PROCESS)
+        else:
+            establish_widget_connections(next_display)
+            register_widget_rules(next_display)
+            next_display.previous_display = curr_display
+            self.set_display_widget(next_display)
+
+    def home_triggered(self):
+        new_process = QApplication.keyboardModifiers() == Qt.ShiftModifier
+        self.home(open_in_new_process=new_process)
 
-    def current_macros(self):
-        try:
-            return self.current_stack_item()[1]
-        except IndexError:
-            return None
+    def home(self, open_in_new_process=False):
+        if self.home_widget is None:
+            return
 
-    def current_args(self):
-        try:
-            return self.current_stack_item()[2]
-        except IndexError:
-            return None
+        if open_in_new_process:
+            fname = self.home_widget.loaded_file()
+            macros = self.home_widget.macros()
+            args = self.home_widget.args()
+            load_file(fname,
+                      macros=macros,
+                      args=args,
+                      target=ScreenTarget.NEW_PROCESS)
+        else:
+            self.set_display_widget(self.home_widget)
+
+    def enable_disable_navigation(self):
+        w = self.display_widget()
+        if not isinstance(w, Display):
+            # We can't do much if it is not a Display and we don't have the
+            # previous_display and next_display properties since we don't
+            # have the navigation stack set.
+            nav_stack_methods = hasattr(w, 'previous_display') \
+                                and hasattr(w, 'next_display')
+            if not nav_stack_methods:
+                return
+        if not w:
+            self.ui.actionBack.setDisabled(True)
+            self.ui.actionForward.setDisabled(True)
+            return
+        self.ui.actionBack.setDisabled(w.previous_display is None)
+        self.ui.actionForward.setDisabled(w.next_display is None)
 
-    def merge_with_current_macros(self, macros_to_merge):
-        if self.current_macros() is None:
-            return macros_to_merge
-        if macros_to_merge is None:
-            return self.current_macros()
-        m = self.current_macros().copy()
-        m.update(macros_to_merge)
-        return m
+    def current_file(self):
+        return self.display_widget().loaded_file()
 
     def update_window_title(self):
         if self.showing_file_path_in_title_bar:
             title = self.current_file()
         else:
-            title = self._display_widget.windowTitle()
+            title = self.display_widget().windowTitle()
         title += " - PyDM"
         if data_plugins.is_read_only():
             title += " [Read Only Mode]"
         self.setWindowTitle(title)
 
     @property
     def showing_file_path_in_title_bar(self):
@@ -350,36 +293,58 @@
 
     @Slot(bool)
     def open_file_action(self, checked):
         modifiers = QApplication.keyboardModifiers()
         try:
             curr_file = self.current_file()
             folder = os.path.dirname(curr_file)
-        except IndexError:
+        except Exception:
             folder = os.getcwd()
 
         filename = QFileDialog.getOpenFileName(self, 'Open File...', folder, 'PyDM Display Files (*.ui *.py)')
         filename = filename[0] if isinstance(filename, (list, tuple)) else filename
 
         if filename:
             filename = str(filename)
             try:
                 if modifiers == Qt.ShiftModifier:
-                    self.app.new_window(filename)
+                    target = ScreenTarget.NEW_PROCESS
                 else:
-                    self.open_file(filename)
+                    target = None
+                self.open(filename, target=target)
+
             except (IOError, OSError, ValueError, ImportError) as e:
                 self.handle_open_file_error(filename, e)
 
+    def open(self, filename, macros=None, args=None, target=None):
+        if not os.path.isabs(filename):
+            base_path = None
+            curr_display = self.display_widget()
+            if curr_display:
+                base_path = os.path.dirname(curr_display.loaded_file())
+            filename = find_file(filename, base_path=base_path)
+        new_widget = load_file(filename,
+                               macros=macros,
+                               args=args,
+                               target=target)
+        if new_widget:
+            if self.home_widget is None:
+                self.home_widget = new_widget
+            display_widget = self.display_widget()
+            if display_widget:
+                new_widget.previous_display = display_widget
+            self.set_display_widget(new_widget)
+        return new_widget
+
     def load_tool(self, checked):
         try:
             curr_dir = os.path.dirname(self.current_file())
-        except IndexError:
-            logger.error("The display manager does not have a display loaded. Suggesting current work directory.")
+        except Exception:
             curr_dir = os.getcwd()
+            logger.error("The display manager does not have a display loaded. Suggesting current work directory.")
         filename = QFileDialog.getOpenFileName(self, 'Load tool...', curr_dir, 'PyDM External Tool Files (*_tool.py)')
         filename = filename[0] if isinstance(filename, (list, tuple)) else filename
 
         if filename:
             filename = str(filename)
             tools.install_external_tool(filename)
             self.update_tools_menu()
@@ -394,21 +359,31 @@
                                   **kwargs)
 
         self.ui.menuTools.addSeparator()
         self.ui.menuTools.addAction(self.ui.actionLoadTool)
 
     @Slot(bool)
     def reload_display(self, checked):
-        try:
-            curr_file = self.current_file()
-        except IndexError:
+        curr_display = self.display_widget()
+        if not curr_display:
             logger.error("The display manager does not have a display loaded.")
             return
-        self.statusBar().showMessage("Reloading '{0}'...".format(self.current_file()), 5000)
-        self.go_abs(self.current_file())
+
+        prev_display = curr_display.previous_display
+        next_display = curr_display.next_display
+
+        macros = curr_display.macros()
+        args = curr_display.args()
+        loaded_file = curr_display.loaded_file()
+
+        self.statusBar().showMessage(
+            "Reloading '{0}'...".format(self.current_file()), 5000)
+        new_widget = self.open(loaded_file, macros=macros, args=args)
+        new_widget.previous_display = prev_display
+        new_widget.next_display = next_display
 
     @Slot(bool)
     def increase_font_size(self, checked):
         old_factor = self.font_factor
         self.font_factor += 0.1
         self.set_font_size(old_factor, self.font_factor)
 
@@ -455,8 +430,7 @@
 
     def resizeForNewDisplayWidget(self):
         if not self.isFullScreen():
             self.resize(self._new_widget_size)
 
     def closeEvent(self, event):
         self.clear_display_widget()
-        self.app.close_window(self)
```

### Comparing `pydm-1.8.0/pydm/pydm_ui.py` & `pydm-1.9.0/pydm/pydm_ui.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/qtdesigner.py` & `pydm-1.9.0/pydm/qtdesigner.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/conftest.py` & `pydm-1.9.0/pydm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/test_data_plugins_import.py` & `pydm-1.9.0/pydm/tests/test_data_plugins_import.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/test_display.py` & `pydm-1.9.0/pydm/tests/test_display.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 
 # The path to the .ui file used in these tests
 test_ui_path = os.path.join(
     os.path.dirname(os.path.realpath(__file__)),
     "test_data", "test.ui")
 
 
-def test_display_raises_without_filename(qtbot):
-    """If you don't specify a ui_filename argument, or don't reimplement
-    ui_filename(), make sure you get a NotImplementedError."""
-    with pytest.raises(NotImplementedError):
-        my_display = Display(parent=None)
-
-
 def test_ui_filename_arg(qtbot):
     """If you supply a valid filename argument, you shouldn't get any exceptions."""
     my_display = Display(parent=None, ui_filename=test_ui_path)
     qtbot.addWidget(my_display)
 
 
 def test_reimplemented_ui_filename(qtbot):
@@ -37,8 +30,7 @@
 
     class TestDisplay(Display):
         def ui_filename(self):
             return "this_doesnt_exist.ui"
 
     with pytest.raises(IOError):
         my_display = TestDisplay(parent=None)
-
```

### Comparing `pydm-1.8.0/pydm/tests/test_plugins_import.py` & `pydm-1.9.0/pydm/tests/test_plugins_import.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/utilities/test_colors.py` & `pydm-1.9.0/pydm/tests/utilities/test_colors.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/utilities/test_iconfont.py` & `pydm-1.9.0/pydm/tests/utilities/test_iconfont.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/utilities/test_macro.py` & `pydm-1.9.0/pydm/tests/utilities/test_macro.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/utilities/test_stylesheet.py` & `pydm-1.9.0/pydm/tests/utilities/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/utilities/test_units.py` & `pydm-1.9.0/pydm/tests/utilities/test_units.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/utilities/test_utilities.py` & `pydm-1.9.0/pydm/tests/utilities/test_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,32 +29,26 @@
     assert (dir_name == '/bin')
     assert (file_name == 'ls')
     assert (args == [])
 
 
 def test_find_display_in_path():
     temp, file_path = tempfile.mkstemp(suffix=".ui", prefix="display_")
-    print("File Path: ", file_path)
     direc, fname, _ = path_info(file_path)
-
-    print("Direc: ", direc)
     # Try to find the file as is... is should not find it.
     assert(find_display_in_path(fname) is None)
 
     # Try to find the file passing the path
     disp_path = find_display_in_path(fname, mode=None, path=direc)
-    print("Rel Name: {} | Expected: {} | Disp Path: {}".format(fname, direc,
-                                                             disp_path))
     assert(disp_path == file_path)
 
     # Try to find the file passing the path but relative name
     rel_name = ".{}{}".format(os.sep, fname)
     expected = "{}{}{}".format(direc, os.sep, rel_name)
     disp_path = find_display_in_path(rel_name, mode=None, path=direc)
-    print("Rel Name: {} | Expected: {} | Disp Path: {}".format(rel_name, expected, disp_path))
     assert (disp_path == expected)
 
 
 def test_which():
     if platform.system() == 'Windows':
         out = which('ping')
         assert (out.lower() == 'c:\windows\system32\ping.exe')
```

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_base.py` & `pydm-1.9.0/pydm/tests/widgets/test_base.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_baseplot.py` & `pydm-1.9.0/pydm/tests/widgets/test_baseplot.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_byte.py` & `pydm-1.9.0/pydm/tests/widgets/test_byte.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_channel.py` & `pydm-1.9.0/pydm/tests/widgets/test_channel.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_checkbox.py` & `pydm-1.9.0/pydm/tests/widgets/test_checkbox.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_colormaps.py` & `pydm-1.9.0/pydm/tests/widgets/test_colormaps.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_display_format.py` & `pydm-1.9.0/pydm/tests/widgets/test_display_format.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_drawing.py` & `pydm-1.9.0/pydm/tests/widgets/test_drawing.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_enum_button.py` & `pydm-1.9.0/pydm/tests/widgets/test_enum_button.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_enum_combo_box.py` & `pydm-1.9.0/pydm/tests/widgets/test_enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_frame.py` & `pydm-1.9.0/pydm/tests/widgets/test_frame.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_label.py` & `pydm-1.9.0/pydm/tests/widgets/test_label.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,41 +147,39 @@
 
 @pytest.mark.parametrize("value, display_format, unit_name, expected", [
     ("abc", DisplayFormat.Default, "", "abc"),
     (123, DisplayFormat.Default, "", "123"),
     (0b100, DisplayFormat.Default, "", "4"),
     (0x1FF, DisplayFormat.Default, "", "511"),
 
-    ("abc", DisplayFormat.String, "s", "abc"),
+    ("abc", DisplayFormat.String, "s", "abc s"),
     (123, DisplayFormat.String, "s", "123 s"),
     (0b100, DisplayFormat.String, "s", "4 s"),
     (0x1FF, DisplayFormat.String, "s", "511 s"),
 
-    ("abc", DisplayFormat.Decimal, "light years", "abc"), # This setting is acceptable. The displayed value will be "abc"
+    ("abc", DisplayFormat.Decimal, "light years", "abc light years"),
     (123, DisplayFormat.Decimal, "light years", "123 light years"),
     (123.45, DisplayFormat.Decimal, "light years", "123 light years"), # Using default precision of 0
     (0b100, DisplayFormat.Decimal, "light years", "4 light years"),
     (0x1FF, DisplayFormat.Decimal, "light years", "511 light years"),
 
-    # TODO: When parse_value_for_display returns a string, it should still contain the unit.
-    # Right now, value_changed just returns a string as-is, without appending the unit to it.
-    (123, DisplayFormat.Exponential, "ms", "1e+02"),
-    (3.000e-02, DisplayFormat.Exponential, "ms", "3e-02"),
-    (0b100, DisplayFormat.Exponential, "ms", "4e+00"),
-    (0x1FF, DisplayFormat.Exponential, "ms", "5e+02"),
-
-    (123, DisplayFormat.Hex, "ns", "0x7b"),
-    (3.000e-02, DisplayFormat.Hex, "ns", "0x0"),
-    (0b100, DisplayFormat.Hex, "ns", "0x4"),
-    (0x1FF, DisplayFormat.Hex, "ns", "0x1ff"),
-
-    (123, DisplayFormat.Binary, "light years", "0b1111011"),
-    (3.000e-02, DisplayFormat.Binary, "light years", "0b0"),
-    (0b100, DisplayFormat.Binary, "light years", "0b100"),
-    (0x1FF, DisplayFormat.Binary, "light years", "0b111111111"),
+    (123, DisplayFormat.Exponential, "ms", "1e+02 ms"),
+    (3.000e-02, DisplayFormat.Exponential, "ms", "3e-02 ms"),
+    (0b100, DisplayFormat.Exponential, "ms", "4e+00 ms"),
+    (0x1FF, DisplayFormat.Exponential, "ms", "5e+02 ms"),
+
+    (123, DisplayFormat.Hex, "ns", "0x7b ns"),
+    (3.000e-02, DisplayFormat.Hex, "ns", "0x0 ns"),
+    (0b100, DisplayFormat.Hex, "ns", "0x4 ns"),
+    (0x1FF, DisplayFormat.Hex, "ns", "0x1ff ns"),
+
+    (123, DisplayFormat.Binary, "light years", "0b1111011 light years"),
+    (3.000e-02, DisplayFormat.Binary, "light years", "0b0 light years"),
+    (0b100, DisplayFormat.Binary, "light years", "0b100 light years"),
+    (0x1FF, DisplayFormat.Binary, "light years", "0b111111111 light years"),
 ])
 def test_show_units(qtbot, signals, value, display_format, unit_name, expected):
     """
     Test the widget's capability to display a unit following a value if the user enables unit displaying.
 
     Expectations:
     1. The unit will be displayed following a space after the value
```

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_lineedit.py` & `pydm-1.9.0/pydm/tests/widgets/test_lineedit.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_logdisplay.py` & `pydm-1.9.0/pydm/tests/widgets/test_logdisplay.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_pushbutton.py` & `pydm-1.9.0/pydm/tests/widgets/test_pushbutton.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_related_display_button.py` & `pydm-1.9.0/pydm/tests/widgets/test_related_display_button.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_rules.py` & `pydm-1.9.0/pydm/tests/widgets/test_rules.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_rules_editor.py` & `pydm-1.9.0/pydm/tests/widgets/test_rules_editor.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_shell_command.py` & `pydm-1.9.0/pydm/tests/widgets/test_shell_command.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,268 +3,166 @@
 import pytest
 
 import platform
 from logging import ERROR
 
 from qtpy import QtCore
 from qtpy.QtCore import QSize
+from qtpy.QtWidgets import QMenu, QAction
 
 from ...widgets.shell_command import PyDMShellCommand
 from ...utilities import IconFont
 
 
 # --------------------
 # POSITIVE TEST CASES
 # --------------------
 
-@pytest.mark.parametrize("command", [
-    "ping",
-    "",
-    None,
+@pytest.mark.parametrize("command, title", [
+    ("foo", None),
+    ("", None),
+    (None, None),
+    (["foo", "bar"], ["A", "B"]),
 ])
-def test_construct(qtbot, command):
+def test_construct(qtbot, command, title):
     """
     Test the construct of the widget.
 
     Expectations:
-    The widget is initialized with all the expected default values for its properties, including its icon and mouse
-    cursor.
+    The widget is initialized, and the commands and titles match the
+    constructor arguments provided.  Also tests the icon and cursor pixmaps.
 
     Parameters
     ----------
     qtbot : fixture
         Window for widget testing
     command : str
-        The shell command to be executed when the widget is pressed
+        The shell command(s) to be executed when the widget is pressed
+    title : str
+        The titles for the shell commands.  Really only relevant if
+        len(commands) > 1
 
     """
-    pydm_shell_command = PyDMShellCommand(command=command)
-    qtbot.addWidget(pydm_shell_command)
-
-    assert pydm_shell_command._command == command
-    assert pydm_shell_command._allow_multiple is False
-    assert pydm_shell_command.process is None
-    assert pydm_shell_command._show_icon is True
-
+    pydm_shell_command = PyDMShellCommand(command=command, title=title)
+    qtbot.addWidget(pydm_shell_command)
+    if command and isinstance(command, str):
+        assert pydm_shell_command._commands == [command]
+    elif command:
+        assert pydm_shell_command._commands == command
+    else:
+        assert pydm_shell_command._commands == []
+    if title and isinstance(title, str):
+        assert pydm_shell_command._titles == [title]
+    elif title:
+        assert pydm_shell_command._titles == title
+    else:
+        assert pydm_shell_command._titles == []
+    
     DEFAULT_ICON_NAME = "cog"
     DEFAULT_ICON_SIZE = QSize(16, 16)
 
     default_icon = IconFont().icon(DEFAULT_ICON_NAME)
 
     default_icon_pixmap = default_icon.pixmap(DEFAULT_ICON_SIZE)
     shell_cmd_icon_pixmap = pydm_shell_command.icon().pixmap(DEFAULT_ICON_SIZE)
 
     assert shell_cmd_icon_pixmap.toImage() == default_icon_pixmap.toImage()
     assert pydm_shell_command.cursor().pixmap().toImage() == default_icon_pixmap.toImage()
 
-
-@pytest.mark.parametrize("currently_show_icon, to_show_icon", [
-    (True, False),
-    (False, True),
-    (True, True),
-    (False, False),
-    (None, True),
-    (None, False),
-    (True, None),
-    (False, None),
-    (None, None),
-])
-def test_show_icon(qtbot, currently_show_icon, to_show_icon):
-    """
-    Test the widget's show icon setting.
-
-    Expectations:
-    The widget will retain the show icon setting as it is set.
-
-    Parameters
-    ----------
-    qtbot : fixture
-        Window for widget testing
-    currently_show_icon : bool
-        The current show icon setting (True is to show the icon; None otherwise)
-    to_show_icon : bool
-        The next show icon setting (True is to show the icon; None otherwise)
-    """
+def test_deprecated_command_property_with_no_commands(qtbot):
     pydm_shell_command = PyDMShellCommand()
     qtbot.addWidget(pydm_shell_command)
+    pydm_shell_command.command = "test"
+    assert pydm_shell_command.commands == ["test"]
 
-    pydm_shell_command.showIcon = currently_show_icon
-    assert pydm_shell_command.showIcon == currently_show_icon
-
-    pydm_shell_command.showIcon = to_show_icon
-    assert pydm_shell_command.showIcon == to_show_icon
-
-
-@pytest.mark.parametrize("currently_allowed, to_allow", [
-    (True, False),
-    (False, True),
-    (True, True),
-    (False, False),
-    (None, True),
-    (None, False),
-    (True, None),
-    (False, None),
-    (None, None),
-])
-def test_allow_multiple_execs(qtbot, currently_allowed, to_allow):
-    """
-    Test the widget's multiple command execution setting.
-
-    Expectations:
-    The widget will retain the multiple command execution setting as it is set.
-
-    Parameters
-    ----------
-    qtbot : fixture
-       Window for widget testing
-    currently_allowed : bool
-       The current  multiple command execution setting (True is to allow the multiple executions; None otherwise)
-    to_show_icon : bool
-       The next multiple command execution setting (True is to allow the multiple executions; None otherwise)
-    """
-    pydm_shell_command = PyDMShellCommand()
-    qtbot.addWidget(pydm_shell_command)
-
-    pydm_shell_command.allowMultipleExecutions = currently_allowed
-    assert pydm_shell_command.allowMultipleExecutions == currently_allowed
-
-    pydm_shell_command.allowMultipleExecutions = to_allow
-    assert pydm_shell_command.allowMultipleExecutions == to_allow
-
-
-@pytest.mark.parametrize("current_cmd, next_cmd", [
-    ("ping", "pong"),
-    ("ping", "ping"),
-    ("ping", "ping"),
-    ("ping", None),
-    ("", "ping"),
-    ("", ""),
-    (None, "ping"),
-    (None, ""),
-    (None, None)
-])
-def test_get_set_command(qtbot, current_cmd, next_cmd):
-    """
-    Test the widget's capability to set the shell command to execute.
-
-    Expectations:
-    The widget will retain the shell command as set.
-
-    Parameters
-    ----------
-    qtbot : fixture
-       Window for widget testing
-    current_cmd : str
-        The current shell command being set for the widget to execute
-    next_cmd : str
-        The next shell command to set for the widget to execute
-    """
+def test_deprecated_command_property_with_commands(qtbot):
     pydm_shell_command = PyDMShellCommand()
     qtbot.addWidget(pydm_shell_command)
+    existing_commands = ["existing", "commands"]
+    pydm_shell_command.commands = existing_commands
+    pydm_shell_command.command = "This shouldn't work"
+    assert pydm_shell_command.commands == existing_commands
 
-    pydm_shell_command.command = current_cmd
-    assert pydm_shell_command.command == current_cmd
+def test_no_crash_without_any_commands(qtbot):
+     pydm_shell_command = PyDMShellCommand()
+     qtbot.addWidget(pydm_shell_command)
+     pydm_shell_command.commands = None
+     qtbot.mouseClick(pydm_shell_command, QtCore.Qt.LeftButton)
 
-    pydm_shell_command.command = next_cmd
-    assert pydm_shell_command.command == next_cmd
+def test_no_crash_with_none_command(qtbot):
+     pydm_shell_command = PyDMShellCommand()
+     qtbot.addWidget(pydm_shell_command)
+     pydm_shell_command.command = None
+     qtbot.mouseClick(pydm_shell_command, QtCore.Qt.LeftButton)
 
-
-@pytest.mark.parametrize("cmd, val", [
-    ("choice /c yn /d n /t 0" if platform.system() == "Windows" else "sleep 0",
-        2 if platform.system() == "Windows" else 0),
-    ("pydm_shell_invalid_command_test invalid command", None),
-    ("", None),
-    (None, None),
+@pytest.mark.parametrize("cmd, retcode, stdout", [
+    (["choice /c yn /d n /t 0"] if platform.system() == "Windows" else ["sleep 0"],
+        [2] if platform.system() == "Windows" else [0], ["[Y,N]?N"] if platform.system() == "Windows" else [""]),
+    (["pydm_shell_invalid_command_test invalid command"], [None], [""]),
+    (["echo hello", "echo world"], [0, 0], ["hello", "world"])
 ])
-def test_mouse_release_event(qtbot, caplog, cmd, val):
+def test_mouse_release_event(qtbot, caplog, cmd, retcode, stdout):
     """
-    Test to ensure the widget's triggering of the Mouse Release event, which will also execute the shell command.
-
-    Expectations:
+    Test to ensure the widget's triggering of the Mouse Release event.
+    
+    Expectations if len(cmd) == 1:
     1. The mouse release will trigger the current shell command being assigned to the widget to execute
     2. If the command is not valid, there will be an error message in the log
     3. If the command is valid, there will be output in stdout (the result could be a success or failure, but at least
         the command will send out text to stdout)
     4. If the command is None or empty, there will be no output to stdout.
+    
+    Expectations if len(cmd) > 1:
+    1. The mouse press will cause the widget to set its 'menu' attribute to an instance of QMenu.
+    2. Triggering each menu item runs the right command.
 
     Parameters
     ----------
     qtbot : fixture
         Window for widget testing
     caplog : fixture
         To capture the log messages
     cmd : str
         The shell command for the widget to execute
-    val : int
+    retcode : int
         The expected exit code.
+    stdout : str
+        The expected stdout for the command.
     """
     pydm_shell_command = PyDMShellCommand()
     qtbot.addWidget(pydm_shell_command)
 
-    pydm_shell_command.command = cmd
-    qtbot.mouseClick(pydm_shell_command, QtCore.Qt.LeftButton)
-
-    if cmd:
-        if "invalid" not in cmd:
-            ret = pydm_shell_command.process.wait()
-            assert ret == val
+    def check_command_output(command, expected_retcode, expected_stdout):
+        if "invalid" not in command:
+            stdout, stderr = pydm_shell_command.process.communicate()
+            assert pydm_shell_command.process.returncode == expected_retcode
+            assert expected_stdout in str(stdout)
         else:
             for record in caplog.records:
                 assert record.levelno == ERROR
-            assert "Error in command" in caplog.text
-    else:
-        assert pydm_shell_command.process is None
-
-
-@pytest.mark.parametrize("cmd, val", [
-    ("choice /c yn /d n /t 0" if platform.system() == "Windows" else "sleep 0",
-        2 if platform.system() == "Windows" else 0),
-    ("pydm_shell_invalid_command_test invalid command", None),
-    ("", None),
-    (None, None),
-])
-def test_execute_command(qtbot, signals, caplog, cmd, val):
-    """
-    Test to ensure the widget's ability to execute a shell command.
+            assert "Error in shell command" in caplog.text
 
-    Expectations:
-    1. If the command is not valid, there will be an error message in the log
-    2. If the command is valid, there will be output in stdout (the result could be a success or failure, but at least
-        the command will send out text to stdout)
-    3. If the command is None or empty, there will be no output to stdout.
-
-    Parameters
-    ----------
-    qtbot : fixture
-        Window for widget testing
-    signals : fixture
-        The signals fixture, which provides access signals to be bound to the appropriate slots
-    caplog : fixture
-        To capture the log messages
-    cmd : str
-        The shell command for the widget to execute
-    val : int
-        The expected exit code.
-    """
-    pydm_shell_command = PyDMShellCommand()
-    qtbot.addWidget(pydm_shell_command)
-
-    pydm_shell_command.command = cmd
-    signals.send_value_signal[str].connect(pydm_shell_command.execute_command)
-    signals.send_value_signal[str].emit(cmd)
-
-    if cmd:
-        if "invalid" not in cmd:
-            ret = pydm_shell_command.process.wait()
-            assert ret == val
-        else:
-            for record in caplog.records:
-                assert record.levelno == ERROR
-            assert "Error in command" in caplog.text
+    pydm_shell_command.commands = cmd
+    
+    if len(cmd) > 1:
+        for current_command, expected_retcode, expected_stdout in zip(cmd, retcode, stdout):
+            # We can't actually do the click and show the menu - it halts the test and waits
+            # for user input.  So instead, we'll force trigger _rebuild_menu().
+            pydm_shell_command._rebuild_menu()
+            assert isinstance(pydm_shell_command.menu(), QMenu)
+            actions = pydm_shell_command.menu().findChildren(QAction)
+            assert current_command in [a.text() for a in actions]
+            action_for_current_command = [a for a in actions if a.text() == current_command][0]
+            action_for_current_command.trigger()
+            check_command_output(current_command, expected_retcode, expected_stdout)
+    elif len(cmd) == 1:
+        qtbot.mouseClick(pydm_shell_command, QtCore.Qt.LeftButton)
+        check_command_output(cmd[0], retcode[0], stdout[0])
     else:
+        qtbot.mouseClick(pydm_shell_command, QtCore.Qt.LeftButton)
         assert pydm_shell_command.process is None
 
 
 @pytest.mark.parametrize("allow_multiple", [
     True,
     False,
 ])
@@ -290,18 +188,16 @@
     """
     pydm_shell_command = PyDMShellCommand()
     qtbot.addWidget(pydm_shell_command)
 
     pydm_shell_command._allow_multiple = allow_multiple
 
     cmd = "choice /c yn /d y /t 1" if platform.system() == "Windows" else "sleep 0.1"
-    pydm_shell_command.command = cmd
-    signals.send_value_signal[str].connect(pydm_shell_command.execute_command)
-    signals.send_value_signal[str].emit(cmd)
-    signals.send_value_signal[str].emit(cmd)
+    pydm_shell_command.execute_command(cmd)
+    pydm_shell_command.execute_command(cmd)
 
     if not allow_multiple:
         for record in caplog.records:
             assert record.levelno == ERROR
-        assert "Command already active." in caplog.text
+        assert "already active" in caplog.text
     else:
-        assert not caplog.text
+        assert not caplog.text
```

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_slider.py` & `pydm-1.9.0/pydm/tests/widgets/test_slider.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_spinbox.py` & `pydm-1.9.0/pydm/tests/widgets/test_spinbox.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_template_repeater.py` & `pydm-1.9.0/pydm/tests/widgets/test_template_repeater.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,11 +13,10 @@
     # of the template.
     template_repeater = PyDMTemplateRepeater()
     qtbot.addWidget(template_repeater)
     template_repeater.templateFilename = test_template_path
     test_data = [{"devname": "test_device"}]
     template_repeater.data = test_data
     assert template_repeater.count() == len(test_data)
-    print(template_repeater.children())
     slider = template_repeater.findChild(PyDMSlider, "bCtrlSlider")
     assert slider is not None
     assert slider.channel == "ca://{}:BCTRL".format(test_data[0]["devname"])
```

### Comparing `pydm-1.8.0/pydm/tests/widgets/test_timeplot.py` & `pydm-1.9.0/pydm/tests/widgets/test_timeplot.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tools/__init__.py` & `pydm-1.9.0/pydm/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/tools/tools.py` & `pydm-1.9.0/pydm/tools/tools.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/color2hex.pkl` & `pydm-1.9.0/pydm/utilities/color2hex.pkl`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/colors.py` & `pydm-1.9.0/pydm/utilities/colors.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/connection.py` & `pydm-1.9.0/pydm/utilities/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,27 @@
     status : bool
         If True, will call connect on the channels otherwise it will call
         disconnect.
     """
     widgets = [widget]
     widgets.extend(widget.findChildren(QWidget))
     for child_widget in widgets:
-        if hasattr(child_widget, 'channels'):
-            if child_widget.channels() is None:
-                continue
-            for channel in child_widget.channels():
-                if channel is None:
+        try:
+            if hasattr(child_widget, 'channels'):
+                if child_widget.channels() is None:
                     continue
-                if status:
-                    channel.connect()
-                else:
-                    channel.disconnect()
+                for channel in child_widget.channels():
+                    if channel is None:
+                        continue
+                    if status:
+                        channel.connect()
+                    else:
+                        channel.disconnect()
+        except NameError:
+            continue
 
 def establish_widget_connections(widget):
     """
     Connect the inner channels of widgets on the given widget.
 
     Parameters
     ----------
```

### Comparing `pydm-1.8.0/pydm/utilities/fontawesome-charmap.json` & `pydm-1.9.0/pydm/utilities/fontawesome-charmap.json`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/fontawesome.ttf` & `pydm-1.9.0/pydm/utilities/fontawesome.ttf`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/hex2color.pkl` & `pydm-1.9.0/pydm/utilities/hex2color.pkl`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/iconfont.py` & `pydm-1.9.0/pydm/utilities/iconfont.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/macro.py` & `pydm-1.9.0/pydm/utilities/macro.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # Macro parsing states
 PRE_NAME = 0
 IN_NAME = 1
 PRE_VAL = 2
 IN_VAL = 3
 
+
 def substitute_in_file(file_path, macros):
     """
     Substitute the macros given by ${name} at the given file with the entries on the `macros` dictionary.
 
     Parameters
     ----------
     file_path : str
@@ -23,34 +24,33 @@
     -------
     file : io.StringIO
         File-like object with the proper substitutions.
     """
     template = template_for_file(file_path)
     return replace_macros_in_template(template, macros)
 
+
 def replace_macros_in_template(template, macros):
-    expanded_text = template.safe_substitute(macros)
+    curr_template = template
+    prev_template = Template("")
+    expanded_text = ""
+    for i in range(100):
+        expanded_text = curr_template.safe_substitute(macros)
+        if curr_template.template == prev_template.template:
+            break
+        prev_template = curr_template
+        curr_template = Template(expanded_text)
     return io.StringIO(six.text_type(expanded_text))
 
+
 def template_for_file(file_path):
     with open(file_path) as orig_file:
         text = Template(orig_file.read())
     return text
 
-def find_base_macros(widget):
-    '''
-    Find and return the first set of defined base_macros from this widget or
-    its ancestors.
-    '''
-    while widget is not None:
-        if hasattr(widget, 'base_macros'):
-            return widget.base_macros
-        widget = widget.parent()
-    return {}
-
 
 def parse_macro_string(macro_string):
     """Parses a macro string and returns a dictionary.
     First, this method attempts to parse the string as JSON.
     If that fails, it attempts to parse it as an EPICS-style
     macro string.  The parsing algorithm for that case is very
     closely based on macParseDefns in libCom/macUtil.c"""
```

### Comparing `pydm-1.8.0/pydm/utilities/remove_protocol.py` & `pydm-1.9.0/pydm/utilities/remove_protocol.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/stylesheet.py` & `pydm-1.9.0/pydm/utilities/stylesheet.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/utilities/units.py` & `pydm-1.9.0/pydm/utilities/units.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/__init__.py` & `pydm-1.9.0/pydm/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/base.py` & `pydm-1.9.0/pydm/widgets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from qtpy.QtWidgets import (QApplication, QMenu, QGraphicsOpacityEffect,
                             QToolTip, QWidget)
 from qtpy.QtGui import QCursor
 from qtpy.QtCore import Qt, QEvent, Signal, Slot, Property
 from .channel import PyDMChannel
 from .. import data_plugins, tools, config
 from ..utilities import is_qt_designer, remove_protocol
+from ..display import Display
 from .rules import RulesDispatcher
 
 try:
     from json.decoder import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 
@@ -196,14 +197,23 @@
             self._rules = new_rules
             try:
                 rules_list = json.loads(self._rules)
                 RulesDispatcher().register(self, rules_list)
             except JSONDecodeError as ex:
                 logger.exception('Invalid format for Rules')
 
+    def find_parent_display(self):
+        widget = self.parent()
+        while widget is not None:
+            if isinstance(widget, Display):
+                return widget
+            widget = widget.parent()
+        return None
+
+
 class TextFormatter(object):
 
     default_precision_from_pv = True
 
     def __init__(self):
         self._show_units = False
         self.format_string = "{}"
@@ -283,15 +293,15 @@
         Parameters
         ----------
         new_prec : int
             The new precision value to use
         """
         # Only allow one to change the property if not getting the precision
         # from the PV
-        if self.precisionFromPV:
+        if self._precision_from_pv is not None and self._precision_from_pv:
             return
         if new_prec and self._prec != int(new_prec) and new_prec >= 0:
             self._user_prec = int(new_prec)
             if not is_qt_designer() or config.DESIGNER_ONLINE:
                 self.value_changed(self.value)
     
     @Slot(str)
```

### Comparing `pydm-1.8.0/pydm/widgets/baseplot.py` & `pydm-1.9.0/pydm/widgets/baseplot.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/baseplot_curve_editor.py` & `pydm-1.9.0/pydm/widgets/baseplot_curve_editor.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/baseplot_table_model.py` & `pydm-1.9.0/pydm/widgets/baseplot_table_model.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/byte.py` & `pydm-1.9.0/pydm/widgets/byte.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,7 +500,27 @@
         """
         super(PyDMByteIndicator, self).value_changed(new_val)
         try:
             int(new_val)
             self.update_indicators()
         except:
             pass
+
+    def paintEvent(self, _):
+        """
+        Paint events are sent to widgets that need to update themselves,
+        for instance when part of a widget is exposed because a covering
+        widget was moved.
+
+        At PyDMDrawing this method handles the alarm painting with parameters
+        from the stylesheet, configures the brush, pen and calls ```draw_item```
+        so the specifics can be performed for each of the drawing classes.
+
+        Parameters
+        ----------
+        event : QPaintEvent
+        """
+        painter = QPainter(self)
+        opt = QStyleOption()
+        opt.initFrom(self)
+        self.style().drawPrimitive(QStyle.PE_Widget, opt, painter, self)
+        painter.setRenderHint(QPainter.Antialiasing)
```

### Comparing `pydm-1.8.0/pydm/widgets/channel.py` & `pydm-1.9.0/pydm/widgets/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             enum_strings_slot_matched = self.enum_strings_slot == other.enum_strings_slot
             unit_slot_matched = self.unit_slot == other.unit_slot
             prec_slot_matched = self.prec_slot == other.prec_slot
             upper_ctrl_slot_matched = self.upper_ctrl_limit_slot == other.upper_ctrl_limit_slot
             lower_ctrl_slot_matched = self.lower_ctrl_limit_slot == other.lower_ctrl_limit_slot
             write_access_slot_matched = self.write_access_slot == other.write_access_slot
 
-            value_signal_matched = True
+            value_signal_matched = self.value_signal is None and other.value_signal is None
             if self.value_signal and other.value_signal:
                 value_signal_matched = self.value_signal.signal == other.value_signal.signal
 
             return (address_matched and
                     connection_slot_matched and
                     value_slot_matched and
                     severity_slot_matched and
```

### Comparing `pydm-1.8.0/pydm/widgets/checkbox.py` & `pydm-1.9.0/pydm/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/colormaps.py` & `pydm-1.9.0/pydm/widgets/colormaps.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/display_format.py` & `pydm-1.9.0/pydm/widgets/display_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     Decimal = 2
     Exponential = 3
     Hex = 4
     Binary = 5
 
 
 def parse_value_for_display(value, precision, display_format_type=DisplayFormat.Default, string_encoding="utf_8", widget=None):
+    if value is None:
+        return ""
     try:
         widget_name = widget.objectName()
     except(AttributeError, TypeError):
         widget_name = ""
 
     if display_format_type == DisplayFormat.Default:
         return value
```

### Comparing `pydm-1.8.0/pydm/widgets/drawing.py` & `pydm-1.9.0/pydm/widgets/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import math
 import os
 import logging
 
-from qtpy.QtWidgets import (QApplication, QWidget,
-                            QStyle, QStyleOption)
+from qtpy.QtWidgets import (QWidget, QStyle, QStyleOption)
 from qtpy.QtGui import (QColor, QPainter, QBrush, QPen, QPolygon, QPolygonF, QPixmap,
                             QMovie)
-from qtpy.QtCore import Property, Qt, QPoint, QPointF, QSize, Slot
+from qtpy.QtCore import Property, Qt, QPoint, QPointF, QSize, Slot, QTimer
 from qtpy.QtDesigner import QDesignerFormWindowInterface
 from .base import PyDMWidget
-from ..utilities import is_pydm_app, is_qt_designer
+from ..utilities import is_qt_designer, find_file
 
 logger = logging.getLogger(__name__)
 
 
 def deg_to_qt(deg):
     """
     Converts from degrees to QT degrees.
@@ -497,38 +496,43 @@
     def __init__(self, parent=None, init_channel=None, filename=""):
         super(PyDMDrawingImage, self).__init__(parent, init_channel)
         hint = super(PyDMDrawingImage, self).sizeHint()
         self._pixmap = QPixmap(hint)
         self._pixmap.fill(self.null_color)
         self._aspect_ratio_mode = Qt.KeepAspectRatio
         self._movie = None
+        self._file = None
         # Make sure we don't set a non-existant file
         if filename:
             self.filename = filename
         # But we always have an internal value to reference
         else:
             self._file = filename
         if is_qt_designer():  # pragma: no cover
             designer_window = self.get_designer_window()
             if designer_window is not None:
                 designer_window.fileNameChanged.connect(self.designer_form_saved)
+                QTimer.singleShot(200, self.reload_image)
 
     def get_designer_window(self):  # pragma: no cover
         # Internal function to find the designer window that owns this widget.
         p = self.parent()
         while p is not None:
             if isinstance(p, QDesignerFormWindowInterface):
                 return p
             p = p.parent()
         return None
 
     @Slot(str)
     def designer_form_saved(self, filename):  # pragma: no cover
         self.filename = self._file
 
+    def reload_image(self):
+        self.filename = self._file
+
     @Property(str)
     def filename(self):
         """
         The filename of the image to be displayed.
         This can be an absolute or relative path to the display file.
 
         Returns
@@ -554,27 +558,24 @@
         """
         # Expand user (~ or ~user) and environment variables.
         pixmap = None
         self._file = new_file
         abs_path = os.path.expanduser(os.path.expandvars(self._file))
         # Find the absolute path relative to UI
         if not os.path.isabs(abs_path):
-            try:
-                # Based on the QApplication
-                if is_pydm_app():
-                    abs_path = QApplication.instance().get_path(abs_path)
-                # Based on the QtDesigner
-                elif is_qt_designer():  # pragma: no cover
-                    p = self.get_designer_window()
-                    if p is not None:
-                        ui_dir = p.absoluteDir().absolutePath()
-                        abs_path = os.path.join(ui_dir, abs_path)
-            except Exception:
+            parent_display = self.find_parent_display()
+            base_path = None
+            if parent_display:
+                base_path = os.path.dirname(parent_display.loaded_file())
+            abs_path = find_file(abs_path, base_path=base_path)
+            if not abs_path:
                 logger.exception("Unable to find full filepath for %s",
                                  self._file)
+                return
+
         # Check that the path exists
         if os.path.isfile(abs_path):
             if self._movie is not None:
                 self._movie.stop()
                 self._movie.deleteLater()
                 self._movie = None
             if not abs_path.endswith(".gif"):
```

### Comparing `pydm-1.8.0/pydm/widgets/embedded_display.py` & `pydm-1.9.0/pydm/widgets/embedded_display.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from qtpy.QtWidgets import QFrame, QApplication, QLabel, QVBoxLayout, QWidget
 from qtpy.QtCore import Qt, QSize, Property, QTimer
+
+import copy
 import os.path
 import logging
 from .base import PyDMPrimitiveWidget
 from ..utilities import (is_pydm_app, establish_widget_connections,
-                         close_widget_connections, macro, is_qt_designer)
-from ..utilities.display_loading import (load_ui_file, load_py_file)
+                         close_widget_connections, macro, is_qt_designer,
+                         find_file)
+from ..display import (load_file)
 
 logger = logging.getLogger(__name__)
 
+
 class PyDMEmbeddedDisplay(QFrame, PyDMPrimitiveWidget):
     """
     A QFrame capable of rendering a PyDM Display
 
     Parameters
     ----------
     parent : QWidget
@@ -27,22 +31,16 @@
         self._filename = None
         self._macros = None
         self._embedded_widget = None
         self._disconnect_when_hidden = True
         self._is_connected = False
         self._only_load_when_shown = True
         self._needs_load = True
-        self.base_path = ""
-        self.base_macros = {}
-        if is_pydm_app():
-            self.base_path = self.app.directory_stack[-1]
-            self.base_macros = self.app.macro_stack[-1]
-        else:
-            self._load_error_timer = None
-            self._load_error = None
+        self._load_error_timer = None
+        self._load_error = None
         self.layout = QVBoxLayout(self)
         self.err_label = QLabel(self)
         self.err_label.setAlignment(Qt.AlignHCenter)
         self.layout.addWidget(self.err_label)
         self.layout.setContentsMargins(0, 0, 0, 0)
         self.err_label.hide()
         if not is_pydm_app():
@@ -90,15 +88,14 @@
         new_macros : str
         """
         new_macros = str(new_macros)
         if new_macros != self._macros:
             self._macros = new_macros
             self._needs_load = True
             self.load_if_needed()
-        
 
     @Property(str)
     def filename(self):
         """
         Filename of the display to embed.
 
         Returns
@@ -134,17 +131,21 @@
         """
         Dictionary containing the key value pair for each macro specified.
 
         Returns
         --------
         dict
         """
-        m = macro.find_base_macros(self)
-        m.update(macro.parse_macro_string(self.macros))
-        return m
+        parent_display = self.find_parent_display()
+        parent_macros = {}
+        if parent_display:
+            parent_macros = copy.copy(parent_display.macros())
+        widget_macros = macro.parse_macro_string(self.macros)
+        parent_macros.update(widget_macros)
+        return parent_macros
 
     def load_if_needed(self):
         if self._needs_load and (
                 not self._only_load_when_shown or self.isVisible() or is_qt_designer()):
             self.embedded_widget = self.open_file()
 
     def open_file(self, force=False):
@@ -156,65 +157,40 @@
         display : QWidget
         """
         if (not force) and (not self._needs_load):
             return
             
         if not self.filename:
             return
-        # Expand user (~ or ~user) and environment variables.
-        fname = os.path.expanduser(os.path.expandvars(self.filename))
-        if self.base_path:
-            full_fname = os.path.join(self.base_path, fname)
-        else:
-            full_fname = fname
-
-        if not full_fname:
-            return
 
-        if not is_pydm_app():
-            (filename, extension) = os.path.splitext(full_fname)
-            if extension == ".ui":
-                loadfunc = load_ui_file
-            elif extension == ".py":
-                loadfunc = load_py_file
-            else:
-                self.display_error_text('Invalid filename extension.')
-                return
-
-            try:
-                w = loadfunc(full_fname, macros=self.parsed_macros())
-                self._needs_load = False
-                self.clear_error_text()
-                return w
-            except Exception as e:
-                self._load_error = e
-                if self._load_error_timer:
-                    self._load_error_timer.stop()
-                self._load_error_timer = QTimer(self)
-                self._load_error_timer.setSingleShot(True)
-                self._load_error_timer.setTimerType(Qt.VeryCoarseTimer)
-                self._load_error_timer.timeout.connect(self._display_designer_load_error)
-                self._load_error_timer.start(3000)
-            return None
-        
-        # If you get this far, you are running inside a PyDMApplication, load
-        # using that system.
         try:
-            if os.path.isabs(full_fname) and os.path.exists(full_fname):
-                w = self.app.open_file(full_fname, macros=self.parsed_macros())
-            else:
-                w = self.app.open_relative(full_fname, self,
-                                              macros=self.parsed_macros())
+            parent_display = self.find_parent_display()
+            base_path = ""
+            if parent_display:
+                base_path = os.path.dirname(parent_display.loaded_file())
+
+            fname = find_file(self.filename, base_path=base_path)
+            w = load_file(fname, macros=self.parsed_macros(), target=None)
             self._needs_load = False
             self.clear_error_text()
             return w
-        except (ValueError, IOError) as e:
-            self.display_error_text(e)
+        except Exception as e:
+            self._load_error = e
+            if self._load_error_timer:
+                self._load_error_timer.stop()
+            self._load_error_timer = QTimer(self)
+            self._load_error_timer.setSingleShot(True)
+            self._load_error_timer.setTimerType(Qt.VeryCoarseTimer)
+            self._load_error_timer.timeout.connect(self._display_designer_load_error)
+            self._load_error_timer.start(1000)
+        return None
 
     def clear_error_text(self):
+        if self._load_error_timer:
+            self._load_error_timer.stop()
         self.err_label.clear()
         self.err_label.hide()
 
     def display_error_text(self, e):
         self.err_label.setText(
             "Could not open {filename}.\nError: {err}".format(
                 filename=self._filename, err=e))
```

### Comparing `pydm-1.8.0/pydm/widgets/enum_button.py` & `pydm-1.9.0/pydm/widgets/enum_button.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from qtpy.QtCore import (Qt, QSize, Property, Slot, Q_ENUMS)
 from qtpy.QtWidgets import (QWidget, QButtonGroup, QGridLayout, QPushButton,
-                            QRadioButton)
+                            QRadioButton, QStyleOption, QStyle)
+from qtpy.QtGui import QPainter
 
 from .base import PyDMWritableWidget
 from .. import data_plugins
 
 
 class WidgetType(object):
     PushButton = 0
@@ -240,7 +241,27 @@
         """
         if new_enum_strings is not None \
                 and new_enum_strings != self.enum_strings:
             super(PyDMEnumButton, self).enum_strings_changed(new_enum_strings)
             self._has_enums = True
             self.check_enable_state()
             self.rebuild_widgets()
+
+    def paintEvent(self, _):
+        """
+        Paint events are sent to widgets that need to update themselves,
+        for instance when part of a widget is exposed because a covering
+        widget was moved.
+
+        At PyDMDrawing this method handles the alarm painting with parameters
+        from the stylesheet, configures the brush, pen and calls ```draw_item```
+        so the specifics can be performed for each of the drawing classes.
+
+        Parameters
+        ----------
+        event : QPaintEvent
+        """
+        painter = QPainter(self)
+        opt = QStyleOption()
+        opt.initFrom(self)
+        self.style().drawPrimitive(QStyle.PE_Widget, opt, painter, self)
+        painter.setRenderHint(QPainter.Antialiasing)
```

### Comparing `pydm-1.8.0/pydm/widgets/enum_combo_box.py` & `pydm-1.9.0/pydm/widgets/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/frame.py` & `pydm-1.9.0/pydm/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/image.py` & `pydm-1.9.0/pydm/widgets/image.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/label.py` & `pydm-1.9.0/pydm/widgets/label.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         new_value = parse_value_for_display(value=new_value, precision=self.precision,
                                             display_format_type=self._display_format_type,
                                             string_encoding=self._string_encoding,
                                             widget=self)
         # If the value is a string, just display it as-is, no formatting
         # needed.
         if isinstance(new_value, str):
+            if self._show_units and self._unit != "":
+                new_value = "{} {}".format(new_value, self._unit)
             self.setText(new_value)
             return
         # If the value is an enum, display the appropriate enum string for
         # the value.
         if self.enum_strings is not None and isinstance(new_value, int):
             try:
                 self.setText(self.enum_strings[new_value])
```

### Comparing `pydm-1.8.0/pydm/widgets/line_edit.py` & `pydm-1.9.0/pydm/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/logdisplay.py` & `pydm-1.9.0/pydm/widgets/logdisplay.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import functools
 
 from collections import OrderedDict
 
 from qtpy.QtCore import (QObject, Slot, Signal, Property,
                          Q_ENUMS, QSize)
 from qtpy.QtWidgets import (QWidget, QPlainTextEdit, QComboBox, QLabel,
-                            QPushButton, QHBoxLayout, QVBoxLayout)
+                            QPushButton, QHBoxLayout, QVBoxLayout,
+                            QStyleOption, QStyle)
+from qtpy.QtGui import QPainter
 
 logger = logging.getLogger(__name__)
 
 
 def logger_destroyed(log, obj):
     """
     Callback invoked when the Widget is destroyed.
@@ -218,7 +220,27 @@
             logger.exception("Invalid logging level specified %s",
                              level.upper())
         else:
             # Set the existing handler and logger to this level
             self.handler.setLevel(level)
             if self.log.level > self.handler.level or self.log.level == logging.NOTSET:
                 self.log.setLevel(self.handler.level)
+
+    def paintEvent(self, _):
+        """
+        Paint events are sent to widgets that need to update themselves,
+        for instance when part of a widget is exposed because a covering
+        widget was moved.
+
+        At PyDMDrawing this method handles the alarm painting with parameters
+        from the stylesheet, configures the brush, pen and calls ```draw_item```
+        so the specifics can be performed for each of the drawing classes.
+
+        Parameters
+        ----------
+        event : QPaintEvent
+        """
+        painter = QPainter(self)
+        opt = QStyleOption()
+        opt.initFrom(self)
+        self.style().drawPrimitive(QStyle.PE_Widget, opt, painter, self)
+        painter.setRenderHint(QPainter.Antialiasing)
```

### Comparing `pydm-1.8.0/pydm/widgets/pushbutton.py` & `pydm-1.9.0/pydm/widgets/pushbutton.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/qtplugin_base.py` & `pydm-1.9.0/pydm/widgets/qtplugin_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,50 +31,52 @@
     DISPLAY = "PyDM Display Widgets"
     INPUT = "PyDM Input Widgets"
     PLOT = "PyDM Plot Widgets"
     DRAWING = "PyDM Drawing Widgets"
 
 
 def qtplugin_factory(cls, is_container=False, group='PyDM Widgets',
-                     extensions=None):
+                     extensions=None, icon=None):
     """
     Helper function to create a generic PyDMDesignerPlugin class.
 
     :param cls: Widget class
     :type cls:  QWidget
     """
 
     class Plugin(PyDMDesignerPlugin):
         __doc__ = "PyDMDesigner Plugin for {}".format(cls.__name__)
 
         def __init__(self):
-            super(Plugin, self).__init__(cls, is_container, group, extensions)
+            super(Plugin, self).__init__(cls, is_container, group, extensions,
+                                         icon)
 
     return Plugin
 
 
 class PyDMDesignerPlugin(QtDesigner.QPyDesignerCustomWidgetPlugin):
     """
     Parent class to standardize how pydm plugins are accessed in qt designer.
     All functions have default returns that can be overriden as necessary.
     """
 
     def __init__(self, cls, is_container=False, group='PyDM Widgets',
-                 extensions=None):
+                 extensions=None, icon=None):
         """
         Set up the plugin using the class info in cls
 
         :param cls: Class of the widget to use
         :type cls:  QWidget
         """
         QtDesigner.QPyDesignerCustomWidgetPlugin.__init__(self)
         self.initialized = False
         self.is_container = is_container
         self.cls = cls
         self._group = group
+        self._icon = icon or QtGui.QIcon()
         self.extensions = extensions
         self.manager = None
 
     def initialize(self, core):
         """
         Override this function if you need special initialization instructions.
         Make sure you don't neglect to set the self.initialized flag to True
@@ -153,15 +155,15 @@
         """
         return self.is_container
 
     def icon(self):
         """
         Return a QIcon to represent this widget in Qt Designer.
         """
-        return QtGui.QIcon()
+        return self._icon
 
     def domXml(self):
         """
         XML Description of the widget's properties.
         """
         return (
             "<widget class=\"{0}\" name=\"{0}\">\n"
```

### Comparing `pydm-1.8.0/pydm/widgets/qtplugin_extensions.py` & `pydm-1.9.0/pydm/widgets/qtplugin_extensions.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/qtplugins.py` & `pydm-1.9.0/pydm/widgets/qtplugins.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/related_display_button.py` & `pydm-1.9.0/pydm/widgets/related_display_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from qtpy.QtWidgets import QPushButton, QMenu, QAction
-from qtpy.QtGui import QCursor, QIcon
-from qtpy.QtCore import Slot, Property, Qt, QSize, QPoint
+import copy
 import os
-import json
 import logging
 import warnings
 from functools import partial
+
+from qtpy.QtWidgets import QPushButton, QMenu, QAction
+from qtpy.QtGui import QCursor, QIcon
+from qtpy.QtCore import Slot, Property, Qt, QSize, QPoint
+
 from .base import PyDMPrimitiveWidget
-from ..utilities import IconFont
-from ..utilities.macro import find_base_macros, parse_macro_string
+from ..utilities import IconFont, find_file, is_pydm_app
+from ..utilities.macro import parse_macro_string
+from ..display import (load_file, ScreenTarget)
+
 
 logger = logging.getLogger(__name__)
 
 
 class PyDMRelatedDisplayButton(QPushButton, PyDMPrimitiveWidget):
     """
     A QPushButton capable of opening a new Display at the same of at a
@@ -262,32 +266,46 @@
             PyDMRelatedDisplayButton.EXISTING_WINDOW or 0 will open the
             file on the same window. PyDMRelatedDisplayButton.NEW_WINDOW
             or 1 will result on a new process.
         """
         # Check for None and ""
         if not filename:
             return
-        
-        macros = parse_macro_string(macro_string)
-        base_macros = find_base_macros(self)
-        merged_macros = base_macros.copy()
-        merged_macros.update(macros)
-        
+
+        parent_display = self.find_parent_display()
+        base_path = ""
+        macros = {}
+        if parent_display:
+            base_path = os.path.dirname(parent_display.loaded_file())
+            macros = copy.copy(parent_display.macros())
+
+        fname = find_file(filename, base_path=base_path)
+        widget_macros = parse_macro_string(macro_string)
+        macros.update(widget_macros)
+
+        screen_target = None
         if self._shift_key_was_down:
             target = self.NEW_WINDOW
+            screen_target = ScreenTarget.NEW_PROCESS
         if target is None:
             if self._open_in_new_window:
                 target = self.NEW_WINDOW
+                screen_target = ScreenTarget.NEW_PROCESS
             else:
                 target = self.EXISTING_WINDOW
-        if target == self.EXISTING_WINDOW:
-            self.window().go(filename, macros=merged_macros)
-        if target == self.NEW_WINDOW:
-            self.window().new_window(filename,
-                                     macros=merged_macros)
+                screen_target = None
+
+        if is_pydm_app():
+            if target == self.NEW_WINDOW:
+                load_file(fname, macros=macros, target=screen_target)
+            else:
+                self.window().open(fname, macros=macros)
+        else:
+            w = load_file(fname, macros=macros, target=ScreenTarget.DIALOG)
+
 
     def context_menu(self):
         try:
             menu = super(PyDMRelatedDisplayButton, self).context_menu()
         except:
             menu = QMenu(self)
         if len(menu.findChildren(QAction)) > 0:
```

### Comparing `pydm-1.8.0/pydm/widgets/rules.py` & `pydm-1.9.0/pydm/widgets/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,34 @@
             if hasattr(child_widget, 'rules'):
                 if child_widget.rules:
                     RulesDispatcher().unregister(weakref.ref(child_widget))
         except Exception:
             pass
 
 
+def register_widget_rules(widget):
+    """
+    Given a widget to start from, traverse the tree of child widgets,
+    and try to unregister rules to any widgets.
+
+    Parameters
+    ----------
+    widget : QWidget
+    """
+    widgets = [widget]
+    widgets.extend(widget.findChildren(QWidget))
+    for child_widget in widgets:
+        try:
+            if hasattr(child_widget, 'rules'):
+                if child_widget.rules:
+                    RulesDispatcher().register(child_widget, child_widget.rules)
+        except Exception:
+            pass
+
+
 class RulesDispatcher(object):
     """
     Singleton class responsible for handling all the interactions with the
     RulesEngine and dispatch the payloads from the rules thread to the widget.
     """
     __instance = None
```

### Comparing `pydm-1.8.0/pydm/widgets/rules_editor.py` & `pydm-1.9.0/pydm/widgets/rules_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
             prop = self.cmb_property.currentData()
             self.lbl_expected_type.setText(prop[1].__name__)
             idx = self.get_current_index()
             self.change_entry("property", self.cmb_property.currentText())
         except:
             self.lbl_expected_type.setText("")
 
-    def tbl_channels_changed(self, *args, **kwargs):
+    def tbl_channels_changed(self, topleft=None, bottomright=None, roles=None):
         """Callback executed when the channels in the table are modified."""
         if self.loading_data:
             return
 
         new_channels = []
 
         for row in range(self.tbl_channels.rowCount()):
```

### Comparing `pydm-1.8.0/pydm/widgets/scale.py` & `pydm-1.9.0/pydm/widgets/scale.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/scatterplot.py` & `pydm-1.9.0/pydm/widgets/scatterplot.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/scatterplot_curve_editor.py` & `pydm-1.9.0/pydm/widgets/scatterplot_curve_editor.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/slider.py` & `pydm-1.9.0/pydm/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/spinbox.py` & `pydm-1.9.0/pydm/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/symbol.py` & `pydm-1.9.0/pydm/widgets/symbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import os
 import json
 import logging
 from qtpy.QtWidgets import QApplication, QWidget, QStyle, QStyleOption
 from qtpy.QtGui import QPainter, QPixmap
 from qtpy.QtCore import Property, Qt, QSize, QSizeF, QRectF, qInstallMessageHandler
 from qtpy.QtSvg import QSvgRenderer
-from ..utilities import is_pydm_app
+from ..utilities import is_pydm_app, find_file
 from .base import PyDMWidget
 
 logger = logging.getLogger(__name__)
 
 
 class PyDMSymbol(QWidget, PyDMWidget):
     """
@@ -86,23 +87,18 @@
         self._state_images_string = str(new_files)
         try:
             new_file_dict = json.loads(self._state_images_string)
         except Exception:
             self._state_images = {}
             return
         self._sizeHint = QSize(0, 0)
+        parent_display = self.find_parent_display()
+        base_path = os.path.dirname(parent_display.loaded_file())
         for (state, filename) in new_file_dict.items():
-            if is_pydm_app():
-                try:
-                    file_path = self.app.get_path(filename)
-                except Exception as e:
-                    logger.exception("Couldn't get file with path %s", filename)
-                    file_path = filename
-            else:
-                file_path = filename
+            file_path = find_file(filename, base_path=base_path)
             # First, lets try SVG.  We have to try SVG first, otherwise
             # QPixmap will happily load the SVG and turn it into a raster image.
             # Really annoying: We have to try to load the file as SVG,
             # and we expect it will fail often (because many images aren't SVG).
             # Qt prints a warning message to stdout any time SVG loading fails.
             # So we have to temporarily silence Qt warning messages here.
             qInstallMessageHandler(self.qt_message_handler)
```

### Comparing `pydm-1.8.0/pydm/widgets/tab_bar.py` & `pydm-1.9.0/pydm/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/tab_bar_qtplugin.py` & `pydm-1.9.0/pydm/widgets/tab_bar_qtplugin.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/template_repeater.py` & `pydm-1.9.0/pydm/widgets/template_repeater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import json
+import copy
 import logging
 from qtpy.QtWidgets import (QFrame, QApplication, QLabel, QVBoxLayout,
                            QHBoxLayout, QWidget, QStyle, QSizePolicy,
-                           QLayout, QListWidget, QListWidgetItem)
-from qtpy.QtCore import Qt, QSize, QRect, Slot, Property, QPoint, QUrl, Q_ENUMS
-from qtpy import uic
-from .base import PyDMPrimitiveWidget, PyDMWidget
-from .embedded_display import PyDMEmbeddedDisplay
-from pydm.utilities import is_qt_designer, is_pydm_app
+                           QLayout)
+from qtpy.QtCore import Qt, QSize, QRect, Property, QPoint, Q_ENUMS
+from .base import PyDMPrimitiveWidget
+from pydm.utilities import is_qt_designer
 import pydm.data_plugins
-from ..utilities import macro
+from ..utilities import macro, find_file
+from ..display import load_file
 logger = logging.getLogger(__name__)
 
 
 class FlowLayout(QLayout):
     def __init__(self, parent=None, margin=-1, h_spacing=-1, v_spacing=-1):
         QLayout.__init__(self, parent)
         self.setContentsMargins(margin, margin, margin, margin)
@@ -107,21 +107,24 @@
         if not parent:
             return -1
         elif parent.isWidgetType():
             return parent.style().pixelMetric(pm, None, parent)
         else:
             return parent.spacing()
 
+
 class LayoutType(object):
     Vertical = 0
     Horizontal = 1
     Flow = 2
 
+
 layout_class_for_type = (QVBoxLayout, QHBoxLayout, FlowLayout)
 
+
 class PyDMTemplateRepeater(QFrame, PyDMPrimitiveWidget, LayoutType):
     """
     PyDMTemplateRepeater takes a .ui file with macro variables as a template, and a JSON
     file (or a list of dictionaries) with a list of values to use to fill in
     the macro variables, then creates a layout with one instance of the
     template for each item in the list.
 
@@ -135,22 +138,24 @@
     Parameters
     ----------
     parent : optional
         The parent of this widget.
     """
     Q_ENUMS(LayoutType)
     LayoutType = LayoutType
+
     def __init__(self, parent=None):
         QFrame.__init__(self, parent)
         PyDMPrimitiveWidget.__init__(self)
         self._template_filename = ""
         self._count_shown_in_designer = 1
         self._data_source = ""
         self._data = []
         self._cached_template = None
+        self._parent_macros = None
         self._layout_type = LayoutType.Vertical
         self._temp_layout_spacing = 4
         self.app = QApplication.instance()
         self.rebuild()
     
     @Property(LayoutType)
     def layoutType(self):
@@ -175,15 +180,15 @@
         Parameters
         ----------
         new_type : LayoutType
         """
         if new_type != self._layout_type:
             self._layout_type = new_type
             self.rebuild()
-    
+
     @Property(int)
     def layoutSpacing(self):
         if self.layout():
             return self.layout().spacing()
         return self._temp_layout_spacing
     
     @layoutSpacing.setter
@@ -280,32 +285,37 @@
         -------
         data_source : str
         """
         if data_source != self._data_source:
             self._data_source = data_source
             if self._data_source:
                 try:
-                    # Expand user (~ or ~user) and environment variables.
-                    fname = os.path.expanduser(os.path.expandvars(self._data_source))
-                    if is_pydm_app():
-                        # If we're running this inside the PyDM app, we can
-                        # make sure the path is relative to the currently loaded
-                        # display (.ui or .py file).
-                        fname = self.app.get_path(fname)
-                    with open(fname) as f:
-                        try:
-                            self.data = json.load(f)
-                        except ValueError:
-                            logger.error('Failed to parse data source file for PyDMTemplateRepeater.')
-                            self.data = []
+                    parent_display = self.find_parent_display()
+                    base_path = None
+                    if parent_display:
+                        base_path = os.path.dirname(
+                            parent_display.loaded_file())
+                    fname = find_file(self._data_source, base_path=base_path)
+
+                    if not fname:
+                        if not is_qt_designer():
+                            logger.error('Cannot locate data source file {} for PyDMTemplateRepeater.'.format(fname))
+                        self.data = []
+                    else:
+                        with open(fname) as f:
+                            try:
+                                self.data = json.load(f)
+                            except ValueError:
+                                logger.error('Failed to parse data source file {} for PyDMTemplateRepeater.'.format(fname))
+                                self.data = []
                 except IOError as e:
                     self.data = []
             else:
                 self.clear()
-        
+
     def open_template_file(self, variables=None):
         """
         Opens the widget specified in the templateFilename property.
         
         Parameters
         ----------
         variables : dict
@@ -313,28 +323,35 @@
             to all the macros specified on the template repeater widget.
         Returns
         -------
         display : QWidget
         """
         if not variables:
             variables = {}
-        # Expand user (~ or ~user) and environment variables.
-        fname = os.path.expanduser(os.path.expandvars(self.templateFilename))
-        if is_pydm_app():
-            if not self._cached_template:
-                self._cached_template = self.app.open_template(fname)
-            return self.app.widget_from_template(self._cached_template, variables)
-        else:
-            try:
-                f = macro.substitute_in_file(fname, variables)
-                return uic.loadUi(f)
-            except Exception as e:
-                logger.exception("Exception while opening template file.")
-                return None
-       
+
+        parent_display = self.find_parent_display()
+        base_path = None
+        if parent_display:
+            base_path = os.path.dirname(
+                parent_display.loaded_file())
+        fname = find_file(self.templateFilename, base_path=base_path)
+
+        if self._parent_macros is None:
+            self._parent_macros = {}
+            if parent_display:
+                self._parent_macros = parent_display.macros()
+
+        parent_macros = copy.copy(self._parent_macros)
+        parent_macros.update(variables)
+        try:
+            w = load_file(fname, macros=parent_macros, target=None)
+        except Exception as ex:
+            w = QLabel('Error: could not load template: ' + str(ex))
+        return w
+
     def rebuild(self):
         """ Clear out all existing widgets, and populate the list using the
         template file and data source."""
         self.clear()
         if (not self.templateFilename) or (not self.data):
             return
         self.setUpdatesEnabled(False)
@@ -390,9 +407,7 @@
         Sets the dictionary used by the widget to fill in each instance of 
         the template.  This property will be overwritten if the user changes
         the dataSource property.  After setting this property, `rebuild` 
         is automatically called to refresh the widget.
         """
         self._data = new_data
         self.rebuild()
-
-
```

### Comparing `pydm-1.8.0/pydm/widgets/timeplot.py` & `pydm-1.9.0/pydm/widgets/timeplot.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/timeplot_curve_editor.py` & `pydm-1.9.0/pydm/widgets/timeplot_curve_editor.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/waveformplot.py` & `pydm-1.9.0/pydm/widgets/waveformplot.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/waveformplot_curve_editor.py` & `pydm-1.9.0/pydm/widgets/waveformplot_curve_editor.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm/widgets/waveformtable.py` & `pydm-1.9.0/pydm/widgets/waveformtable.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/pydm.egg-info/PKG-INFO` & `pydm-1.9.0/pydm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydm
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python Display Manager
 Home-page: https://github.com/slaclab/pydm
 Author: SLAC National Accelerator Laboratory
 License: BSD
 Description: [![Build Status](https://dev.azure.com/pydm/pydm/_apis/build/status/slaclab.pydm?branchName=master)](https://dev.azure.com/pydm/pydm/_build/latest?definitionId=1&branchName=master)
         [![codecov](https://codecov.io/gh/slaclab/pydm/branch/master/graph/badge.svg)](https://codecov.io/gh/slaclab/pydm)
         
@@ -148,13 +148,12 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Provides-Extra: perf
-Provides-Extra: PyQt5
 Provides-Extra: PySide
-Provides-Extra: all
 Provides-Extra: pyepics
+Provides-Extra: perf
 Provides-Extra: dev
+Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pydm Version: 1.8.0 Summary: Python Display Manager
+Metadata-Version: 2.1 Name: pydm Version: 1.9.0 Summary: Python Display Manager
 Home-page: https://github.com/slaclab/pydm Author: SLAC National Accelerator
 Laboratory License: BSD Description: [![Build Status](https://dev.azure.com/
 pydm/pydm/_apis/build/status/slaclab.pydm?branchName=master)](https://
 dev.azure.com/pydm/pydm/_build/latest?definitionId=1&branchName=master) [!
 [codecov](https://codecov.io/gh/slaclab/pydm/branch/master/graph/badge.svg)]
 (https://codecov.io/gh/slaclab/pydm)
                   ****** PyDM: Python Display Manager ******
@@ -67,10 +67,9 @@
 version.svg)](https://anaconda.org/pydm-tag/pydm) [![Anaconda-Server Badge]
 (https://anaconda.org/pydm-tag/pydm/badges/downloads.svg)](https://
 anaconda.org/pydm-tag/pydm) ```sh conda install -c pydm-tag -c conda-forge pydm
 ``` Platform: UNKNOWN Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 2 Classifier: Programming Language :: Python :: 2.7 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Description-Content-Type: text/markdown Provides-Extra: perf Provides-
-Extra: PyQt5 Provides-Extra: PySide Provides-Extra: all Provides-Extra: pyepics
-Provides-Extra: dev
+:: 3.6 Description-Content-Type: text/markdown Provides-Extra: PySide Provides-
+Extra: pyepics Provides-Extra: perf Provides-Extra: dev Provides-Extra: all
```

### Comparing `pydm-1.8.0/pydm.egg-info/SOURCES.txt` & `pydm-1.9.0/pydm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 versioneer.py
 examples/__init__.py
 pydm/__init__.py
 pydm/_version.py
 pydm/application.py
 pydm/config.py
 pydm/default_stylesheet.qss
+pydm/display.py
 pydm/display_module.py
+pydm/exception.py
 pydm/main_window.py
 pydm/pydm_ui.py
 pydm/qtdesigner.py
 pydm.egg-info/PKG-INFO
 pydm.egg-info/SOURCES.txt
 pydm.egg-info/dependency_links.txt
 pydm.egg-info/entry_points.txt
```

### Comparing `pydm-1.8.0/pydm_launcher/main.py` & `pydm-1.9.0/pydm_launcher/main.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/setup.py` & `pydm-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pydm-1.8.0/versioneer.py` & `pydm-1.9.0/versioneer.py`

 * *Files identical despite different names*

