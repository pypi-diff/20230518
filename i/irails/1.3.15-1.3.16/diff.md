# Comparing `tmp/irails-1.3.15.tar.gz` & `tmp/irails-1.3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.15.tar", last modified: Mon May 15 11:56:31 2023, max compression
+gzip compressed data, was "irails-1.3.16.tar", last modified: Thu May 18 07:50:29 2023, max compression
```

## Comparing `irails-1.3.15.tar` & `irails-1.3.16.tar`

### file list

```diff
@@ -1,92 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.062375 irails-1.3.15/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.15/MANIFEST.in
--rw-rw-rw-   0        0        0     5518 2023-05-15 11:56:31.061379 irails-1.3.15/PKG-INFO
--rw-rw-rw-   0        0        0     4734 2023-05-15 07:02:13.000000 irails-1.3.15/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.975525 irails-1.3.15/irails/
--rw-rw-rw-   0        0        0      307 2023-05-15 11:56:20.000000 irails-1.3.15/irails/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-05-13 06:08:26.000000 irails-1.3.15/irails/_i18n.py
--rw-rw-rw-   0        0        0     2883 2023-05-15 06:36:25.000000 irails-1.3.15/irails/_loader.py
--rw-rw-rw-   0        0        0     3563 2023-05-14 13:31:31.000000 irails-1.3.15/irails/_utils.py
--rw-rw-rw-   0        0        0    11802 2023-05-13 14:57:32.000000 irails-1.3.15/irails/auth.py
--rw-rw-rw-   0        0        0    12679 2023-05-13 15:01:43.000000 irails-1.3.15/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.988142 irails-1.3.15/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.990125 irails-1.3.15/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.15/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.15/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.15/irails/cbv.py
--rw-rw-rw-   0        0        0     6118 2023-05-15 06:53:38.000000 irails-1.3.15/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.15/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24553 2023-05-15 08:05:16.000000 irails-1.3.15/irails/core.py
--rw-rw-rw-   0        0        0     6903 2023-05-14 14:13:03.000000 irails-1.3.15/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.15/irails/log.py
--rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.15/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.15/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.15/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.15/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.003846 irails-1.3.15/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.15/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.15/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6898 2023-05-14 13:32:08.000000 irails-1.3.15/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.15/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.15/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.15/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.15/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.15/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4042 2023-05-15 06:46:20.000000 irails-1.3.15/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2426 2023-05-15 07:00:43.000000 irails-1.3.15/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.933583 irails-1.3.15/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.017513 irails-1.3.15/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.15/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.15/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.15/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.15/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0      999 2023-05-14 14:07:15.000000 irails-1.3.15/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1014 2023-05-14 14:04:24.000000 irails-1.3.15/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.15/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.15/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.15/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.020489 irails-1.3.15/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.15/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.022483 irails-1.3.15/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.15/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.036445 irails-1.3.15/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.15/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.15/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.15/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.15/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.15/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.15/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.15/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.15/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.15/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.936577 irails-1.3.15/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.042439 irails-1.3.15/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.15/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.15/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.15/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.15/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.045421 irails-1.3.15/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.15/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.15/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.048412 irails-1.3.15/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.939569 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.051406 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.056393 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.941563 irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.059384 irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.15/irails/unit_test.py
--rw-rw-rw-   0        0        0     2887 2023-05-12 05:35:40.000000 irails-1.3.15/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.985140 irails-1.3.15/irails.egg-info/
--rw-rw-rw-   0        0        0     5518 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      340 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:56:31.062375 irails-1.3.15/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.665364 irails-1.3.16/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     5518 2023-05-18 07:50:29.664366 irails-1.3.16/PKG-INFO
+-rw-rw-rw-   0        0        0     4734 2023-05-15 07:02:13.000000 irails-1.3.16/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.565266 irails-1.3.16/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-18 07:49:44.000000 irails-1.3.16/irails/__init__.py
+-rw-rw-rw-   0        0        0     3948 2023-05-18 07:35:56.000000 irails-1.3.16/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2873 2023-05-16 07:25:29.000000 irails-1.3.16/irails/_loader.py
+-rw-rw-rw-   0        0        0     3545 2023-05-16 07:12:34.000000 irails-1.3.16/irails/_utils.py
+-rw-rw-rw-   0        0        0    11909 2023-05-16 08:07:09.000000 irails-1.3.16/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.16/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.577236 irails-1.3.16/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.579231 irails-1.3.16/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.16/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.16/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.16/irails/cbv.py
+-rw-rw-rw-   0        0        0     6118 2023-05-15 06:53:38.000000 irails-1.3.16/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.16/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24864 2023-05-18 07:46:03.000000 irails-1.3.16/irails/core.py
+-rw-rw-rw-   0        0        0     7871 2023-05-18 07:46:03.000000 irails-1.3.16/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.16/irails/log.py
+-rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.16/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.16/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.16/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.16/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.591864 irails-1.3.16/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.16/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.16/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6898 2023-05-14 13:32:08.000000 irails-1.3.16/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.16/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.16/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.16/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.16/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.16/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4042 2023-05-15 06:46:20.000000 irails-1.3.16/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2426 2023-05-15 07:00:43.000000 irails-1.3.16/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.525398 irails-1.3.16/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.605284 irails-1.3.16/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.16/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.16/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.16/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.16/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0      999 2023-05-14 14:07:15.000000 irails-1.3.16/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0     1014 2023-05-14 14:04:24.000000 irails-1.3.16/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.16/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.16/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.16/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.607279 irails-1.3.16/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.16/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.609278 irails-1.3.16/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.16/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.623236 irails-1.3.16/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.16/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.16/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.16/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.640190 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.16/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.16/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.16/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.16/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.16/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.530383 irails-1.3.16/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.644938 irails-1.3.16/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.16/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.16/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.16/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.16/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.648409 irails-1.3.16/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.16/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.16/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.651415 irails-1.3.16/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.534373 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.655392 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.660384 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.535371 irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.662377 irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.16/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.16/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:50:29.573248 irails-1.3.16/irails.egg-info/
+-rw-rw-rw-   0        0        0     5518 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3088 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      360 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 07:50:29.000000 irails-1.3.16/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 07:50:29.665364 irails-1.3.16/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.16/setup.py
```

### Comparing `irails-1.3.15/PKG-INFO` & `irails-1.3.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.15
+Version: 1.3.16
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.15/README.md` & `irails-1.3.16/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/_i18n.py` & `irails-1.3.16/irails/_i18n.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,108 +4,121 @@
 
 import os,sys
 import gettext
 from typing import Union
 _default_localedir = os.path.join(sys.base_prefix, 'share', 'locale')
 _old_find = gettext.find
 
-# Locate a .mo file using the gettext strategy
-def __new_find(domain, localedir=None, languages=None, all=False):
-    # Get some reasonable defaults for arguments that were not supplied
-    if localedir is None:
-        localedir = _default_localedir
-    if languages is None:
-        languages = []
-        for envar in ('LANGUAGE', 'LC_ALL', 'LC_MESSAGES', 'LANG'):
-            val = os.environ.get(envar)
-            if val:
-                languages = val.split(':')
-                break
-        if 'C' not in languages:
-            languages.append('C')
-    # now normalize and expand the languages
-    nelangs = []
-    for lang in languages:
-        for nelang in gettext._expand_lang(lang):
-            if nelang not in nelangs:
-                nelangs.append(nelang)
-    # select a language
-    if all:
-        result = []
-    else:
-        result = None
-    for lang in nelangs:
-        
-        if lang == 'C':
-            break
-        # mofile = os.path.join(localedir, lang, 'LC_MESSAGES', '%s.mo' % domain)
-        check_compile_po(localedir,lang)
-        mofile = os.path.join(localedir, f'{lang}.mo')
-        if os.path.exists(mofile):
-            
-            if all:
-                result.append(mofile)
-            else:
-                return mofile
-        
-    return result
-
-gettext.find=__new_find #rewrite find method
 
+def load_module(module_name:str,module_path:str):
+    if os.path.exists(module_path):
+        spec = importlib.util.spec_from_file_location(module_name, module_path)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+        return module
+    return None
 def check_compile_po(localedir,lang): 
     po_file = os.path.join(localedir, f'{lang}.po') 
     mo_file = os.path.join(localedir, f'{lang}.mo')
-    def do_command():
-        from ._loader import load_module
+    def do_mfgmft():
+         
         _tools_file = os.path.join(sys.prefix,'Tools','i18n',f"msgfmt.py")
         module = load_module('mfgmft',_tools_file)
         if module:
             module.make(po_file,mo_file)
         else:
             print(f"not found tools file : {_tools_file}")
     # 判断po文件是否存在
     if os.path.exists(po_file): 
         if os.path.exists(mo_file):
             mod_time =  (os.stat(mo_file).st_mtime)
         else:
             mod_time = 0
         pod_time =  (os.stat(po_file).st_mtime) 
         if pod_time>mod_time: 
-            do_command()
+            do_mfgmft()
 # 获取当前模块的 ModuleSpec 实例
-module_spec = importlib.util.find_spec(__name__)
+# module_spec = importlib.util.find_spec(__name__)
 
-__all_trans = {}           
-def load_app_translations(module_dir,is_core:bool=False,lan=None) -> gettext.GNUTranslations: 
+__all_trans = {}          
+default_langs = ['en','zh'] 
+def load_app_translations(module_dir,lan=None) -> gettext.GNUTranslations: 
     global __all_trans
     
-    if not is_core and not lan:
+    if  not lan:
         from .config import config
         cfg = config.get('i18n')
         if not cfg:
-            lan = ['en','zh']
+            lan = default_langs
         else:
-            lan = cfg.get('lang',['en','zh'])
+            lan = cfg.get('lang',default_langs)
         if not isinstance(lan,list):
             lan=[lan]
-    else:
-        if not lan:
-            lan = ['en','zh']
+    
 
     key = f"{module_dir}@{lan}"
     if key in __all_trans:
         return __all_trans[key]
     # 加载翻译文件
     locales_dir = os.path.join(module_dir, "locales")
     ret = None
     try:
         
         ret = gettext.translation("messages", locales_dir, languages=lan) 
         ret.install()
     except Exception as e:
+         
         ret = gettext
     
     #cache item
     __all_trans[key] = ret
     return ret
  
- 
+ 
+def __load_core_i18n():
+
+    _dir = os.path.dirname(__file__)
+    # Locate a .mo file using the gettext strategy
+    def __new_find(domain, localedir=None, languages=None, all=False):
+        # Get some reasonable defaults for arguments that were not supplied
+        if localedir is None:
+            localedir = _default_localedir
+        if languages is None:
+            languages = []
+            for envar in ('LANGUAGE', 'LC_ALL', 'LC_MESSAGES', 'LANG'):
+                val = os.environ.get(envar)
+                if val:
+                    languages = val.split(':')
+                    break
+            if 'C' not in languages:
+                languages.append('C')
+        # now normalize and expand the languages
+        nelangs = []
+        for lang in languages:
+            for nelang in gettext._expand_lang(lang):
+                if nelang not in nelangs:
+                    nelangs.append(nelang)
+        # select a language
+        if all:
+            result = []
+        else:
+            result = None
+        for lang in nelangs:
+            
+            if lang == 'C':
+                break
+            # mofile = os.path.join(localedir, lang, 'LC_MESSAGES', '%s.mo' % domain)
+            check_compile_po(localedir,lang)
+            mofile = os.path.join(localedir, f'{lang}.mo')
+            if os.path.exists(mofile):
+                
+                if all:
+                    result.append(mofile)
+                else:
+                    return mofile
+            
+        return result
+
+    gettext.find=__new_find #rewrite find method
+    t = load_app_translations(_dir)
+    return  t.gettext
+_=__load_core_i18n()
```

### Comparing `irails-1.3.15/irails/_loader.py` & `irails-1.3.16/irails/_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import sys,os
 from .config import config,ROOT_PATH 
 from ._i18n import load_app_translations
-from gettext import gettext as _
+from ._i18n import   _
 
 app_dirs = []
 app_enabled = []
 
 
 def __list_directories(dir):
     """
```

### Comparing `irails-1.3.15/irails/_utils.py` & `irails-1.3.16/irails/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,24 +53,25 @@
             file.write(line_to_add)
         return True              
     # If the line is not in the file, add it
     if not found:
         lines.append('\n' + line_to_add.strip() + '\n')
         with open(filepath, 'w') as file:
             file.writelines(lines)
+_datetime_regex = re.compile(
+r'^\d{4}-\d{2}-\d{2}(T\d{2}:\d{2}:\d{2}(\.\d+)?(Z|[+-]\d{2}:\d{2})?)?$'
+)
+
+_date_regex = re.compile(r'^\d{4}-\d{2}-\d{2}$')
+
+_time_regex = re.compile(r'^\d{2}:\d{2}:\d{2}$')
 def is_datetime_format(s):
     if not isinstance(s,str) or not str:
         return False 
-    _datetime_regex = re.compile(
-        r'^\d{4}-\d{2}-\d{2}(T\d{2}:\d{2}:\d{2}(\.\d+)?(Z|[+-]\d{2}:\d{2})?)?$'
-    )
-
-    _date_regex = re.compile(r'^\d{4}-\d{2}-\d{2}$')
-
-    _time_regex = re.compile(r'^\d{2}:\d{2}:\d{2}$')
+    
     def is_valid_datetime_string(datetime_str):
         return bool(_datetime_regex.match(datetime_str))
 
     def is_valid_date_string(date_str):
         return bool(_date_regex.match(date_str))
 
     def is_valid_time_string(time_str):
```

### Comparing `irails-1.3.15/irails/auth.py` & `irails-1.3.16/irails/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  
 from .config import config,ROOT_PATH
 from .log import _log
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Type, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
-
+from ._i18n import _
 AUTH_EXPIRED='[EXPIRED]!'
 
 _session_name:str = ""
 
 class CasbinAuth:
     def __init__(self,enforcer:Enforcer,session_name="user") -> None:
         global _session_name
@@ -56,17 +56,17 @@
 
         return self.enforcer.enforce(user, path, method)
     def __get_token_from_header(self, authorization: str, prefix: str) -> str:
         """Parses the Authorization header and returns only the token"""
         try:
             scheme, token = authorization.split()
         except ValueError as e:
-            raise AuthenticationError('Could not separate Authorization scheme and token') from e 
+            raise AuthenticationError(_('Could not separate Authorization scheme and token')) from e 
         if scheme.lower() != prefix.lower():
-            raise AuthenticationError(f'Authorization scheme {scheme} is not supported')
+            raise AuthenticationError( _('Authorization scheme %s is not supported') % {scheme})
         return token
     def get_user_from_request(self,request:Request,prefix:str="Bearer",is_jwt:bool=False,**kwargs) : 
         userobj = request.session.get(self.__session_name)
         payload = None
         username = ''
        
         if is_jwt:   
@@ -76,15 +76,16 @@
                 scheme, credentials = auth.split() 
                 token = self.__get_token_from_header(authorization=auth, prefix=prefix)
                 
                 del kwargs['username_field']
                 try:
                     payload = jwt.decode(token,**kwargs)
                 except jwt.InvalidTokenError as e:
-                    _log.debug('token:'+token + f' has been expired.{e.args}')
+                    msg = _('token %s has been expired(%s)'%(token,e.args))
+                    _log.debug(msg)
                     request.session[self.__session_name] = None
                     return "","",None
                 if is_datetime_format(payload['exp']):
                     payload['exp'] = datetime.fromisoformat(payload['exp'])
 
 
                 return  payload[username_field],token,payload
@@ -224,24 +225,24 @@
                 expires_delta = int(authCfg.get('expires_delta',60))
             else:
                 expires_delta = 60
             expire = datetime.utcnow() + timedelta(
                 minutes=expires_delta
             )
         if isinstance(user,str):
-            userObj = {"exp": expire, "username": user }
+            auth_user_obj = {"exp": expire, "username": user }
         elif isinstance(user,JWTUser):
-            userObj = {"exp": expire, "username": user.username}
+            auth_user_obj = {"exp": expire, "username": user.username}
         elif isinstance(user,BaseUser):
-            userObj = {"exp": expire, "username": user.display_name}
+            auth_user_obj = {"exp": expire, "username": user.display_name}
         request:Request = kwargs['request']
         
-        access_token = jwt.encode(userObj, self.secret_key ,self.algorithm )
-        userObj.update({"token":access_token})
-        request.session[_session_name] = userObj
+        access_token = jwt.encode(auth_user_obj, self.secret_key ,self.algorithm )
+        auth_user_obj.update({"token":access_token})
+        request.session[_session_name] = auth_user_obj
         return access_token
     
 _casbin_auth:CasbinAuth = None
 
 def init(app:FastAPI,backend:AuthenticationBackend,adapter_class:Type=None,**kwagrs)->AuthenticationBackend:
     """
         kwargs:secret_key=KEY
@@ -280,9 +281,9 @@
     module_dir = os.path.dirname(__file__)
     module_dir = os.path.join(module_dir,'casbin_adapters')
     module_path = os.path.join(module_dir, module_name + '.py') 
     module = load_module(module_name,module_path)
     if module and hasattr(module,'Adapter'):
         return getattr(module,'Adapter')   
     else:
-        raise RuntimeError("Can't load module:{module_path}")
+        raise RuntimeError(_("Can't load module:%s") % module_path)
```

### Comparing `irails-1.3.15/irails/base_controller.py` & `irails-1.3.16/irails/base_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from .log import _log
 import os,uuid
 from hashlib import md5
 from typing import Dict
 from logging import Logger
 import inspect
 import datetime
-from irails._i18n import load_app_translations
- 
+from irails._i18n import load_app_translations,_
+
 __session_config = config.get('session') 
 _session_key = "session_id"
 alow_extensions = []
 MAX_UPLOAD_LEN = -1
 MAX_FILES = 1
 if __session_config:
     _session_key = __session_config.get("key","session_id")
@@ -60,20 +60,20 @@
             
         url_path = "/"+"/".join(pairs)  + "/"
     return url_path.lower() + url.strip()
 
 class BaseController:
     @property
     def _(self):
-        m = getattr(self,'__appdir__').split(os.sep)
-        if len(m)>2:
-            m = os.sep.join(m[-2:])
-        else:
-            raise RuntimeError(f"load_app_translations:{m} is invalid app module") 
-        languages = ['zh']
+        m = getattr(self,'__appdir__')#.split(os.sep)
+        # if len(m)>2:
+        #     m = os.sep.join(m[-2:])
+        # else:
+        #     raise RuntimeError(_("load_app_translations:%s is invalid app module") % m) 
+        languages = None
         if 'lang' in self._session:
             languages = self._session['lang']
         else:
             language_header = self._request.headers.get('accept-language')
             if language_header:
                 languages = language_header.split(',')
                 if languages:
@@ -269,15 +269,15 @@
         params = {}
         form_params = {}
         query_params = {}
         json_params = {}
         try:
             form_params =  await  request.form()
         except Exception as e:
-            _log.info("while parse form raised:"+str(e.args))
+            _log.info(_("when parsing `Form params` raised:")+str(e.args))
             pass
 
         
         try:
             json_params =  await  request.json()
         except:
             pass
```

### Comparing `irails-1.3.15/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.16/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.16/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/cbv.py` & `irails-1.3.16/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/config.py` & `irails-1.3.16/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/controller_utils.py` & `irails-1.3.16/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/core.py` & `irails-1.3.16/irails/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,29 @@
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 from . import database
 from ._loader import _load_apps
 from ._utils import get_controller_name,get_snaked_name
-from ._i18n import load_app_translations
-_=None
+
+from ._i18n import _
+
+
 __is_debug=config.get('debug',False)
 
-def __load_core_i18n():
-    _dir = os.path.dirname(__file__)
-    t = load_app_translations(_dir,True)
-    global _
-    _ = t.gettext
-__load_core_i18n()
+def singleton(cls):
+    instances = {}
+    def get_instance(*args,**kwargs):
+        if cls not in instances:
+            instances[cls] = cls(*args,**kwargs)
+        return instances[cls]
+    return get_instance
 
+@singleton
 class MvcApp(FastAPI):
     def __init__(self,  **kwargs):
         self.__authObj:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
         self.__user_auth_url=""
         self.__public_auth_url=""
         self.__app_views_dirs = {} 
@@ -208,40 +212,40 @@
             __all_controller__[_controller_hash] = {'label':'new','obj': _controllerBase}
 
         class puppetController( targetController ,_controllerBase ): 
             '''puppet class inherited by the User defined controller class '''
             def __init__(self,**kwags) -> None: 
                 
                 super().__init__()
-            def _user_logout(self,msg=_('your are successed logout!'),redirect:str="/"):
+            def _user_logout(self,msg=_('you are successed logout!'),redirect:str="/"):
                 """see .core.py"""
                 self.flash  = msg
                 if  hasattr(application,'authObj'):
                     application.authObj.clear_userinfo(request=self.request)
                 accept_header = self.request.headers.get("Accept")    
                 if accept_header == "application/json":
                     return {'status':'success','msg':msg}
                 else:
                     return self.redirect(redirect)
-            def _verity_successed(self,user, msg=_("User authentication successed!"),redirect_url='/'):
+            def _verity_successed(self,user, msg=_("User authentication successed!"),redirect='/'):
                 '''call by targetController''' 
                  
                 self.flash  = msg
                 accept_header = self._request.headers.get("Accept")
                 if  hasattr(application,'authObj'):
                     access_token = application.authObj.create_access_token(user,request=self.request)
                 
                     if accept_header == "application/json":
                         return {'status':'success','msg':msg,'token':str(access_token)}
                      
                 else:  
                     if accept_header == "application/json":
                         return {'status':'success','msg':msg }
                  
-                return RedirectResponse(redirect_url,status_code=StateCodes.HTTP_303_SEE_OTHER)
+                return RedirectResponse(redirect,status_code=StateCodes.HTTP_303_SEE_OTHER)
             def _verity_error(self,msg=_("User authentication failed!")):
                 '''call by targetController'''
                  
                 self.flash  = msg 
                 
                 accept_header = self.request.headers.get("Accept")
                 if accept_header == "application/json":
@@ -389,33 +393,35 @@
     _register_controllers()
 
     
     if __is_debug:
         _log.info(_("checking database configure..."))
     check_init_database()
 
-    auth_type = config.get("auth",None)
-    _casbin_adapter_class=None
-    _adapter_uri:str=None
+    # Initializing the authentication system
+    auth_type = config.get("auth", None)
+    _casbin_adapter_class = None
+    _adapter_uri: str = None
     if auth_type:
-        auth_type=auth_type.get("type" )
+        auth_type = auth_type.get("type")
         if auth_type:
-            __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
-            _casbin_adapter_class =  auth.get_adapter_module(__type_casbin_adapter)
-            _adapter_uri = config.get("auth").get("adapter_uri") 
+            # Get the adapter type from the configuration
+            __type_casbin_adapter = config.get("auth").get("casbin_adapter", "file")
+            _casbin_adapter_class = auth.get_adapter_module(__type_casbin_adapter)
+            _adapter_uri = config.get("auth").get("adapter_uri")
+            # Raise an error if the adapter is not supported
             if not _casbin_adapter_class:
-                raise RuntimeError(_( "Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
-            
-    
+                raise RuntimeError(_("Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
+    # Check for database migrations
     check_db_migrate()
-
+    # Initialize the authentication system if the adapter class and URI are present
     if _casbin_adapter_class and _adapter_uri:
-        _adapter_uri = os.path.abspath(os.path.join(ROOT_PATH,_adapter_uri))
-        _log.info(_("init casbin auth system..."))
-        application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
+        _adapter_uri = os.path.abspath(os.path.join(ROOT_PATH, _adapter_uri))
+    _log.info(_("init casbin auth system..."))
+    application.authObj = __init_auth(application, auth_type, _casbin_adapter_class, _adapter_uri)
     _log.info(_("load irails apps finished."))
     return application
 # import subprocess
 # import time
 # # 定义启动和停止进程的方法
 # def start_uvicon():
 #     cmd = 'uvicorn main:app --host 0.0.0.0 --port 8000'
```

### Comparing `irails-1.3.15/irails/database.py` & `irails-1.3.16/irails/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,51 @@
 from sqlalchemy.ext.automap import automap_base
 
 from ._utils import camelize_classname,pluralize_collection
  
 from alembic import command
 from alembic.config import Config
 import configparser
-import re,os
+import re,os,sys
 from typing import Union
 from .log import _log
+from ._i18n import _,load_app_translations
 DataMap = None
 mapped_base = None
 engine:Engine=None 
 class Base(DeclarativeBase):
     pass
 
  
+class _serviceMeta(type):
+    def __new__(cls, name, bases, attrs):
+        module_name = attrs['__module__']
+        module = sys.modules[module_name]
+        module_package = module.__package__
+        
+                
+        print(f"Creating class {name} in module {module_name}")
+        obj = super().__new__(cls, name, bases, attrs)
+        if module_package:
+            package_module = sys.modules[module_package]
+            service_package_path =  package_module.__path__[0]
+            app_dirs = service_package_path.split(os.sep)
+            if len(app_dirs)>2:
+                app_dirs = app_dirs[-2:]
+                setattr(obj,"__appdir__",".".join(app_dirs))
+                app_dir = os.path.dirname(service_package_path)
+                t = load_app_translations(app_dir)
+                setattr(obj,"_",t)
+        return obj
 
-class Service():
+class Service(metaclass=_serviceMeta):
     __all_generated = {}
     engine:Engine = engine
+    _ = _
+    
     @classmethod
     def session(self):
         if hasattr(self,"_session"):
             return self._session
         if hasattr(self,'_session_local'):
             session_local = getattr(self,'_session_local')
         else:
@@ -98,20 +121,20 @@
             cls.__all_generated[table_name] = tbItem
             return tbItem
         else:
             raise NameError()
 
 
             
-def ismongo_cloud(uri):
-    import re 
-    # uri = 'mongodb+srv://dbbruce:smjk123@atlascluster.siz4vrp.mongodb.net/?retryWrites=true&w=majority' 
-    # 匹配 MongoDB Cloud 连接字符串的正则表达式
-    regex = re.compile("mongodb\+srv:\/\/.*@.*\.mongodb\.net\/.*\?.*") 
-    return regex.match(uri)
+# def ismongo_cloud(uri):
+#     import re 
+#     # uri = 'mongodb+srv://dbbruce:smjk123@atlascluster.siz4vrp.mongodb.net/?retryWrites=true&w=majority' 
+#     # 匹配 MongoDB Cloud 连接字符串的正则表达式
+#     regex = re.compile("mongodb\+srv:\/\/.*@.*\.mongodb\.net\/.*\?.*") 
+#     return regex.match(uri)
       
 
 def sanitize_path(path):
     # 匹配非法字符
     illegal_chars = r'[\\/:\*\?"<>\|]'
     # 将非法字符替换为下划线
     sanitized_path = re.sub(illegal_chars, '_', path)
@@ -161,15 +184,15 @@
     global DataMap,mapped_base ,engine
     dbencode = cfg.get('dbencode')
     dbdecode = cfg.get('dbdecode')
     if uri.startswith('sqlite'):
         db_directory = os.path.dirname(uri.split(':///')[1])
         os.makedirs(db_directory, exist_ok=True) 
 
-    engine = create_engine(uri,  echo=debug)
+    engine = create_engine(uri,  echo=False)
     dbfirst = cfg.get("dbfirst")
     maptables = cfg.get("maptables")
     
     if not dbfirst :
         pass
     elif dbfirst: 
         def convert_varchar(s):
```

### Comparing `irails-1.3.15/irails/log.py` & `irails-1.3.16/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/midware.py` & `irails-1.3.16/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/midware_casbin.py` & `irails-1.3.16/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/midware_session.py` & `irails-1.3.16/irails/midware_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import sys
 import typing,uuid
 from typing import Dict
 from base64 import b64decode, b64encode
-
+from ._i18n import _
 import itsdangerous
 from itsdangerous.exc import BadSignature
 
 from starlette.datastructures import MutableHeaders, Secret
 from starlette.requests import HTTPConnection
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 from .log import _log
@@ -116,22 +116,15 @@
             self.redis_client.delete(session_id)
 except(ImportError):
     class RedisStorage(SessionStorage):
         def __init__(self, k: str = "") -> None:
             raise ImportError("redis seen is not installed,please use `pip install redis` to install it.")
     pass
 
-# _KT = typing.TypeVar("_KT")
-# _VT = typing.TypeVar("_VT")
-# class sessionDict(dict):
-#     def __getitem__(self, __key: _KT) -> _VT:
-#         if __key in self:
-#             return super().__getitem__(__key)
-#         else:
-#             return None
+ 
 class SessionMiddleware:
     def __init__(
         self,
         app: ASGIApp,
         
         secret_key: typing.Union[str, Secret],
         storage:SessionStorage = None,
```

### Comparing `irails-1.3.15/irails/mvc_router.py` & `irails-1.3.16/irails/mvc_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Type,TYPE_CHECKING, Any, Callable, get_type_hints 
 from fastapi import FastAPI,APIRouter  
 from .controller_utils import (TEMPLATE_PATH_KEY, VER_KEY, ControllerBase,
                                _get_leaf_controllers,
                                _register_controller_to_router, _route_method)
 
  
-import inspect
- 
+from ._i18n import _
+
 class InferringRouter(APIRouter):
     """
     Overrides the route decorator logic to use the annotated return type as the `response_model` if unspecified.
     """
     pass
     # if not TYPE_CHECKING:  # pragma: no branch
 
@@ -85,15 +85,15 @@
     def http(path,methods=['GET'],*args,**kwargs):
         return _route_method(path,method=methods,*args,**kwargs)
     @staticmethod
     def get(path: str, *args, **kwargs): 
         """if path eq application._public_auth_url,the auth agr must set to 'none' """
         if MvcRouter.app and path == MvcRouter.app.public_auth_url:
             if 'auth' in kwargs and kwargs['auth']!='none':
-                raise RuntimeError('the public auth path must set to "none" on auth arguments') 
+                raise RuntimeError(_('the public auth path must set to "none" on auth arguments')) 
             elif not 'auth' in kwargs:
                  kwargs['auth'] = 'none'
         return _route_method(path, "get", *args, **kwargs)
 
     @staticmethod
     def post(path: str, *args, **kwargs): 
         return _route_method(path, "post", *args, **kwargs)
```

### Comparing `irails-1.3.15/irails/scripts/_app.py` & `irails-1.3.16/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_controller.py` & `irails-1.3.16/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_i18n.py` & `irails-1.3.16/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_model.py` & `irails-1.3.16/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_project.py` & `irails-1.3.16/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_run.py` & `irails-1.3.16/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_shell.py` & `irails-1.3.16/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/_test.py` & `irails-1.3.16/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/main.py` & `irails-1.3.16/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.16/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/app/home.tpl` & `irails-1.3.16/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/app/model.jinja` & `irails-1.3.16/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/app/service.jinja` & `irails-1.3.16/irails/scripts/tpls/app/service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.16/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.16/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.16/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.16/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.16/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.16/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.16/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.16/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.16/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.16/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/unit_test.py` & `irails-1.3.16/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.15/irails/view.py` & `irails-1.3.16/irails/view.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,89 @@
 import os
 from typing import Any, Mapping
-from fastapi import BackgroundTasks, Request,Response
+from fastapi import BackgroundTasks, Request, Response
 from fastapi.templating import Jinja2Templates
 from fastapi.exceptions import HTTPException
 import jinja2
- 
-from .config import ROOT_PATH,config 
+
+from .config import ROOT_PATH, config
 from .log import _log
-env_configs = {} 
+from ._i18n import _
+env_configs = {}
 static_format = []
+
+
 def __get_view_configure():
-    global static_format,env_configs
-    env_options = config.get("view")# {'variable_start_string':'${','variable_end_string':'}'}
+    global static_format, env_configs
+    # {'variable_start_string':'${','variable_end_string':'}'}
+    env_options = config.get("view")
     if env_options:
-        static_format = env_options.get('static_format',[])
+        static_format = env_options.get('static_format', [])
         env_options = env_options.get("jinja2")
         env_configs = env_options.config
-     
+
 
 __get_view_configure()
 
+
 class _View(object):
-    def __init__(self,request,response=None, tmpl_path:str=f"{os.path.abspath('')}/app/views"):
+    def __init__(self, request, response=None, tmpl_path: str = f"{os.path.abspath('')}/app/views"):
         self._views_directory = tmpl_path
-        
-        self._templates = Jinja2Templates(directory=self.views_directory,**env_configs)
+
+        self._templates = Jinja2Templates(
+            directory=self.views_directory, **env_configs)
         self.request = request
         self.response = response
-       
+
     @property
     def templates(self):
         return self._templates
 
     @property
     def views_directory(self):
         return self._views_directory
-    
+
     @views_directory.setter
     def views_directory(self, views_directory: str):
         self._views_directory = views_directory
         self._templates = Jinja2Templates(directory=self.views_directory)
 
-    
-
-    def __call__(self, view_path: str="", context: dict={} ,**kwargs):
+    def __call__(self, view_path: str = "", context: dict = {}, **kwargs):
         request = self.request
         if not request or not isinstance(request, Request):
-            raise ValueError("request instance type must be fastapi.Request") 
+            raise ValueError(
+                _("request instance type must be fastapi.Request"))
 
         if not view_path.endswith(".html"):
             view_path = f"{view_path}.html"
 
         context["request"] = request
-        view_path_real = os.path.join(self.views_directory,view_path).replace(ROOT_PATH,"").replace("\\","/")
+        view_path_real = os.path.join(self.views_directory, view_path).replace(
+            ROOT_PATH, "").replace("\\", "/")
         try:
-            res = self._templates.TemplateResponse(view_path, context,**kwargs)
+            res = self._templates.TemplateResponse(
+                view_path, context, **kwargs)
             return res
         except jinja2.exceptions.TemplateSyntaxError as e:
             source = e.source.split('\n')[e.lineno-1:e.lineno]
-            info = f"TemplateSyntaxError on {view_path_real}:line:{e.lineno},{source}"
+            info = _("TemplateSyntaxError on %s :line:%s ,%s") % (
+                view_path_real, e.lineno, source)
             _log.error(info)
-            raise HTTPException(500,info)
+            raise HTTPException(500, info)
         except jinja2.exceptions.TemplateNotFound as e:
             source = e.args[0]
-            info = f"{view_path_real} raised TemplatesNotFound Error: `{source}`"
+            info = _("%s raised TemplatesNotFound Error: `%s`") % (
+                view_path_real, source)
             _log.error(info)
-            raise HTTPException(500,info)
+            raise HTTPException(500, info)
         except jinja2.exceptions.UndefinedError as e:
-            info =f"Tempate {view_path_real} raised Exception {e.args}"
+            info = _("Tempate %s raised Exception %s") % (
+                view_path_real, e.args)
             _log.error(info)
-            
-            raise HTTPException(500,info)
+
+            raise HTTPException(500, info)
         except Exception as e:
-            info =f"Tempate {view_path_real} raised Exception {e.args}"
+            info = _("Tempate %s raised Exception %s") % (
+                view_path_real, e.args)
             _log.error(info)
-            
-            raise HTTPException(500,info)
-        
-         
+
+            raise HTTPException(500, info)
```

### Comparing `irails-1.3.15/irails.egg-info/PKG-INFO` & `irails-1.3.16/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.15
+Version: 1.3.16
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.15/irails.egg-info/SOURCES.txt` & `irails-1.3.16/irails.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,24 @@
 irails/scripts/tpls/project/configs/cache.yaml
 irails/scripts/tpls/project/configs/casbin-adapter.csv
 irails/scripts/tpls/project/configs/casbin-model.conf
 irails/scripts/tpls/project/configs/database.yaml
 irails/scripts/tpls/project/configs/general.yaml
 irails/scripts/tpls/project/configs/session.yaml
 irails/scripts/tpls/project/configs/upload.yaml
+irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
 irails/scripts/tpls/project/data/alembic/README
 irails/scripts/tpls/project/data/alembic/env.py
 irails/scripts/tpls/project/data/alembic/script.py.mako
 irails/scripts/tpls/project/public/error_404.html
 irails/scripts/tpls/project/public/error_500.html
 irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
 irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
```

### Comparing `irails-1.3.15/setup.py` & `irails-1.3.16/setup.py`

 * *Files identical despite different names*

