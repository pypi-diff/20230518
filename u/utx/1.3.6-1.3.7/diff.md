# Comparing `tmp/utx-1.3.6.tar.gz` & `tmp/utx-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/utx-pypi/utx-pypi/dist/.tmp-qdr0e8z_/utx-1.3.6.tar", last modified: Mon May 15 14:20:49 2023, max compression
+gzip compressed data, was "/home/runner/work/utx-pypi/utx-pypi/dist/.tmp-bv920h80/utx-1.3.7.tar", last modified: Thu May 18 08:44:41 2023, max compression
```

## Comparing `utx-1.3.6.tar` & `utx-1.3.7.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-15 14:20:37.000000 utx-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 14:20:37.000000 utx-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-15 14:20:49.000000 utx-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-15 14:20:37.000000 utx-1.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:20:49.000000 utx-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-15 14:20:37.000000 utx-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 14:20:37.000000 utx-1.3.6/utx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-05-15 14:20:37.000000 utx-1.3.6/utx/cli/scaffold_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/comparison_table_model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/css/monokai_sublime.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/css/report.css
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/custom_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)  8164040 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/fonts/SourceHanSansCN-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/image/
--rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/broken.png
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/console_hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/console_normal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/download_log.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/eye.svg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/fail.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/less.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/maximize.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/minimize.svg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/more.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/open_in_new_tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/order.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/step_fail.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/step_success.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/success.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/target.png
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/image/time.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35951 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/js/echarts/
--rw-r--r--   0 runner    (1001) docker     (123)   406678 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/echarts/echarts.common.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/echarts/pfm_charts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/echarts/shine.js
--rw-r--r--   0 runner    (1001) docker     (123)   184850 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    93106 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/jquery-1.10.2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24870 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/jquery-lang.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/css/js/langpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/langpack/zh_CN.js
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/lazyload.js
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/paging.js
--rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/js/report.js
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/log_template.html
--rw-r--r--   0 runner    (1001) docker     (123)    22855 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/summary_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/summary_template_pool.html
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/css/summary_template_v2.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/utils/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/utils/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-05-15 14:20:37.000000 utx-1.3.6/utx/core/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/mod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/mod/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/plugins/pg_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/plugins/pg_2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/mod/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/report/pocoui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-15 14:20:37.000000 utx-1.3.6/utx/mod/report/seleniumui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-15 14:20:37.000000 utx-1.3.6/utx/scripts/ipa_pkg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4048 2023-05-15 14:20:37.000000 utx-1.3.6/utx/scripts/ipa_sign.sh
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-15 14:20:37.000000 utx-1.3.6/utx/scripts/plistdump-tcp-proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-15 14:20:37.000000 utx-1.3.6/utx/scripts/run-usbmuxd-proxy.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-15 14:20:37.000000 utx-1.3.6/utx/scripts/uitest_screenrecord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-15 14:20:37.000000 utx-1.3.6/utx/selenium/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35985 2023-05-15 14:20:37.000000 utx-1.3.6/utx/selenium/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx/selenium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:37.000000 utx-1.3.6/utx/selenium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-15 14:20:37.000000 utx-1.3.6/utx/selenium/utils/airtest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30042 2023-05-15 14:20:37.000000 utx-1.3.6/utx/selenium/utils/six.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 14:20:49.000000 utx-1.3.6/utx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-18 08:44:30.000000 utx-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-18 08:44:30.000000 utx-1.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-18 08:44:41.000000 utx-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-18 08:44:30.000000 utx-1.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:44:41.000000 utx-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-18 08:44:30.000000 utx-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-18 08:44:30.000000 utx-1.3.7/utx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-05-18 08:44:30.000000 utx-1.3.7/utx/cli/scaffold_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/comparison_table_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/css/monokai_sublime.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/css/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/custom_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)  8164040 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/fonts/SourceHanSansCN-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/image/
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/broken.png
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/console_hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/console_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/download_log.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/eye.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/fail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/less.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/maximize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/minimize.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/more.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/open_in_new_tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/order.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/step_fail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/step_success.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/success.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/target.png
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/image/time.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35951 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/js/echarts/
+-rw-r--r--   0 runner    (1001) docker     (123)   406678 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/echarts/echarts.common.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/echarts/pfm_charts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/echarts/shine.js
+-rw-r--r--   0 runner    (1001) docker     (123)   184850 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    93106 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/jquery-1.10.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24870 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/jquery-lang.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/css/js/langpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/langpack/zh_CN.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/lazyload.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/paging.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/js/report.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/log_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22855 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/summary_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/summary_template_pool.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/css/summary_template_v2.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/utils/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/utils/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-05-18 08:44:30.000000 utx-1.3.7/utx/core/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/mod/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/plugins/pg_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/plugins/pg_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/mod/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/report/pocoui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-18 08:44:30.000000 utx-1.3.7/utx/mod/report/seleniumui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-18 08:44:30.000000 utx-1.3.7/utx/scripts/ipa_pkg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4048 2023-05-18 08:44:30.000000 utx-1.3.7/utx/scripts/ipa_sign.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-18 08:44:30.000000 utx-1.3.7/utx/scripts/plistdump-tcp-proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-18 08:44:30.000000 utx-1.3.7/utx/scripts/run-usbmuxd-proxy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-18 08:44:30.000000 utx-1.3.7/utx/scripts/uitest_screenrecord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-18 08:44:30.000000 utx-1.3.7/utx/selenium/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35985 2023-05-18 08:44:30.000000 utx-1.3.7/utx/selenium/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx/selenium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:30.000000 utx-1.3.7/utx/selenium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-18 08:44:30.000000 utx-1.3.7/utx/selenium/utils/airtest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30042 2023-05-18 08:44:30.000000 utx-1.3.7/utx/selenium/utils/six.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 08:44:41.000000 utx-1.3.7/utx.egg-info/top_level.txt
```

### Comparing `utx-1.3.6/LICENSE` & `utx-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/PKG-INFO` & `utx-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utx
-Version: 1.3.6
+Version: 1.3.7
 Summary: UTX will help you write ui automated tests more easily!
 Home-page: https://github.com/openutx
 Author: lijiawei
 Author-email: jiawei.li2@qq.com
 License: Apache License 2.0
 Keywords: utx,airtest,pytest,selenium,ui,tools
 Platform: any
```

### Comparing `utx-1.3.6/README.md` & `utx-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/setup.py` & `utx-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/cli/cli.py` & `utx-1.3.7/utx/cli/cli.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/cli/fixture.py` & `utx-1.3.7/utx/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/cli/func.py` & `utx-1.3.7/utx/cli/func.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/cli/plugin.py` & `utx-1.3.7/utx/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/cli/scaffold.py` & `utx-1.3.7/utx/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/cli/scaffold_web.py` & `utx-1.3.7/utx/cli/scaffold_web.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/comparison_table_model.json` & `utx-1.3.7/utx/core/css/comparison_table_model.json`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/css/monokai_sublime.min.css` & `utx-1.3.7/utx/core/css/css/monokai_sublime.min.css`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/css/report.css` & `utx-1.3.7/utx/core/css/css/report.css`

 * *Files 1% similar despite different names*

```diff
@@ -693,15 +693,15 @@
 }
 
 .footer {
   height: 120px;
   color: #999;
   min-width: 1160px;
   border-top: solid 1px #172036;
-  position: absolute;
+  position: relative;
   width: 100%;
   bottom: -219px;
   left: 0;
 }
 .footer-content {
   display: flex;
   align-items: center;
```

### Comparing `utx-1.3.6/utx/core/css/custom_report.py` & `utx-1.3.7/utx/core/css/custom_report.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/fonts/SourceHanSansCN-Regular.ttf` & `utx-1.3.7/utx/core/css/fonts/SourceHanSansCN-Regular.ttf`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.eot` & `utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.svg` & `utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.ttf` & `utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.woff` & `utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/fonts/glyphicons-halflings-regular.woff2` & `utx-1.3.7/utx/core/css/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/arrow.png` & `utx-1.3.7/utx/core/css/image/arrow.png`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/back.svg` & `utx-1.3.7/utx/core/css/image/back.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/broken.png` & `utx-1.3.7/utx/core/css/image/broken.png`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/close.svg` & `utx-1.3.7/utx/core/css/image/close.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/console_hover.svg` & `utx-1.3.7/utx/core/css/image/console_hover.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/console_normal.svg` & `utx-1.3.7/utx/core/css/image/console_normal.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/copy.svg` & `utx-1.3.7/utx/core/css/image/copy.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/download_log.svg` & `utx-1.3.7/utx/core/css/image/download_log.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/eye.svg` & `utx-1.3.7/utx/core/css/image/eye.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/fail.svg` & `utx-1.3.7/utx/core/css/image/fail.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/less.svg` & `utx-1.3.7/utx/core/css/image/less.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/maximize.svg` & `utx-1.3.7/utx/core/css/image/maximize.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/minimize.svg` & `utx-1.3.7/utx/core/css/image/minimize.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/more.svg` & `utx-1.3.7/utx/core/css/image/more.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/open_in_new_tab.svg` & `utx-1.3.7/utx/core/css/image/open_in_new_tab.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/step_fail.svg` & `utx-1.3.7/utx/core/css/image/step_fail.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/step_success.svg` & `utx-1.3.7/utx/core/css/image/step_success.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/success.svg` & `utx-1.3.7/utx/core/css/image/success.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/target.png` & `utx-1.3.7/utx/core/css/image/target.png`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/image/time.svg` & `utx-1.3.7/utx/core/css/image/time.svg`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/bootstrap.min.js` & `utx-1.3.7/utx/core/css/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/echarts/echarts.common.min.js` & `utx-1.3.7/utx/core/css/js/echarts/echarts.common.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/echarts/pfm_charts.js` & `utx-1.3.7/utx/core/css/js/echarts/pfm_charts.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/echarts/shine.js` & `utx-1.3.7/utx/core/css/js/echarts/shine.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/highlight.min.js` & `utx-1.3.7/utx/core/css/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/jquery-1.10.2.min.js` & `utx-1.3.7/utx/core/css/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/jquery-lang.js` & `utx-1.3.7/utx/core/css/js/jquery-lang.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/langpack/zh_CN.js` & `utx-1.3.7/utx/core/css/js/langpack/zh_CN.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/lazyload.js` & `utx-1.3.7/utx/core/css/js/lazyload.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/paging.js` & `utx-1.3.7/utx/core/css/js/paging.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/js/report.js` & `utx-1.3.7/utx/core/css/js/report.js`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/log_template.html` & `utx-1.3.7/utx/core/css/log_template.html`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/report.py` & `utx-1.3.7/utx/core/css/report.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/summary_template.html` & `utx-1.3.7/utx/core/css/summary_template.html`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/summary_template_pool.html` & `utx-1.3.7/utx/core/css/summary_template_pool.html`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/css/summary_template_v2.html` & `utx-1.3.7/utx/core/css/summary_template_v2.html`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/utils/hook.py` & `utx-1.3.7/utx/core/utils/hook.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/utils/runner.py` & `utx-1.3.7/utx/core/utils/runner.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/core/utils/tools.py` & `utx-1.3.7/utx/core/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -569,16 +569,15 @@
         new_report_name = dirs[-1]
         print(f"The new report name: {new_report_name}")
         return new_report_name
 
     def __take_messages(self):
         new_report = self.__get_report()
         self.msg = MIMEMultipart()
-        now = time.strftime("%Y-%m-%d_%H-%M")
-        self.msg["Subject"] = f"UTX自动化{self.title}测试报告_" + now
+        self.msg["Subject"] = self.title
         self.msg["date"] = time.strftime("%Y-%m-%d_%H-%M")
 
         with open(os.path.join(self.report_path, new_report), "rb") as f:
             mail_body = f.read()
         html = MIMEText(mail_body, _subtype="html", _charset="utf-8")
         self.msg.attach(html)
```

### Comparing `utx-1.3.6/utx/mod/load.py` & `utx-1.3.7/utx/mod/load.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/mod/platform.py` & `utx-1.3.7/utx/mod/platform.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/mod/report/pocoui.py` & `utx-1.3.7/utx/mod/report/pocoui.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/mod/report/seleniumui.py` & `utx-1.3.7/utx/mod/report/seleniumui.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/scripts/ipa_pkg.py` & `utx-1.3.7/utx/scripts/ipa_pkg.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/scripts/ipa_sign.sh` & `utx-1.3.7/utx/scripts/ipa_sign.sh`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/scripts/plistdump-tcp-proxy.py` & `utx-1.3.7/utx/scripts/plistdump-tcp-proxy.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/scripts/run-usbmuxd-proxy.sh` & `utx-1.3.7/utx/scripts/run-usbmuxd-proxy.sh`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/scripts/uitest_screenrecord.py` & `utx-1.3.7/utx/scripts/uitest_screenrecord.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/selenium/exceptions.py` & `utx-1.3.7/utx/selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/selenium/proxy.py` & `utx-1.3.7/utx/selenium/proxy.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/selenium/utils/airtest_api.py` & `utx-1.3.7/utx/selenium/utils/airtest_api.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx/selenium/utils/six.py` & `utx-1.3.7/utx/selenium/utils/six.py`

 * *Files identical despite different names*

### Comparing `utx-1.3.6/utx.egg-info/PKG-INFO` & `utx-1.3.7/utx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utx
-Version: 1.3.6
+Version: 1.3.7
 Summary: UTX will help you write ui automated tests more easily!
 Home-page: https://github.com/openutx
 Author: lijiawei
 Author-email: jiawei.li2@qq.com
 License: Apache License 2.0
 Keywords: utx,airtest,pytest,selenium,ui,tools
 Platform: any
```

### Comparing `utx-1.3.6/utx.egg-info/SOURCES.txt` & `utx-1.3.7/utx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

