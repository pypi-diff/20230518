# Comparing `tmp/dockx_checker-0.0.1.tar.gz` & `tmp/dockx_checker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockx_checker-0.0.1.tar", last modified: Wed May 17 10:10:41 2023, max compression
+gzip compressed data, was "dockx_checker-0.0.2.tar", last modified: Thu May 18 01:13:54 2023, max compression
```

## Comparing `dockx_checker-0.0.1.tar` & `dockx_checker-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.089684 dockx_checker-0.0.1/
--rw-r--r--   0 mroy       (501) staff       (20)       37 2023-05-17 08:13:26.000000 dockx_checker-0.0.1/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      196 2023-05-17 10:10:41.089555 dockx_checker-0.0.1/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)       79 2023-05-17 01:32:47.000000 dockx_checker-0.0.1/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.076803 dockx_checker-0.0.1/dockx_checker.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      196 2023-05-17 10:10:40.000000 dockx_checker-0.0.1/dockx_checker.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     3081 2023-05-17 10:10:41.000000 dockx_checker-0.0.1/dockx_checker.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-17 10:10:40.000000 dockx_checker-0.0.1/dockx_checker.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       68 2023-05-17 10:10:40.000000 dockx_checker-0.0.1/dockx_checker.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-17 03:17:54.000000 dockx_checker-0.0.1/dockx_checker.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)       32 2023-05-17 10:10:40.000000 dockx_checker-0.0.1/dockx_checker.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       18 2023-05-17 10:10:41.000000 dockx_checker-0.0.1/dockx_checker.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.077093 dockx_checker-0.0.1/dockx_checker_src/
--rw-r--r--   0 mroy       (501) staff       (20)        0 2023-05-17 01:32:47.000000 dockx_checker-0.0.1/dockx_checker_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)      437 2023-05-17 03:18:37.000000 dockx_checker-0.0.1/dockx_checker_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     2940 2023-05-17 09:59:13.000000 dockx_checker-0.0.1/dockx_checker_src/service.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.077200 dockx_checker-0.0.1/dockx_checker_src/static/
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.084429 dockx_checker-0.0.1/dockx_checker_src/static/css/
--rw-r--r--   0 mroy       (501) staff       (20)    71861 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.css
--rw-r--r--   0 mroy       (501) staff       (20)   210357 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    53265 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.min.css
--rw-r--r--   0 mroy       (501) staff       (20)   131395 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    71935 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 mroy       (501) staff       (20)   210361 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    53340 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 mroy       (501) staff       (20)   131472 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)     7965 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.css
--rw-r--r--   0 mroy       (501) staff       (20)   110875 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 mroy       (501) staff       (20)     6490 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 mroy       (501) staff       (20)    40331 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)     7958 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 mroy       (501) staff       (20)   110888 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 mroy       (501) staff       (20)     6562 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 mroy       (501) staff       (20)    48693 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    76347 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.css
--rw-r--r--   0 mroy       (501) staff       (20)   212450 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    58266 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 mroy       (501) staff       (20)   131956 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    76214 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 mroy       (501) staff       (20)   212393 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 mroy       (501) staff       (20)    58194 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 mroy       (501) staff       (20)   131791 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)   237950 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.css
--rw-r--r--   0 mroy       (501) staff       (20)   608300 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.css.map
--rw-r--r--   0 mroy       (501) staff       (20)   194901 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.min.css
--rw-r--r--   0 mroy       (501) staff       (20)   522639 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.min.css.map
--rw-r--r--   0 mroy       (501) staff       (20)   237528 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.css
--rw-r--r--   0 mroy       (501) staff       (20)   608144 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 mroy       (501) staff       (20)   195007 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 mroy       (501) staff       (20)   767483 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.min.css.map
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.084910 dockx_checker-0.0.1/dockx_checker_src/static/downloads/
--rw-r--r--   0 mroy       (501) staff       (20)        2 2023-05-17 09:08:41.000000 dockx_checker-0.0.1/dockx_checker_src/static/downloads/test.txt
--rw-r--r--   0 mroy       (501) staff       (20)       32 2023-05-17 08:17:16.000000 dockx_checker-0.0.1/dockx_checker_src/static/index.css
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.089230 dockx_checker-0.0.1/dockx_checker_src/static/js/
--rw-r--r--   0 mroy       (501) staff       (20)   207989 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.js
--rw-r--r--   0 mroy       (501) staff       (20)   451770 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 mroy       (501) staff       (20)    80420 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 mroy       (501) staff       (20)   333078 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 mroy       (501) staff       (20)   136215 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.js
--rw-r--r--   0 mroy       (501) staff       (20)   308207 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.js.map
--rw-r--r--   0 mroy       (501) staff       (20)    73978 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.min.js
--rw-r--r--   0 mroy       (501) staff       (20)   221179 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 mroy       (501) staff       (20)   145543 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.js
--rw-r--r--   0 mroy       (501) staff       (20)   309348 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.js.map
--rw-r--r--   0 mroy       (501) staff       (20)    60404 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.min.js
--rw-r--r--   0 mroy       (501) staff       (20)   216913 2023-05-17 02:07:43.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.min.js.map
--rw-r--r--   0 mroy       (501) staff       (20)   284996 2023-05-17 02:08:09.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.js
--rw-r--r--   0 mroy       (501) staff       (20)    87462 2023-05-17 02:08:09.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.min.js
--rw-r--r--   0 mroy       (501) staff       (20)   134714 2023-05-17 02:08:09.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.min.map
--rw-r--r--   0 mroy       (501) staff       (20)   231697 2023-05-17 02:08:09.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.slim.js
--rw-r--r--   0 mroy       (501) staff       (20)    70193 2023-05-17 02:08:09.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.slim.min.js
--rw-r--r--   0 mroy       (501) staff       (20)   107105 2023-05-17 02:08:09.000000 dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.slim.min.map
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-17 10:10:41.089384 dockx_checker-0.0.1/dockx_checker_src/templates/
--rw-r--r--   0 mroy       (501) staff       (20)     2440 2023-05-17 10:00:20.000000 dockx_checker-0.0.1/dockx_checker_src/templates/index.html
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-05-17 10:10:41.089722 dockx_checker-0.0.1/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)      488 2023-05-17 10:10:36.000000 dockx_checker-0.0.1/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.223960 dockx_checker-0.0.2/
+-rw-r--r--   0 mroy       (501) staff       (20)       37 2023-05-17 08:13:26.000000 dockx_checker-0.0.2/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      196 2023-05-18 01:13:54.223821 dockx_checker-0.0.2/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)       79 2023-05-17 01:32:47.000000 dockx_checker-0.0.2/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.204025 dockx_checker-0.0.2/dockx_checker.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      196 2023-05-18 01:13:53.000000 dockx_checker-0.0.2/dockx_checker.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     3081 2023-05-18 01:13:54.000000 dockx_checker-0.0.2/dockx_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-18 01:13:53.000000 dockx_checker-0.0.2/dockx_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       68 2023-05-18 01:13:54.000000 dockx_checker-0.0.2/dockx_checker.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-17 03:17:54.000000 dockx_checker-0.0.2/dockx_checker.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)       32 2023-05-18 01:13:54.000000 dockx_checker-0.0.2/dockx_checker.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       18 2023-05-18 01:13:54.000000 dockx_checker-0.0.2/dockx_checker.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.204331 dockx_checker-0.0.2/dockx_checker_src/
+-rw-r--r--   0 mroy       (501) staff       (20)        0 2023-05-17 01:32:47.000000 dockx_checker-0.0.2/dockx_checker_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)      437 2023-05-17 03:18:37.000000 dockx_checker-0.0.2/dockx_checker_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2956 2023-05-18 01:13:39.000000 dockx_checker-0.0.2/dockx_checker_src/service.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.204431 dockx_checker-0.0.2/dockx_checker_src/static/
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.213759 dockx_checker-0.0.2/dockx_checker_src/static/css/
+-rw-r--r--   0 mroy       (501) staff       (20)    71861 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.css
+-rw-r--r--   0 mroy       (501) staff       (20)   210357 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    53265 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)   131395 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    71935 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 mroy       (501) staff       (20)   210361 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    53340 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)   131472 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)     7965 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.css
+-rw-r--r--   0 mroy       (501) staff       (20)   110875 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)     6490 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)    40331 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)     7958 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 mroy       (501) staff       (20)   110888 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)     6562 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)    48693 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    76347 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.css
+-rw-r--r--   0 mroy       (501) staff       (20)   212450 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    58266 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)   131956 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    76214 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 mroy       (501) staff       (20)   212393 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)    58194 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)   131791 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)   237950 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.css
+-rw-r--r--   0 mroy       (501) staff       (20)   608300 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)   194901 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)   522639 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.min.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)   237528 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.css
+-rw-r--r--   0 mroy       (501) staff       (20)   608144 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 mroy       (501) staff       (20)   195007 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 mroy       (501) staff       (20)   767483 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.min.css.map
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.214233 dockx_checker-0.0.2/dockx_checker_src/static/downloads/
+-rw-r--r--   0 mroy       (501) staff       (20)        2 2023-05-17 09:08:41.000000 dockx_checker-0.0.2/dockx_checker_src/static/downloads/test.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       32 2023-05-17 08:17:16.000000 dockx_checker-0.0.2/dockx_checker_src/static/index.css
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.223304 dockx_checker-0.0.2/dockx_checker_src/static/js/
+-rw-r--r--   0 mroy       (501) staff       (20)   207989 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.js
+-rw-r--r--   0 mroy       (501) staff       (20)   451770 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 mroy       (501) staff       (20)    80420 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 mroy       (501) staff       (20)   333078 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 mroy       (501) staff       (20)   136215 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.js
+-rw-r--r--   0 mroy       (501) staff       (20)   308207 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 mroy       (501) staff       (20)    73978 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 mroy       (501) staff       (20)   221179 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 mroy       (501) staff       (20)   145543 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.js
+-rw-r--r--   0 mroy       (501) staff       (20)   309348 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.js.map
+-rw-r--r--   0 mroy       (501) staff       (20)    60404 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.min.js
+-rw-r--r--   0 mroy       (501) staff       (20)   216913 2023-05-17 02:07:43.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.min.js.map
+-rw-r--r--   0 mroy       (501) staff       (20)   284996 2023-05-17 02:08:09.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.js
+-rw-r--r--   0 mroy       (501) staff       (20)    87462 2023-05-17 02:08:09.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.min.js
+-rw-r--r--   0 mroy       (501) staff       (20)   134714 2023-05-17 02:08:09.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.min.map
+-rw-r--r--   0 mroy       (501) staff       (20)   231697 2023-05-17 02:08:09.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.slim.js
+-rw-r--r--   0 mroy       (501) staff       (20)    70193 2023-05-17 02:08:09.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.slim.min.js
+-rw-r--r--   0 mroy       (501) staff       (20)   107105 2023-05-17 02:08:09.000000 dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.slim.min.map
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-05-18 01:13:54.223488 dockx_checker-0.0.2/dockx_checker_src/templates/
+-rw-r--r--   0 mroy       (501) staff       (20)     2440 2023-05-17 10:00:20.000000 dockx_checker-0.0.2/dockx_checker_src/templates/index.html
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-05-18 01:13:54.224003 dockx_checker-0.0.2/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)      488 2023-05-18 01:13:50.000000 dockx_checker-0.0.2/setup.py
```

### Comparing `dockx_checker-0.0.1/dockx_checker.egg-info/SOURCES.txt` & `dockx_checker-0.0.2/dockx_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/service.py` & `dockx_checker-0.0.2/dockx_checker_src/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from docx import Document
 STATIC_PATH = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static')
 app = Flask(__name__,)
 
 
 KEYS = {}
-with open(Path("~").expanduser()/"Desktop"/"hit.txt") as f:
+with open(Path("~").expanduser()/"Desktop"/"hit.txt", encoding="gbk") as f:
     for l in f:
         if l.strip() != "":
             k,v = l.strip().split(":")
             KEYS[k.strip()] = v.strip()
 
 def DealDocx(path):
     doc = Document(path)
```

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.min.css` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/css/bootstrap.rtl.min.css.map` & `dockx_checker-0.0.2/dockx_checker_src/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.js.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.min.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.bundle.min.js.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.js.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.min.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.esm.min.js.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.js.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.min.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/bootstrap.min.js.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.min.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.min.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.min.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.slim.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.slim.min.js` & `dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/static/js/jquery.slim.min.map` & `dockx_checker-0.0.2/dockx_checker_src/static/js/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `dockx_checker-0.0.1/dockx_checker_src/templates/index.html` & `dockx_checker-0.0.2/dockx_checker_src/templates/index.html`

 * *Files identical despite different names*

