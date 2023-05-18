# Comparing `tmp/Flask-BigApp-2023.1.9.tar.gz` & `tmp/Flask-BigApp-2023.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.9.tar", last modified: Thu May 18 10:34:32 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.9.1.tar", last modified: Thu May 18 10:51:58 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.9.tar` & `Flask-BigApp-2023.1.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.9/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.9/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1844 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      699 2023-05-04 14:17:25.000000 Flask-BigApp-2023.1.9/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.9/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1629 2023-05-18 10:31:56.000000 Flask-BigApp-2023.1.9/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1844 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11282 2023-05-18 10:29:58.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-05-18 10:09:34.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-05-03 21:04:51.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/orm.py
--rw-rw-r--   0 david     (1000) david     (1000)      788 2023-05-18 10:27:54.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/registeries.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-04-09 22:17:36.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     2462 2023-05-18 10:22:21.000000 Flask-BigApp-2023.1.9/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.9.1/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.9.1/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      699 2023-05-04 14:17:25.000000 Flask-BigApp-2023.1.9.1/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.9.1/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1582 2023-05-18 10:49:36.000000 Flask-BigApp-2023.1.9.1/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1796 2023-05-18 10:51:58.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-05-18 10:51:58.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-18 10:51:58.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-05-18 10:51:58.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-05-18 10:51:58.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-05-18 10:51:58.000000 Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11282 2023-05-18 10:29:58.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-05-18 10:09:34.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-05-03 21:04:51.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      788 2023-05-18 10:27:54.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/registeries.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-04-09 22:17:36.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.837501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:51:58.841501 Flask-BigApp-2023.1.9.1/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2462 2023-05-18 10:22:21.000000 Flask-BigApp-2023.1.9.1/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.9/LICENSE` & `Flask-BigApp-2023.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/PKG-INFO` & `Flask-BigApp-2023.1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9
+Version: 2023.1.9.1
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
```

### Comparing `Flask-BigApp-2023.1.9/README.md` & `Flask-BigApp-2023.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/setup.py` & `Flask-BigApp-2023.1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.9',
+    version=f'2023.1.9.1',
     url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
     platforms='any',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment', 'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
         'Operating System :: OS Independent', 'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Natural Language :: English',
```

### Comparing `Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.9
+Version: 2023.1.9.1
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
```

### Comparing `Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.9.1/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/bigapp.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/blueprint.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/orm.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/orm.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/registeries.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/registeries.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/security.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp/utilities.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.9.1/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.9/tests/test_group.py` & `Flask-BigApp-2023.1.9.1/tests/test_group.py`

 * *Files identical despite different names*

