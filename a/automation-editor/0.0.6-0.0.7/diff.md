# Comparing `tmp/automation_editor-0.0.6.tar.gz` & `tmp/automation_editor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor-0.0.6.tar", last modified: Thu May  4 05:57:52 2023, max compression
+gzip compressed data, was "automation_editor-0.0.7.tar", last modified: Thu May 18 02:14:01 2023, max compression
```

## Comparing `automation_editor-0.0.6.tar` & `automation_editor-0.0.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.692423 automation_editor-0.0.6/
--rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5885 2023-05-04 05:57:52.691424 automation_editor-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.508917 automation_editor-0.0.6/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.535932 automation_editor-0.0.6/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.540932 automation_editor-0.0.6/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-05-03 02:40:57.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.543931 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.549934 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     4000 2023-05-03 02:40:57.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.557931 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-05-03 02:33:10.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.563935 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/install_menu/
--rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
--rw-rw-rw-   0        0        0     2927 2023-05-03 09:50:43.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.570934 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4163 2023-05-03 02:40:57.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.577936 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-05-03 02:39:24.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.584938 automation_editor-0.0.6/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.597463 automation_editor-0.0.6/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.601453 automation_editor-0.0.6/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.606453 automation_editor-0.0.6/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.609452 automation_editor-0.0.6/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.623899 automation_editor-0.0.6/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-05-03 08:50:31.000000 automation_editor-0.0.6/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.630898 automation_editor-0.0.6/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor-0.0.6/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.638895 automation_editor-0.0.6/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.641897 automation_editor-0.0.6/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.648898 automation_editor-0.0.6/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor-0.0.6/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.658897 automation_editor-0.0.6/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.665897 automation_editor-0.0.6/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.672894 automation_editor-0.0.6/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.679906 automation_editor-0.0.6/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.686903 automation_editor-0.0.6/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor-0.0.6/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:57:52.532934 automation_editor-0.0.6/automation_editor.egg-info/
--rw-rw-rw-   0        0        0     5885 2023-05-04 05:57:52.000000 automation_editor-0.0.6/automation_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2023-05-04 05:57:52.000000 automation_editor-0.0.6/automation_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 05:57:52.000000 automation_editor-0.0.6/automation_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-04 05:57:52.000000 automation_editor-0.0.6/automation_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 05:57:52.000000 automation_editor-0.0.6/automation_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1280 2023-05-04 05:57:32.000000 automation_editor-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 05:57:52.693421 automation_editor-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.606707 automation_editor-0.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5885 2023-05-18 02:14:01.605186 automation_editor-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.438042 automation_editor-0.0.7/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.472344 automation_editor-0.0.7/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.476417 automation_editor-0.0.7/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     1622 2023-05-18 02:09:55.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.480947 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.486414 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     4000 2023-05-03 02:40:57.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.491414 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-05-03 02:33:10.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.496989 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
+-rw-rw-rw-   0        0        0     3556 2023-05-18 02:09:55.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.502049 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4163 2023-05-03 02:40:57.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.508111 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-05-03 02:39:24.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.515011 automation_editor-0.0.7/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.522682 automation_editor-0.0.7/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.525716 automation_editor-0.0.7/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.531130 automation_editor-0.0.7/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.534504 automation_editor-0.0.7/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.541175 automation_editor-0.0.7/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-03 08:50:31.000000 automation_editor-0.0.7/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.548221 automation_editor-0.0.7/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor-0.0.7/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.554331 automation_editor-0.0.7/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.556132 automation_editor-0.0.7/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.565199 automation_editor-0.0.7/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor-0.0.7/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.574872 automation_editor-0.0.7/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.581068 automation_editor-0.0.7/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.587145 automation_editor-0.0.7/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.594105 automation_editor-0.0.7/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.600175 automation_editor-0.0.7/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor-0.0.7/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:14:01.468306 automation_editor-0.0.7/automation_editor.egg-info/
+-rw-rw-rw-   0        0        0     5885 2023-05-18 02:14:01.000000 automation_editor-0.0.7/automation_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2023-05-18 02:14:01.000000 automation_editor-0.0.7/automation_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:14:01.000000 automation_editor-0.0.7/automation_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-18 02:14:01.000000 automation_editor-0.0.7/automation_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-18 02:14:01.000000 automation_editor-0.0.7/automation_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1280 2023-05-18 02:13:47.000000 automation_editor-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:14:01.607708 automation_editor-0.0.7/setup.cfg
```

### Comparing `automation_editor-0.0.6/LICENSE` & `automation_editor-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/PKG-INFO` & `automation_editor-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_editor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `automation_editor-0.0.6/README.md` & `automation_editor-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 from PySide6.QtWidgets import QApplication
-from je_editor import EditorMain, shell_manager
+from je_editor import EditorMain, ShellManager
 from qt_material import apply_stylesheet
 
 from automation_editor.automation_editor_ui. \
     menu.api_testka_menu.build_api_testka_menu import set_apitestka_menu
 from automation_editor.automation_editor_ui. \
     menu.auto_control_menu.build_autocontrol_menu import set_autocontrol_menu
 from automation_editor.automation_editor_ui.menu.install_menu.build_install_menu import set_install_menu
@@ -25,16 +25,14 @@
         self.help_menu.deleteLater()
         set_autocontrol_menu(self)
         set_apitestka_menu(self)
         set_load_density_menu(self)
         set_web_runner_menu(self)
         set_install_menu(self)
         syntax_extend_package(self)
-        shell_manager.main_window = self
-        shell_manager.later_init()
         self.setWindowTitle("Automation Editor")
 
 
 def start_editor():
     new_editor = QApplication(sys.argv)
     window = AutomationEditor()
     apply_stylesheet(new_editor, theme='dark_amber.xml')
```

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor-0.0.7/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/exception/exception_tags.py` & `automation_editor-0.0.7/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/exception/exceptions.py` & `automation_editor-0.0.7/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor-0.0.7/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/json_format/json_process.py` & `automation_editor-0.0.7/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor-0.0.7/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor-0.0.7/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor-0.0.7/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor-0.0.7/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor-0.0.7/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor-0.0.7/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/automation_editor.egg-info/PKG-INFO` & `automation_editor-0.0.7/automation_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-editor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `automation_editor-0.0.6/automation_editor.egg-info/SOURCES.txt` & `automation_editor-0.0.7/automation_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.6/pyproject.toml` & `automation_editor-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

