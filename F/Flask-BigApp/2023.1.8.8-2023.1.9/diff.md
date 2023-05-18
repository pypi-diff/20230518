# Comparing `tmp/Flask-BigApp-2023.1.8.8.tar.gz` & `tmp/Flask-BigApp-2023.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-BigApp-2023.1.8.8.tar", last modified: Wed May  3 21:05:16 2023, max compression
+gzip compressed data, was "Flask-BigApp-2023.1.9.tar", last modified: Thu May 18 10:34:32 2023, max compression
```

## Comparing `Flask-BigApp-2023.1.8.8.tar` & `Flask-BigApp-2023.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/
--rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.8.8/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.8.8/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      554 2023-04-01 10:35:56.000000 Flask-BigApp-2023.1.8.8/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.8.8/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)      174 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-05-03 21:02:22.000000 Flask-BigApp-2023.1.8.8/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.237607 Flask-BigApp-2023.1.8.8/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.237607 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-05-03 21:05:16.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1851 2023-05-03 21:05:16.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-03 21:05:16.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       54 2023-05-03 21:05:16.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1000) david     (1000)      101 2023-05-03 21:05:16.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-05-03 21:05:16.000000 Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp/
--rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    11896 2023-04-16 20:47:54.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/bigapp.py
--rw-rw-r--   0 david     (1000) david     (1000)     6465 2023-03-31 22:32:21.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/blueprint.py
--rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)      916 2023-03-31 22:01:28.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/objects.py
--rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-05-03 21:04:51.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/orm.py
--rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/resources.py
--rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-04-09 22:17:36.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/security.py
--rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp/utilities.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.237607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
--rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.237607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
--rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
--rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
--rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.237607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.237607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
--rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
--rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
--rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
--rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
--rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
--rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
--rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
--rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
--rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/resources.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 21:05:16.241607 Flask-BigApp-2023.1.8.8/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     1792 2023-04-10 18:58:43.000000 Flask-BigApp-2023.1.8.8/tests/test_group.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/
+-rw-rw-r--   0 david     (1000) david     (1000)    25342 2022-11-24 21:56:54.000000 Flask-BigApp-2023.1.9/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)       60 2023-01-08 16:44:01.000000 Flask-BigApp-2023.1.9/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1844 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      699 2023-05-04 14:17:25.000000 Flask-BigApp-2023.1.9/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      271 2023-04-10 18:03:50.000000 Flask-BigApp-2023.1.9/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)      174 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1629 2023-05-18 10:31:56.000000 Flask-BigApp-2023.1.9/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1844 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1855 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       54 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-08 17:03:33.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1000) david     (1000)      101 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-05-18 10:34:32.000000 Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp/
+-rw-rw-r--   0 david     (1000) david     (1000)      305 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10308 2023-04-05 11:13:29.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/auth.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11282 2023-05-18 10:29:58.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/bigapp.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6229 2023-05-18 10:09:34.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/blueprint.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4958 2023-04-01 16:09:06.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5845 2023-05-03 21:04:51.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/orm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      788 2023-05-18 10:27:54.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/registeries.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1659 2023-04-01 10:10:00.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/resources.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7663 2023-04-09 22:17:36.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/security.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3093 2023-03-31 22:23:19.000000 Flask-BigApp-2023.1.9/src/flask_bigapp/utilities.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/
+-rw-rw-r--   0 david     (1000) david     (1000)      360 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/css/
+-rw-rw-r--   0 david     (1000) david     (1000)       45 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/css/example__css.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/img/
+-rw-rw-r--   0 david     (1000) david     (1000)    28469 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/js/example__js.js
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.732208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/
+-rw-rw-r--   0 david     (1000) david     (1000)      268 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/400.html
+-rw-rw-r--   0 david     (1000) david     (1000)      315 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/401.html
+-rw-rw-r--   0 david     (1000) david     (1000)      261 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/403.html
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/404.html
+-rw-rw-r--   0 david     (1000) david     (1000)      302 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/405.html
+-rw-rw-r--   0 david     (1000) david     (1000)      278 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/errors/500.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/
+-rw-rw-r--   0 david     (1000) david     (1000)      766 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/
+-rw-rw-r--   0 david     (1000) david     (1000)       13 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/footer.html
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/includes/menu.html
+-rw-rw-r--   0 david     (1000) david     (1000)     9883 2023-04-01 00:04:55.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)      992 2023-02-11 11:08:32.000000 Flask-BigApp-2023.1.9/src/flask_bigapp_cli/resources.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-18 10:34:32.736208 Flask-BigApp-2023.1.9/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2462 2023-05-18 10:22:21.000000 Flask-BigApp-2023.1.9/tests/test_group.py
```

### Comparing `Flask-BigApp-2023.1.8.8/LICENSE` & `Flask-BigApp-2023.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/PKG-INFO` & `Flask-BigApp-2023.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.8.8
+Version: 2023.1.9
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,7 +35,11 @@
 
 **What is Flask-BigApp?**
 
 Flask-BigApp's main purpose is to help simplify the importing of blueprints, routes and models.
 It has a few extra features built in to help with theming, securing pages and password authentication.
 
 [Go to Wiki](https://github.com/CheeseCake87/Flask-BigApp/wiki)
+
+If you'd like to jump stright in, here's a working example porject:
+
+[TemPro-Flask-BigApp](https://github.com/Flask-Planet/TemPro-Flask-BigApp)
```

### Comparing `Flask-BigApp-2023.1.8.8/setup.py` & `Flask-BigApp-2023.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup, find_packages
 
 readme = pathlib.Path(pathlib.Path.cwd() / "README.md").read_text()
 
 setup(
     name='Flask-BigApp',
-    version=f'2023.1.8.8',
+    version=f'2023.1.9',
     url='https://github.com/Flask-Planet/Flask-BigApp',
     license='GNU Lesser General Public License v2.1',
     author='David Carmichael',
     author_email='carmichaelits@gmail.com',
     description='A Flask auto importer that allows your Flask apps to grow big.',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
```

### Comparing `Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/PKG-INFO` & `Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-BigApp
-Version: 2023.1.8.8
+Version: 2023.1.9
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Home-page: https://github.com/Flask-Planet/Flask-BigApp
 Author: David Carmichael
 Author-email: carmichaelits@gmail.com
 License: GNU Lesser General Public License v2.1
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,7 +35,11 @@
 
 **What is Flask-BigApp?**
 
 Flask-BigApp's main purpose is to help simplify the importing of blueprints, routes and models.
 It has a few extra features built in to help with theming, securing pages and password authentication.
 
 [Go to Wiki](https://github.com/CheeseCake87/Flask-BigApp/wiki)
+
+If you'd like to jump stright in, here's a working example porject:
+
+[TemPro-Flask-BigApp](https://github.com/Flask-Planet/TemPro-Flask-BigApp)
```

### Comparing `Flask-BigApp-2023.1.8.8/src/Flask_BigApp.egg-info/SOURCES.txt` & `Flask-BigApp-2023.1.9/src/Flask_BigApp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 src/Flask_BigApp.egg-info/requires.txt
 src/Flask_BigApp.egg-info/top_level.txt
 src/flask_bigapp/__init__.py
 src/flask_bigapp/auth.py
 src/flask_bigapp/bigapp.py
 src/flask_bigapp/blueprint.py
 src/flask_bigapp/helpers.py
-src/flask_bigapp/objects.py
 src/flask_bigapp/orm.py
+src/flask_bigapp/registeries.py
 src/flask_bigapp/resources.py
 src/flask_bigapp/security.py
 src/flask_bigapp/utilities.py
 src/flask_bigapp_cli/__init__.py
 src/flask_bigapp_cli/cli.py
 src/flask_bigapp_cli/resources.py
 src/flask_bigapp_cli/__temp_theme_dir__/builtins/context_processors.py
```

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/auth.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/auth.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/bigapp.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/bigapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import logging
 import os
 from importlib import import_module
 from inspect import getmembers
 from inspect import isclass
 from pathlib import Path
-from types import ModuleType
 from typing import Dict, Union, Optional, Any
 
 from flask import Blueprint
 from flask import Flask
 from flask import session
 from flask_sqlalchemy.model import DefaultMeta
 from toml import load as toml_load
 
 from .blueprint import BigAppBlueprint
 from .helpers import init_app_config
-from .objects import ModelRegistry
+from .registeries import ModelRegistry
 from .resources import Resources
 from .utilities import cast_to_bool, cast_to_import_str, deprecated
 
 
 class BigApp(object):
     _app: Flask
     _app_name: str
     _app_path: Path
     _app_folder: Path
 
-    __blueprint_registry__: Dict[str, Optional[ModuleType]]
     __model_registry__: ModelRegistry
 
     config_path: Path
     config: Dict
     themes: Dict[str, Path]
 
     def __init__(
@@ -72,15 +70,14 @@
 
         self._app = app
         self._app_name = app.name
         self._app_path = Path(self._app.root_path)
         self._app_folder = self._app_path.parent
 
         self.__model_registry__ = ModelRegistry()
-        self.__blueprint_registry__ = dict()
 
         self.config_path = self._app_path / app_config_file
         self.config = init_app_config(self.config_path, self._app)
         self.themes = dict()
 
     def init_session(self) -> None:
         """
@@ -100,14 +97,15 @@
             builtins_folder = Path(self._app_path / folder)
         else:
             builtins_folder = folder
 
         if builtins_folder.is_dir():
             with self._app.app_context():
                 for py_file in builtins_folder.glob("*.py"):
+                    print(f"{cast_to_import_str(self._app_name, builtins_folder)}.{py_file.stem}")
                     module = import_module(
                         f"{cast_to_import_str(self._app_name, builtins_folder)}.{py_file.stem}")
                     if hasattr(module, "loader"):
                         module.loader(self._app)
 
     def import_blueprints(self, folder: str) -> None:
         """
@@ -129,29 +127,20 @@
         """
         if isinstance(blueprint, str):
             potential_bp = Path(self._app_path / blueprint)
         else:
             potential_bp = blueprint
 
         if potential_bp.is_dir():
-            if potential_bp.name in self.__blueprint_registry__:
-                raise ImportError(
-                    f"Blueprint {potential_bp.name} is already registered, blueprint folders must be unique\n"
-                    f"Importing from {potential_bp}"
-                )
             try:
-                module = import_module(
-                    cast_to_import_str(self._app_name, potential_bp))
+                module = import_module(cast_to_import_str(self._app_name, potential_bp))
                 for dir_item in dir(module):
                     _ = getattr(module, dir_item)
                     if isinstance(_, BigAppBlueprint):
                         if _.enabled:
-                            self.__blueprint_registry__.update(
-                                {potential_bp.name: module}
-                            )
                             self._app.register_blueprint(_)
                         break
             except Exception as e:
                 logging.critical(f"{e}",
                                  f"Error importing blueprint: from {potential_bp}")
 
     def import_themes(self, themes_folder: str) -> None:
@@ -282,35 +271,32 @@
 
     def model(self, class_: str) -> DefaultMeta:
         """
         Returns the model class for the given ORM class name
         """
         return self.__model_registry__.class_(class_)
 
-    def model_meta(self, class_: Union[str, Any]) -> dict:
+    def model_meta(self, class_: Union[str, DefaultMeta]) -> dict:
         """
         Returns meta information for the given ORM class name
         """
 
         def check_for_table_name(model_):
             if not hasattr(model_, "__tablename__"):
                 raise AttributeError(f"{model_} is not a valid model")
 
         if isinstance(class_, str):
-            model = self.__model_registry__.get(class_)
-            check_for_table_name(model['class'])
+            model = self.__model_registry__.class_(class_)
+            check_for_table_name(model)
             return {
-                "ref": model['ref'],
-                "location": model['class'].__module__,
-                "table_name": model['class'].__tablename__,
+                "location": model.__module__,
+                "table_name": model.__tablename__,
             }
 
-        check_for_table_name(class_)
         return {
-            "ref": class_.__name__,
             "location": class_.__module__,
             "table_name": class_.__tablename__,
         }
 
     @deprecated("import_structures() will be removed, Use import_themes() instead")
     def import_structures(self, structures_folder: str) -> None:
         self.import_themes(structures_folder)
```

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/blueprint.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/blueprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import logging
 from importlib import import_module
 from importlib.util import find_spec
 from pathlib import Path
-from types import ModuleType
-from typing import Dict, Optional, Union
+from typing import Optional, Union, Protocol
 
 from flask import Blueprint
 from flask import session
 
-from flask_bigapp.helpers import init_bp_config
-from flask_bigapp.utilities import cast_to_import_str, deprecated
+from .helpers import init_bp_config
+from .utilities import cast_to_import_str, deprecated
+
+
+class BigApp(Protocol):
+    def import_models(
+            self,
+            from_file: Optional[Union[str, Path]] = None,
+            from_folder: Optional[Union[str, Path]] = None,
+    ) -> None:
+        ...
 
 
 class BigAppBlueprint(Blueprint):
     """
     Class that handles Blueprints from within the Blueprint __init__ from_file
     """
     enabled: bool = False
     location: Path
     bp_name: str
     package: str
     session: dict
     settings: dict
 
-    nested_blueprints: Dict[str, Optional[ModuleType]]
+    _bigapp_instance: BigApp
 
     def __init__(self, dunder_name, config_file: str = "config.toml"):
         """
         dunder_name must be __name__
         config_file must be relative to the location of the blueprint.
         """
         self.package = dunder_name
@@ -37,24 +45,36 @@
 
         if spec is None:
             raise ImportError(f"Cannot find origin of {self.package}")
 
         self.location = Path(f"{spec.origin}").parent
         self.bp_name = self.location.name
 
-        self.nested_blueprints = {}
-
         self.enabled, self.session, self.settings = init_bp_config(self.bp_name, self.location / config_file)
 
         if self.enabled:
             super().__init__(
                 self.bp_name,
                 self.package,
                 **self.settings
             )
+            self._bigapp_instance = self.set_bigapp_instance()
+
+    def set_bigapp_instance(self):
+        def get_bigapp_instance() -> BigApp:
+            from flask_bigapp import BigApp
+
+            app_module = import_module(self.app_name)
+            for dir_item in dir(app_module):
+                potential_instance = getattr(app_module, dir_item)
+                if isinstance(potential_instance, BigApp):
+                    return potential_instance
+            raise ImportError(f"Cannot find BigApp instance in {self.app_name}")
+
+        return get_bigapp_instance()
 
     def import_routes(self, folder: str = "routes") -> None:
         """
         Imports all the routes in the given from_folder.
         If no from_folder is specified defaults to a from_folder named 'routes'
 
         Folder must be relative ( from_folder="here" not from_folder="/home/user/app/from_folder/blueprint/from_folder" )
@@ -99,29 +119,21 @@
 
         if isinstance(blueprint, str):
             potential_bp = Path(self.location / blueprint)
         else:
             potential_bp = blueprint
 
         if potential_bp.is_dir():
-            if potential_bp.name in self.nested_blueprints:
-                raise ImportError(
-                    f"Nested blueprint {potential_bp.name} is already registered, blueprint folders must be unique\n"
-                    f"Importing from {potential_bp}"
-                )
             app_name = self.package.split(".")[0]
             try:
                 module = import_module(cast_to_import_str(app_name, potential_bp))
                 for dir_item in dir(module):
                     _ = getattr(module, dir_item)
                     if isinstance(_, BigAppBlueprint):
                         if _.enabled:
-                            self.nested_blueprints.update(
-                                {potential_bp.name: module}
-                            )
                             self.register_blueprint(_)
                         break
             except Exception as e:
                 logging.critical(f"{e}\n", f"Error importing blueprint: from {potential_bp}")
 
     def init_session(self) -> None:
         """
@@ -145,33 +157,21 @@
         Imports model files from a single from_file or a from_folder. Both are allowed to be set.
 
         File and Folder must be relative ( from_folder="here" not from_folder="/home/user/app/from_folder" )
         """
         if not self.enabled:
             return
 
-        from flask_bigapp import BigApp
-
-        def get_bigapp_instance() -> BigApp:
-            app_module = import_module(self.app_name)
-            for dir_item in dir(app_module):
-                potential_instance = getattr(app_module, dir_item)
-                if isinstance(potential_instance, BigApp):
-                    return potential_instance
-            raise ImportError(f"Cannot find BigApp instance in {self.app_name}")
-
-        bigapp_instance = get_bigapp_instance()
-
         if isinstance(from_file, str):
             from_file = Path(self.location / from_file)
 
         if isinstance(from_folder, str):
             from_folder = Path(self.location / from_folder)
 
-        bigapp_instance.import_models(from_file, from_folder)
+        self._bigapp_instance.import_models(from_file, from_folder)
 
     def tmpl(self, template) -> str:
         """
         Pushes together the name of the blueprint and the template from_file to look for.
         This is a small-time saving method to allow you to only type
         bp.tmpl("index.html") when looking for template files.
         """
```

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/helpers.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/helpers.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/objects.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/registeries.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,30 +6,23 @@
 
 class ModelRegistry:
     registry: t.Dict[str, t.Any]
 
     def __init__(self):
         self.registry = dict()
 
-    def assert_exists(self, ref: str):
-        if ref not in self.registry:
+    def assert_exists(self, class_name: str):
+        if class_name not in self.registry:
             raise KeyError(
-                f"Model {ref} not found in model registry \n"
+                f"Model {class_name} not found in model registry \n"
                 f"Available models: {', '.join(self.registry.keys())}"
             )
 
-    def get(self, ref: str) -> dict:
-        self.assert_exists(ref)
-        return self.registry[ref]
-
-    def class_(self, ref: str) -> DefaultMeta:
-        self.assert_exists(ref)
-        return self.registry[ref]['class']
-
     def add(self, ref, model: t.Optional[ModuleType] = None):
-        self.registry[ref] = {
-            'ref': ref,
-            'class': model
-        }
+        self.registry[ref] = model
+
+    def class_(self, class_name: str) -> DefaultMeta:
+        self.assert_exists(class_name)
+        return self.registry[class_name]
 
     def __repr__(self):
         return f"ModelRegistry({self.registry})"
```

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/orm.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/orm.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/resources.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/security.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/security.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp/utilities.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp/utilities.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/builtins/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png` & `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/static/img/Flask-BigApp-Logo.png`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html` & `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/__temp_theme_dir__/templates/__temp_theme_dir__/extends/main.html`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/cli.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/src/flask_bigapp_cli/resources.py` & `Flask-BigApp-2023.1.9/src/flask_bigapp_cli/resources.py`

 * *Files identical despite different names*

### Comparing `Flask-BigApp-2023.1.8.8/tests/test_group.py` & `Flask-BigApp-2023.1.9/tests/test_group.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,38 @@
     """
     If this test is successful, the app is set up and running correctly.
     """
     response = client.get('/tests/')
     assert response.status_code == 200
 
 
+def test_nested_blueprint(client):
+    """
+    If this test is successful, the app is set up and running correctly.
+    """
+    response = client.get('/tests/nested_test/')
+    assert response.status_code == 200
+
+
+def test_group_nested_blueprint_one(client):
+    """
+    If this test is successful, the app is set up and running correctly.
+    """
+    response = client.get('/tests/nested_test_one/')
+    assert response.status_code == 200
+
+
+def test_group_nested_blueprint_two(client):
+    """
+    If this test is successful, the app is set up and running correctly.
+    """
+    response = client.get('/tests/nested_test_two/')
+    assert response.status_code == 200
+
+
 def test_error_404(client):
     """
     If this test is successful, the app is set up and running correctly.
     """
     response = client.get('/tests/error-page-404')
     assert b"No route associated with the URL" in response.data
```

