# Comparing `tmp/daliuge-translator-2.4.0.tar.gz` & `tmp/daliuge-translator-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daliuge-translator-2.4.0.tar", last modified: Sat Mar 11 06:01:20 2023, max compression
+gzip compressed data, was "daliuge-translator-3.0.0.tar", last modified: Thu May 18 12:49:51 2023, max compression
```

## Comparing `daliuge-translator-2.4.0.tar` & `daliuge-translator-3.0.0.tar`

### file list

```diff
@@ -1,253 +1,150 @@
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.467363 daliuge-translator-2.4.0/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1089 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/.coveragerc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      180 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/MANIFEST.in
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      326 2023-03-11 06:01:20.467363 daliuge-translator-2.4.0/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      157 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     2804 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/build_translator.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.435363 daliuge-translator-2.4.0/daliuge_translator.egg-info/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      326 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/daliuge_translator.egg-info/PKG-INFO
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9433 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/daliuge_translator.egg-info/SOURCES.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/daliuge_translator.egg-info/dependency_links.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       63 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/daliuge_translator.egg-info/entry_points.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      128 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/daliuge_translator.egg-info/requires.txt
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        9 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/daliuge_translator.egg-info/top_level.txt
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.435363 daliuge-translator-2.4.0/dlg/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.435363 daliuge-translator-2.4.0/dlg/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      338 2023-01-20 04:39:24.000000 daliuge-translator-2.4.0/dlg/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      338 2023-02-21 01:56:47.000000 daliuge-translator-2.4.0/dlg/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.435363 daliuge-translator-2.4.0/dlg/dropmake/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1055 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.439363 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      257 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      255 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      255 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12075 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/dm_utils.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12443 2023-03-03 00:15:51.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/dm_utils.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12149 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/dm_utils.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33214 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/lg.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33994 2023-02-01 11:13:24.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/lg.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    33878 2023-02-21 01:56:47.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/lg.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5103 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pg_generator.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5224 2023-03-03 00:15:51.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pg_generator.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5192 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pg_generator.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4295 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pg_manager.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4282 2022-12-02 06:13:10.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pg_manager.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4298 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pg_manager.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10593 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pgt.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10715 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pgt.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10671 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pgt.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15161 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pgtp.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15356 2023-02-01 11:13:24.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pgtp.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15177 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/pgtp.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35069 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/scheduler.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35225 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/scheduler.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35179 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/__pycache__/scheduler.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25512 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/dlg/dropmake/dm_utils.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16607 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/lg.graph.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    66804 2023-02-01 08:50:20.000000 daliuge-translator-2.4.0/dlg/dropmake/lg.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.439363 daliuge-translator-2.4.0/dlg/dropmake/lib/
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   382436 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/lib/libmetis.dylib
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   495581 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/lib/libmetis.so
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7713 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/dlg/dropmake/pg_generator.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5689 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/pg_manager.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17296 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/pgt.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25740 2023-02-01 08:50:20.000000 daliuge-translator-2.4.0/dlg/dropmake/pgtp.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    49735 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/scheduler.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.439363 daliuge-translator-2.4.0/dlg/dropmake/utils/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.439363 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      169 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8415 2023-02-19 06:22:54.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/anneal.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4435 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/antichains.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4434 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/antichains.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4428 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/antichains.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2429 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2717 2023-02-01 11:13:24.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2475 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/__pycache__/bash_parameter.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11713 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/anneal.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5848 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/antichains.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3470 2023-02-01 08:50:20.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/bash_parameter.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.439363 daliuge-translator-2.4.0/dlg/dropmake/utils/heft/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8068 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/utils/heft/base.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.443363 daliuge-translator-2.4.0/dlg/dropmake/web/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2023-01-11 06:33:17.000000 daliuge-translator-2.4.0/dlg/dropmake/web/LICENSE
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       47 2023-01-11 06:33:17.000000 daliuge-translator-2.4.0/dlg/dropmake/web/VERSION
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.443363 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      167 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18547 2022-11-03 13:04:49.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/lg_web.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25609 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25807 2022-12-09 01:48:25.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    25869 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/translator_rest.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4532 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4568 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4548 2022-12-21 05:50:12.000000 daliuge-translator-2.4.0/dlg/dropmake/web/__pycache__/translator_utils.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   139114 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/d3.v3.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11324 2023-02-01 08:50:20.000000 daliuge-translator-2.4.0/dlg/dropmake/web/graph_init.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.443363 daliuge-translator-2.4.0/dlg/dropmake/web/img/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14438 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/img/jsoneditor-icons.png
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      878 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/license.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    28292 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/main.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6377 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/matrix_vis.html
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)    15050 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/pg_viewer.html
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17286 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/pure-min.css
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.447363 daliuge-translator-2.4.0/dlg/dropmake/web/src/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5649 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/FileSaver.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.431363 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.447363 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    64548 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   151749 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48488 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   108539 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4897 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    76483 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4021 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    32461 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   192348 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   492048 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155758 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   625953 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.451363 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   222911 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   402249 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78635 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   311949 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   131637 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   250568 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    58072 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   190253 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.455363 daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/d3.v5.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/dagre-d3.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/dagre-d3.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      806 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/data_prep.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/echarts-dagre.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.455363 daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    69177 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   174048 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    79612 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    60840 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   165349 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/html2canvas.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.455363 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      177 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/arrow_right_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      409 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/explore_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/liu.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/liuFavIcon.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1462 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/settings_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26026 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/translate_green.png
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      423 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/zoom_in_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      370 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/zoom_out_map_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      404 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/zoom_out_white_24dp.svg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30747 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/jquery-ui.min.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89500 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/jquery.min.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17804 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/canteen.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1943 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/caseFrame.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12066 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/caseFrame.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7037 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/config.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7545 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/countup.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45411 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/dat.gui.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9813 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/draggable.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5929 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16465 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecSimpleTransform.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10407 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16061 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecStat.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/echarts-dagre.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   986443 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/echarts.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7598 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/esl.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3080 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/facePrint.js
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/fflate/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30151 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/fflate/index.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9690 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/frameInsight.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    95957 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/jquery.min.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9937 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/perlin.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3908 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/rearrange.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/require.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11232 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/requireES.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2984 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/reset.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   320509 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/rollup.browser.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34282 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/testHelper.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16108 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/main.css
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/src/require.js
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    37985 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/translator_rest.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4718 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/dropmake/web/translator_utils.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/dlg/translator/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/translator/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/dlg/translator/__pycache__/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      165 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      163 2022-12-21 05:49:48.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11776 2022-12-21 08:43:30.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/tool_commands.cpython-310.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11757 2022-11-30 13:05:03.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/tool_commands.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11783 2022-12-21 05:49:48.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/tool_commands.cpython-39.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      291 2023-02-19 06:22:55.000000 daliuge-translator-2.4.0/dlg/translator/__pycache__/version.cpython-38.pyc
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14943 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg/translator/tool_commands.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      223 2023-03-11 06:01:20.000000 daliuge-translator-2.4.0/dlg/translator/version.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1043 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/dlg.spec
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/docker/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      936 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/docker/Dockerfile
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      943 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/docker/Dockerfile.dev
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      809 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/docker/Dockerfile.ray
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      966 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/docker/README.md
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)     1080 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/run_translator.sh
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-03-11 06:01:20.467363 daliuge-translator-2.4.0/setup.cfg
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3731 2023-03-11 05:57:46.000000 daliuge-translator-2.4.0/setup.py
--rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)      100 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/stop_translator.sh
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/test/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.463363 daliuge-translator-2.4.0/test/dropmake/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.467363 daliuge-translator-2.4.0/test/dropmake/logical_graphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10167 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/HelloWorld_simple.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27903 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/Plasma-test.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    27883 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/Plasma_test.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    29943 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/SharedMemoryTest.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   122809 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/chiles_simple.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   145441 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/cont_img.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12121 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/dlg-lg.graph.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10861 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/dlg-lg.json.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12121 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/dlg-lg.schema
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    74241 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/eagle_gather.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    57734 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/eagle_gather_empty.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    67163 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/eagle_gather_simple.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   205135 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/lofar_std.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12929 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/nagsIo.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20439 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/simpleMKN.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15110 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/test-20190830-110556.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10319 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/testLoop (1).graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    24061 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/testLoop.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10370 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/testScatter.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    73505 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/dropmake/logical_graphs/test_grpby_gather.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1913 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/test_lg_fill.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17966 2023-02-01 08:50:20.000000 daliuge-translator-2.4.0/test/dropmake/test_lgweb.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8278 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/test_pg_gen.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4638 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/dropmake/test_scheduler.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.467363 daliuge-translator-2.4.0/test/reproducibility/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/reproducibility/__init__.py
-drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-03-11 06:01:20.467363 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18215 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/HelloSBash.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18125 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/HelloSPython.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18129 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/HelloSPython2.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18205 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/HelloWorldBash.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18210 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/HelloWorldBashSplit.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5076 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/HelloWorldFile.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21994 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/apps.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10023 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/files.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9555 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/groupUse.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    29734 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/groups.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6418 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/misc.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    38202 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/simpleNoScatter.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    38200 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/reproGraphs/simpleScatter.graph
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    96017 2023-03-02 10:50:42.000000 daliuge-translator-2.4.0/test/reproducibility/test_accumulatedata.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    20399 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/reproducibility/test_integration.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1472 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/reproducibility/test_json_output.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2107 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/reproducibility/test_repro_inits.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6605 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/reproducibility/test_reprodata_compare.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6045 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/reproducibility/test_scatter_blockdag.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2356 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test/test_tool_trans.py
--rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      111 2022-11-30 13:05:02.000000 daliuge-translator-2.4.0/test-requirements.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.608460 daliuge-translator-3.0.0/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      180 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/MANIFEST.in
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      307 2023-05-18 12:49:51.608460 daliuge-translator-3.0.0/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      157 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/README.md
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.592460 daliuge-translator-3.0.0/daliuge_translator.egg-info/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      307 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/daliuge_translator.egg-info/PKG-INFO
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4898 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/daliuge_translator.egg-info/SOURCES.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        1 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/daliuge_translator.egg-info/dependency_links.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       62 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/daliuge_translator.egg-info/entry_points.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      152 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/daliuge_translator.egg-info/requires.txt
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)        9 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/daliuge_translator.egg-info/top_level.txt
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.592460 daliuge-translator-3.0.0/dlg/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1275 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1055 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3051 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/definition_classes.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26528 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/dm_utils.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16498 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/lg.graph.schema
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    35682 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/lg.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    36368 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/lg_node.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/lib/
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   382436 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/lib/libmetis.dylib
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)   495581 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/lib/libmetis.so
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7869 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/pg_generator.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5689 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/pg_manager.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17731 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/pgt.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26019 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/pgtp.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    51636 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/scheduler.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/utils/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/utils/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11713 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/utils/anneal.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5848 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/utils/antichains.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3470 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/utils/bash_parameter.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/utils/heft/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8068 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/utils/heft/base.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/web/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26530 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/LICENSE
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      963 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   139114 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/d3.v3.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11324 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/web/graph_init.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/web/img/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    14438 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/img/jsoneditor-icons.png
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      878 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/license.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    28292 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/main.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7019 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/web/matrix_vis.html
+-rwxrwxr-x   0 awicenec  (1000) awicenec  (1000)    15050 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/pg_viewer.html
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17286 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/pure-min.css
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.596460 daliuge-translator-3.0.0/dlg/dropmake/web/src/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5649 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/FileSaver.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.592460 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.600460 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    64548 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   151749 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    48488 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   108539 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4897 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    76483 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4021 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    32461 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   192348 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   492048 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   155758 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   625953 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.600460 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   222911 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   402249 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    78635 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   311949 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   131637 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   250568 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    58072 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   190253 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.600460 daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   243027 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/d3.v5.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   894427 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/dagre-d3.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   725181 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/dagre-d3.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      806 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/data_prep.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/echarts-dagre.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.604460 daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    69177 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   174048 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    79612 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    60840 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   165349 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/html2canvas.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.604460 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      177 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/arrow_right_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      409 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/explore_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5372 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/liu.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5403 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/liuFavIcon.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1462 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/settings_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    26026 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/translate_green.png
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      423 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/zoom_in_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      370 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/zoom_out_map_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      404 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/zoom_out_white_24dp.svg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30747 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/jquery-ui.min.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    89500 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/jquery.min.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.604460 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17804 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/canteen.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1943 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/caseFrame.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    12066 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/caseFrame.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7037 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/config.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7545 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/countup.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    45411 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/dat.gui.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9813 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/draggable.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     5929 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16465 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecSimpleTransform.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    10407 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16061 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecStat.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    94506 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/echarts-dagre.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   986443 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/echarts.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     7598 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/esl.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3080 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/facePrint.js
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.604460 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/fflate/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    30151 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/fflate/index.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9690 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/frameInsight.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    95957 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/jquery.min.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     9937 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/perlin.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3908 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/rearrange.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/require.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    11232 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/requireES.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2984 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/reset.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)   320509 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/rollup.browser.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    34282 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/testHelper.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    16108 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/main.css
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    17695 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/src/require.js
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    39409 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/dropmake/web/translator_rest.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4718 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/dropmake/web/translator_utils.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.604460 daliuge-translator-3.0.0/dlg/translator/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/dlg/translator/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    15225 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/dlg/translator/tool_commands.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      223 2023-05-18 12:49:51.000000 daliuge-translator-3.0.0/dlg/translator/version.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)       38 2023-05-18 12:49:51.608460 daliuge-translator-3.0.0/setup.cfg
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     3769 2023-05-18 12:43:13.000000 daliuge-translator-3.0.0/setup.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.604460 daliuge-translator-3.0.0/test/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1496 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/__init__.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.608460 daliuge-translator-3.0.0/test/dropmake/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/dropmake/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1918 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/dropmake/test_lg_fill.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    18833 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/dropmake/test_lgweb.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     8215 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/dropmake/test_pg_gen.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     4666 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/dropmake/test_scheduler.py
+drwxrwxr-x   0 awicenec  (1000) awicenec  (1000)        0 2023-05-18 12:49:51.608460 daliuge-translator-3.0.0/test/reproducibility/
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)      965 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/reproducibility/__init__.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    99731 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/reproducibility/test_accumulatedata.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)    21073 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/reproducibility/test_integration.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     1472 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/reproducibility/test_json_output.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2107 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/reproducibility/test_repro_inits.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6605 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/reproducibility/test_reprodata_compare.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     6045 2023-05-18 12:38:53.000000 daliuge-translator-3.0.0/test/reproducibility/test_scatter_blockdag.py
+-rw-rw-r--   0 awicenec  (1000) awicenec  (1000)     2898 2023-05-18 12:40:21.000000 daliuge-translator-3.0.0/test/test_tool_trans.py
```

### Comparing `daliuge-translator-2.4.0/.coveragerc` & `daliuge-translator-3.0.0/dlg/dropmake/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,20 @@
+#    ICRAR - International Centre for Radio Astronomy Research
+#    (c) UWA - The University of Western Australia, 2015
+#    Copyright by UWA (in the framework of the ICRAR)
+#    All rights reserved
+#
+#    This library is free software; you can redistribute it and/or
+#    modify it under the terms of the GNU Lesser General Public
+#    License as published by the Free Software Foundation; either
+#    version 2.1 of the License, or (at your option) any later version.
+#
+#    This library is distributed in the hope that it will be useful,
+#    but WITHOUT ANY WARRANTY; without even the implied warranty of
+#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+#    Lesser General Public License for more details.
+#
+#    You should have received a copy of the GNU Lesser General Public
+#    License along with this library; if not, write to the Free Software
+#    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
+#    MA 02111-1307  USA
 #
-# Coverage configuration file
-#
-# ICRAR - International Centre for Radio Astronomy Research
-# (c) UWA - The University of Western Australia, 2020
-# Copyright by UWA (in the framework of the ICRAR)
-# All rights reserved
-#
-# This library is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public
-# License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
-#
-# This library is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# Lesser General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public
-# License along with this library; if not, write to the Free Software
-# Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-# MA 02111-1307  USA
-#
-
-# We currently exclude the deploy directory because it's not
-# part of the core software
-[run]
-source = dlg
-         ../daliuge-common/dlg
```

### Comparing `daliuge-translator-2.4.0/dlg/__init__.py` & `daliuge-translator-3.0.0/dlg/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/__init__.py` & `daliuge-translator-3.0.0/dlg/dropmake/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/dm_utils.py` & `daliuge-translator-3.0.0/dlg/dropmake/dm_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,38 @@
 """
 
 import copy
 import json
 import logging
 import os
 import os.path as osp
-
-from dlg.common import Categories
+from .definition_classes import ConstructTypes
 
 logger = logging.getLogger(__name__)
 
 LG_VER_OLD = 1
 LG_VER_EAGLE_CONVERTED = 2
 LG_VER_EAGLE = 3
 LG_APPREF = "AppRef"
 
 TEMP_FILE_FOLDER = "/tmp"
 
 
+class GraphException(Exception):
+    pass
+
+
+class GInvalidLink(GraphException):
+    pass
+
+
+class GInvalidNode(GraphException):
+    pass
+
+
 def get_lg_ver_type(lgo):
     """
     Get the version type of this logical graph
     """
     # with open(lg_name, 'r+') as file_object:
     #     lgo = json.load(file_object)
 
@@ -175,15 +186,15 @@
     old_new_parent_map_split_1 = dict()
     old_new_parent_map_split_2 = dict()
     dont_change_group = set()
     n_products_map = dict()
     app_keywords = ["inputApplicationName", "outputApplicationName"]
 
     for node in lgo["nodeDataArray"]:
-        if Categories.MKN != node["category"]:
+        if ConstructTypes.MKN != node["category"]:
             continue
         for ak in app_keywords:
             if ak not in node:
                 raise Exception(
                     "MKN construct {0} must specify {1}".format(
                         node["key"], ak
                     )
@@ -192,67 +203,69 @@
         for mknv in node["fields"]:
             mknv_dict[mknv["name"]] = int(mknv["value"])
         M, K, N = mknv_dict["m"], mknv_dict["k"], mknv_dict["n"]
 
         # step 1 - clone the current MKN
         mkn_key = node["key"]
         mkn_local_input_keys = [
-            _make_unique_port_key(x["Id"], node["key"])
-            for x in node["inputLocalPorts"]
+            _make_unique_port_key(x["id"], node["key"])
+            for x in node["inputAppFields"]
+            if x["usage"] == "InputPort"
         ]
         mkn_output_keys = [
-            _make_unique_port_key(x["Id"], node["key"])
-            for x in node["outputPorts"]
+            _make_unique_port_key(x["id"], node["key"])
+            for x in node["inputAppFields"]
+            if x["usage"] == "OutputPort"
         ]
         node_mk = node
         node_mk["mkn"] = [M, K, N]
         node_kn = copy.deepcopy(node_mk)
         node_split_n = copy.deepcopy(node_mk)
 
         node_mk["application"] = node["inputApplicationName"]
-        node_mk["category"] = Categories.GATHER
-        node_mk["type"] = Categories.GATHER
+        node_mk["category"] = ConstructTypes.GATHER
+        node_mk["categoryType"] = ConstructTypes.GATHER
         ipan = node_mk.get("inputApplicationName", "")
         if len(ipan) == 0:
-            node_mk["text"] = node_mk["text"] + "_InApp"
+            node_mk["name"] = node_mk["name"] + "_InApp"
         else:
-            node_mk["text"] = ipan
+            node_mk["name"] = ipan
         #        del node_mk["inputApplicationName"]
         #        del node_mk["outputApplicationName"]
         #        del node_mk["outputAppFields"]
         new_field = {
             "name": "num_of_inputs",
-            "text": "Number of inputs",
+            "name": "Number of inputs",
             "value": "%d" % (M),
         }
         node_mk["fields"].append(new_field)
 
-        node_kn["category"] = Categories.SCATTER
-        node_kn["type"] = Categories.SCATTER
+        node_kn["category"] = ConstructTypes.SCATTER
+        node_kn["categoryType"] = ConstructTypes.SCATTER
 
         opan = node_kn.get("outputAppName", "")
         if len(opan) == 0:
-            node_kn["text"] = node_kn["text"] + "_OutApp"
+            node_kn["name"] = node_kn["name"] + "_OutApp"
         else:
-            node_kn["text"] = opan
+            node_kn["name"] = opan
         k_new = min(keyset) - 1
         keyset.add(k_new)
         node_kn["key"] = k_new
         node_kn["group"] = mkn_key
         dont_change_group.add(k_new)
         old_new_parent_map_split_1[mkn_key] = k_new
         node_kn["application"] = node_kn["outputApplicationName"]
         node_kn["inputAppFields"] = node_kn["outputAppFields"]
         #        del node_kn["inputApplicationName"]
         #        del node_kn["outputApplicationName"]
         #        del node_kn["outputAppFields"]
 
         new_field_kn = {
             "name": "num_of_copies",
-            "text": "Number of copies",
+            "name": "Number of copies",
             "value": "%d" % (K),
         }
         node_kn["fields"].append(new_field_kn)
         node_kn["reprodata"] = node.get("reprodata", {}).copy()
         lgo["nodeDataArray"].append(node_kn)
 
         # for all connections that point to the local input ports of the MKN construct
@@ -261,17 +274,17 @@
             old_new_k2n_to_map[mlik] = k_new
 
         # for all connections that go from the outputPorts of the MKN construct
         # we reconnect them from the new scatter
         for mok in mkn_output_keys:
             old_new_k2n_from_map[mok] = k_new
 
-        node_split_n["category"] = Categories.SCATTER
-        node_split_n["type"] = Categories.SCATTER
-        node_split_n["text"] = "Nothing"
+        node_split_n["category"] = ConstructTypes.SCATTER
+        node_split_n["categoryType"] = ConstructTypes.SCATTER
+        node_split_n["name"] = "Nothing"
         k_new = min(keyset) - 1
         keyset.add(k_new)
         node_split_n["key"] = k_new
         node_split_n["group"] = mkn_key
         dont_change_group.add(k_new)
         old_new_parent_map_split_2[mkn_key] = k_new
 
@@ -281,15 +294,15 @@
         #        del node_split_n["inputApplicationName"]
         #        del node_split_n["outputApplicationName"]
         #        del node_split_n["outputAppFields"]
         # del node_split_n['intputAppFields']
 
         new_field_kn = {
             "name": "num_of_copies",
-            "text": "Number of copies",
+            "name": "Number of copies",
             "value": "%d" % (N),
         }
         node_split_n["fields"].append(new_field_kn)
         node_split_n["reprodata"] = node.get("reprodata", {}).copy()
         lgo["nodeDataArray"].append(node_split_n)
 
     need_to_change_n_products = dict()
@@ -336,15 +349,15 @@
     """
     keyset = get_keyset(lgo)
     old_new_k2n_to_map = dict()
     old_new_k2n_from_map = dict()
     app_keywords = ["inputApplicationName", "outputApplicationName"]
 
     for node in lgo["nodeDataArray"]:
-        if Categories.MKN != node["category"]:
+        if ConstructTypes.MKN != node["category"]:
             continue
         for ak in app_keywords:
             if ak not in node:
                 raise Exception(
                     "MKN construct {0} must specify {1}".format(
                         node["key"], ak
                     )
@@ -359,40 +372,38 @@
         # mkn_key = node['key']
         mkn_local_input_keys = [x["Id"] for x in node["inputLocalPorts"]]
         mkn_output_keys = [x["Id"] for x in node["outputPorts"]]
         node_mk = node
         node_kn = copy.deepcopy(node_mk)
 
         node_mk["application"] = node["inputApplicationName"]
-        node_mk["category"] = Categories.GATHER
-        node_mk["text"] = node_mk["text"] + "_InApp"
+        node_mk["category"] = ConstructTypes.GATHER
+        node_mk["name"] = node_mk["name"] + "_InApp"
         del node["inputApplicationName"]
         del node["outputApplicationName"]
         del node["outputAppFields"]
         new_field = {
             "name": "num_of_inputs",
-            "text": "Number of inputs",
             "value": "%d" % (ratio_mk),
         }
         node_mk["fields"].append(new_field)
 
-        node_kn["category"] = Categories.GATHER
-        node_kn["text"] = node_kn["text"] + "_OutApp"
+        node_kn["category"] = ConstructTypes.GATHER
+        node_kn["name"] = node_kn["name"] + "_OutApp"
         k_new = min(keyset) - 1
         keyset.add(k_new)
         node_kn["key"] = k_new
         node_kn["application"] = node_kn["outputApplicationName"]
         node_kn["inputAppFields"] = node_kn["outputAppFields"]
         del node_kn["inputApplicationName"]
         del node_kn["outputApplicationName"]
         del node_kn["outputAppFields"]
 
         new_field_kn = {
-            "name": "num_of_inputs",
-            "text": "Number of inputs",
+            "name": "Number of inputs",
             "value": "%d" % (ratio_kn),
         }
         node_kn["fields"].append(new_field_kn)
         node_kn["reprodata"] = node.get("reprodata", {}).copy()
         lgo["nodeDataArray"].append(node_kn)
 
         # for all connections that point to the local input ports of the MKN construct
@@ -416,15 +427,18 @@
 
 def getAppRefInputs(lgo):
     """
     Function to retrieve the inputs from an App node referenced by a group.
     Used to recover the Gather node inputs for AppRef format graphs.
     """
     for node in lgo["nodeDataArray"]:
-        if node["category"] not in [Categories.SCATTER, Categories.GATHER]:
+        if node["category"] not in [
+            ConstructTypes.SCATTER,
+            ConstructTypes.GATHER,
+        ]:
             continue
         has_app = None
 
     pass
 
 
 def convert_construct(lgo):
@@ -446,17 +460,17 @@
     # a cycle that is not allowed in DAG during graph translation
 
     # CAUTION: THIS IS VERY LIKELY TO CAUSE ISSUES, SINCE IT IS PICKING THE FIRST ONE FOUND!
     #    app_keywords = ["application", "inputApplicationType", "outputApplicationType"]
     app_keywords = ["inputApplicationType", "outputApplicationType"]
     for node in lgo["nodeDataArray"]:
         if node["category"] not in [
-            Categories.SCATTER,
-            Categories.GATHER,
-            Categories.SERVICE,
+            ConstructTypes.SCATTER,
+            ConstructTypes.GATHER,
+            ConstructTypes.SERVICE,
         ]:
             continue
         has_app = None
 
         # try to find a application using several app_keywords
         # disregard app_keywords that are not present, or have value "None"
         for ak in app_keywords:
@@ -471,18 +485,17 @@
             continue
         # step 1
         app_node = dict()
         app_node["reprodata"] = node.get("reprodata", {}).copy()
         app_node["key"] = node["key"]
         app_node["category"] = node[has_app]  # node['application']
         if has_app[0] == "i":
-            app_node["text"] = node["text"]
+            app_node["name"] = node["text"] if "text" in node else node["name"]
         else:
-            app_node["text"] = node["text"]
-
+            app_node["name"] = node["text"] if "text" in node else node["name"]
         if "mkn" in node:
             app_node["mkn"] = node["mkn"]
 
         if "group" in node:
             app_node["group"] = node["group"]
 
         INPUT_APP_FIELDS = "inputAppFields"
@@ -491,40 +504,42 @@
             # regular application drops
             app_node["fields"] = list(node[INPUT_APP_FIELDS])
             app_node["fields"] += node["fields"]
             # TODO: remove, use fields list
             for afd in node[INPUT_APP_FIELDS]:
                 app_node[afd["name"]] = afd["value"]
 
-        if node["category"] == Categories.GATHER:
+        if node["category"] == ConstructTypes.GATHER:
             app_node["group_start"] = 1
 
-        if node["category"] == Categories.SERVICE:
+        if node["category"] == ConstructTypes.SERVICE:
             app_node["isService"] = True
 
         new_nodes.append(app_node)
 
         # step 2
         k_new = min(keyset) - 1
         node["key"] = k_new
         keyset.add(k_new)
         old_new_grpk_map[app_node["key"]] = k_new
 
-        if Categories.GATHER == node["category"]:
+        if ConstructTypes.GATHER == node["category"]:
             old_new_gather_map[app_node["key"]] = k_new
             app_node["group"] = k_new
             app_node["group_start"] = 1
 
             # extra step to deal with "internal output" fromo within Gather
             dup_app_node_k = min(keyset) - 1
             keyset.add(dup_app_node_k)
             dup_app_node = dict()
             dup_app_node["key"] = dup_app_node_k
             dup_app_node["category"] = node[has_app]  # node['application']
-            dup_app_node["text"] = node["text"]
+            dup_app_node["name"] = (
+                node["text"] if "text" in node else node["name"]
+            )
 
             if "mkn" in node:
                 dup_app_node["mkn"] = node["mkn"]
 
             if "group" in node:
                 dup_app_node["group"] = node["group"]
 
@@ -543,58 +558,62 @@
         # step 3
         for node in lgo["nodeDataArray"]:
             if "group" in node and node["group"] in old_new_grpk_map:
                 k_old = node["group"]
                 node["group"] = old_new_grpk_map[k_old]
 
         # step 4
-        for link in lgo["linkDataArray"]:
-            if link["to"] in old_new_gather_map:
-                k_old = link["to"]
-                k_new = old_new_gather_map[k_old]
-                link["to"] = k_new
-
-                # deal with the internal output from Gather
-                from_node = node_index[link["from"]]
-                # this is an obsolete and awkard way of checking internal output (for backward compatibility)
-                if "group" in from_node and from_node["group"] == k_new:
-                    dup_app_node = duplicated_gather_app[k_new]
-                    k_new_new = dup_app_node["key"]
-                    link["to"] = k_new_new
-                    if k_new_new not in node_index:
-                        node_index[k_new_new] = dup_app_node
-                        dup_app_node["reprodata"] = (
-                            node_index[k_new].get("reprodata", {}).copy()
-                        )
-                        lgo["nodeDataArray"].append(dup_app_node)
-                        old_newnew_gather_map[k_old] = k_new_new
-
-        # step 5
-        # relink the connection from gather to its external output if the gather
-        # has internal output that has been delt with in Step 4
-        for link in lgo["linkDataArray"]:
-            if link["from"] in old_new_gather_map:
-                k_old = link["from"]
-                k_new = old_new_gather_map[k_old]
-                to_node = node_index[link["to"]]
-                gather_construct = node_index[k_new]
-                if "group" not in to_node and "group" not in gather_construct:
-                    cond1 = True
-                elif (
-                    "group" in to_node
-                    and "group" in gather_construct
-                    and to_node["group"] == gather_construct["group"]
-                ):
-                    cond1 = True
-                else:
-                    cond1 = False
-
-                if cond1 and (k_old in old_newnew_gather_map):
-                    link["from"] = old_newnew_gather_map[k_old]
-                # print("from %d to %d to %d" % (link['from'], k_old, link['to']))
+        if len(old_new_gather_map) > 0:
+            for link in lgo["linkDataArray"]:
+                if link["to"] in old_new_gather_map:
+                    k_old = link["to"]
+                    k_new = old_new_gather_map[k_old]
+                    link["to"] = k_new
+
+                    # deal with the internal output from Gather
+                    from_node = node_index[link["from"]]
+                    # this is an obsolete and awkard way of checking internal output (for backward compatibility)
+                    if "group" in from_node and from_node["group"] == k_new:
+                        dup_app_node = duplicated_gather_app[k_new]
+                        k_new_new = dup_app_node["key"]
+                        link["to"] = k_new_new
+                        if k_new_new not in node_index:
+                            node_index[k_new_new] = dup_app_node
+                            dup_app_node["reprodata"] = (
+                                node_index[k_new].get("reprodata", {}).copy()
+                            )
+                            lgo["nodeDataArray"].append(dup_app_node)
+                            old_newnew_gather_map[k_old] = k_new_new
+
+            # step 5
+            # relink the connection from gather to its external output if the gather
+            # has internal output that has been delt with in Step 4
+            for link in lgo["linkDataArray"]:
+                if link["from"] in old_new_gather_map:
+                    k_old = link["from"]
+                    k_new = old_new_gather_map[k_old]
+                    to_node = node_index[link["to"]]
+                    gather_construct = node_index[k_new]
+                    if (
+                        "group" not in to_node
+                        and "group" not in gather_construct
+                    ):
+                        cond1 = True
+                    elif (
+                        "group" in to_node
+                        and "group" in gather_construct
+                        and to_node["group"] == gather_construct["group"]
+                    ):
+                        cond1 = True
+                    else:
+                        cond1 = False
+
+                    if cond1 and (k_old in old_newnew_gather_map):
+                        link["from"] = old_newnew_gather_map[k_old]
+                    # print("from %d to %d to %d" % (link['from'], k_old, link['to']))
 
     # print('%d nodes in lg after construct conversion' % len(lgo['nodeDataArray']))
     return lgo
 
 
 def convert_eagle_to_daliuge_json(lg_name):
     """
@@ -646,16 +665,16 @@
 
             if group_key != "":
                 # This is a node inside a group.
                 group_node = nodes_all.get(group_key, "")
                 group_category = group_node.get("category", "")
 
                 if (
-                    group_category == Categories.GATHER
-                    or group_category == Categories.GROUP_BY
+                    group_category == ConstructTypes.GATHER
+                    or group_category == ConstructTypes.GROUP_BY
                 ):
                     # Check if the node is first in that group.
                     fields = node["fields"]
                     for field in fields:
                         name = field.get("name", "")
                         if name == "group_start":
                             group_start = field.get("value", "")
@@ -699,14 +718,27 @@
         )
     finally:
         pass
 
     return new_path
 
 
+def load_lg(f):
+    if isinstance(f, str):
+        if not os.path.exists(f):
+            raise GraphException("Logical graph {0} not found".format(f))
+        with open(f) as f:
+            lg = json.load(f)
+    elif hasattr(f, "read"):
+        lg = json.load(f)
+    else:
+        lg = f
+    return lg
+
+
 if __name__ == "__main__":
     import pkg_resources
 
     lg_dir = pkg_resources.resource_filename(
         __name__, "../../test/dropmake/logical_graphs"
     )  # @UndefinedVariable
     lg_name = f"{lg_dir}/lofar_std.graph"
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/lg.graph.schema` & `daliuge-translator-3.0.0/dlg/dropmake/lg.graph.schema`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990949572088403%*

 * *Differences: {"'properties'": "{'modelData': {'properties': {'shortDescription': OrderedDict([('type', "*

 * *                 "'string')]), 'detailedDescription': OrderedDict([('type', 'string')])}, "*

 * *                 "'required': {insert: [(17, 'shortDescription'), (18, 'detailedDescription')]}}, "*

 * *                 "'nodeDataArray': {'items': {'properties': {'inputAppFields': {'items': "*

 * *                 "{'required': {delete: [2]}}}, 'outputAppFields': {'items': {'required': {delete: "*

 * *                 "[2]}}}, 'fields':  […]*

```diff
@@ -40,14 +40,17 @@
             "type": "array"
         },
         "modelData": {
             "properties": {
                 "commitHash": {
                     "type": "string"
                 },
+                "detailedDescription": {
+                    "type": "string"
+                },
                 "downloadUrl": {
                     "type": "string"
                 },
                 "eagleCommitHash": {
                     "type": "string"
                 },
                 "eagleVersion": {
@@ -85,14 +88,17 @@
                 },
                 "repositoryUrl": {
                     "type": "string"
                 },
                 "schemaVersion": {
                     "type": "string"
                 },
+                "shortDescription": {
+                    "type": "string"
+                },
                 "signature": {
                     "type": "string"
                 }
             },
             "required": [
                 "filePath",
                 "fileType",
@@ -106,15 +112,17 @@
                 "lastModifiedName",
                 "lastModifiedEmail",
                 "lastModifiedDatetime",
                 "numLGNodes",
                 "commitHash",
                 "downloadUrl",
                 "repositoryUrl",
-                "signature"
+                "signature",
+                "shortDescription",
+                "detailedDescription"
             ],
             "type": "object"
         },
         "nodeDataArray": {
             "items": {
                 "properties": {
                     "applicationArgs": {
@@ -164,15 +172,14 @@
                                         "null"
                                     ]
                                 }
                             },
                             "required": [
                                 "description",
                                 "name",
-                                "text",
                                 "value",
                                 "type",
                                 "precious",
                                 "options",
                                 "positional"
                             ],
                             "type": "object"
@@ -250,15 +257,14 @@
                                         "null"
                                     ]
                                 }
                             },
                             "required": [
                                 "description",
                                 "name",
-                                "text",
                                 "value",
                                 "type",
                                 "precious",
                                 "options",
                                 "positional"
                             ],
                             "type": "object"
@@ -291,15 +297,14 @@
                                         "null"
                                     ]
                                 }
                             },
                             "required": [
                                 "description",
                                 "name",
-                                "text",
                                 "value"
                             ],
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "inputApplicationName": {
@@ -370,15 +375,14 @@
                                         "null"
                                     ]
                                 }
                             },
                             "required": [
                                 "description",
                                 "name",
-                                "text",
                                 "value"
                             ],
                             "type": "object"
                         },
                         "type": "array"
                     },
                     "outputApplicationName": {
@@ -451,32 +455,26 @@
                     "color",
                     "commitHash",
                     "dataHash",
                     "description",
                     "drawOrderHint",
                     "expanded",
                     "fields",
-                    "applicationArgs",
                     "height",
                     "inputAppFields",
                     "inputApplicationName",
                     "inputApplicationType",
-                    "inputLocalPorts",
-                    "inputPorts",
                     "isGroup",
                     "key",
                     "outputAppFields",
                     "outputApplicationName",
                     "outputApplicationType",
-                    "outputLocalPorts",
-                    "outputPorts",
                     "paletteDownloadUrl",
                     "repositoryUrl",
                     "subject",
-                    "text",
                     "width",
                     "x",
                     "y"
                 ],
                 "type": "object"
             },
             "type": "array"
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/lib/libmetis.dylib` & `daliuge-translator-3.0.0/dlg/dropmake/lib/libmetis.dylib`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/lib/libmetis.so` & `daliuge-translator-3.0.0/dlg/dropmake/lib/libmetis.so`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/pg_generator.py` & `daliuge-translator-3.0.0/dlg/dropmake/pg_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,30 +69,24 @@
 
 
 def unroll(lg, oid_prefix=None, zerorun=False, app=None):
     """Unrolls a logical graph"""
     start = time.time()
     lg = LG(lg, ssid=oid_prefix)
     drop_list = lg.unroll_to_tpl()
-    logger.info(
-        "Logical Graph unroll completed in %.3f [s]. # of Drops: %d",
-        (time.time() - start),
-        len(drop_list),
-    )
-    # Optionally set sleepTimes to 0 and apps to a specific type
     if zerorun:
         for dropspec in drop_list:
-            if "sleepTime" in dropspec:
-                dropspec["sleepTime"] = 0
+            if "sleep_time" in dropspec:
+                dropspec["sleep_time"] = 0
     if app:
         logger.info("Replacing apps with %s", app)
         for dropspec in drop_list:
-            if "app" in dropspec:
-                dropspec["app"] = app
-                dropspec["sleepTime"] = (
+            if "dropclass" in dropspec:
+                dropspec["dropclass"] = app
+                dropspec["sleep_time"] = (
                     dropspec["execution_time"]
                     if "execution_time" in dropspec
                     else 2
                 )
     drop_list.append(lg.reprodata)
     return drop_list
 
@@ -117,14 +111,22 @@
 }
 
 
 def known_algorithms():
     return [x for x in _known_algos.keys() if isinstance(x, str)]
 
 
+def _get_algo_param(algo_params, param_name, default):
+    """
+    Make sure that default is set even if value has been passed as None.
+    """
+    param = algo_params.get(param_name)
+    return param if param is not None else default
+
+
 def partition(
     pgt,
     algo,
     num_partitions=1,
     num_islands=1,
     partition_label="partition",
     show_gojs=False,
@@ -155,23 +157,23 @@
         algo_params,
     )
 
     # Read all possible values with defaults
     # Not all algorithms use them, but makes the coding easier
     # do_merge = num_islands > 1
     could_merge = True
-    min_goal = algo_params.get("min_goal", 0)
-    ptype = algo_params.get("ptype", 0)
-    max_load_imb = algo_params.get("max_load_imb", 90)
-    max_cpu = algo_params.get("max_cpu", 8)
-    max_mem = algo_params.get("max_mem", 1000)
-    time_greedy = algo_params.get("time_greedy", 50)
-    deadline = algo_params.get("deadline", None)
-    topk = algo_params.get("topk", 30)
-    swarm_size = algo_params.get("swarm_size", 40)
+    min_goal = _get_algo_param(algo_params, "min_goal", 0)
+    ptype = _get_algo_param(algo_params, "ptype", 0)
+    max_load_imb = _get_algo_param(algo_params, "max_load_imb", 90)
+    max_cpu = _get_algo_param(algo_params, "max_cpu", 8)
+    max_mem = _get_algo_param(algo_params, "max_mem", 1000)
+    time_greedy = _get_algo_param(algo_params, "time_greedy", 50)
+    deadline = _get_algo_param(algo_params, "deadline", None)
+    topk = _get_algo_param(algo_params, "topk", 30)
+    swarm_size = _get_algo_param(algo_params, "swarm_size", 40)
 
     max_dop = {"num_cpus": max_cpu, "mem_usage": max_mem}
 
     if algo == ALGO_NONE:
         pgt = PGT(pgt)
 
     elif algo == ALGO_METIS:
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/pg_manager.py` & `daliuge-translator-3.0.0/dlg/dropmake/pg_manager.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/pgt.py` & `daliuge-translator-3.0.0/dlg/dropmake/pgt.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 import json
 import logging
 import math
 
 from dlg.dropmake.lg import GraphException
 from dlg.dropmake.scheduler import DAGUtil
 from dlg.common import CategoryType, dropdict
-from dlg.common import Categories, DropType
 
 logger = logging.getLogger(__name__)
 
 
 class GPGTNoNeedMergeException(GraphException):
     pass
 
@@ -54,15 +53,19 @@
     A DROP representation of Physical Graph Template
     """
 
     def __init__(self, drop_list, build_dag=True):
         self._drop_list = drop_list
         self._drop_list_len = len(drop_list)
         self._extra_drops = []  # artifacts DROPs produced during L2G mapping
-        self._dag = DAGUtil.build_dag_from_drops(self._drop_list) if build_dag else None
+        self._dag = (
+            DAGUtil.build_dag_from_drops(self._drop_list)
+            if build_dag
+            else None
+        )
         self._json_str = None
         self._oid_gid_map = dict()
         self._gid_island_id_map = dict()
         self._num_parts_done = 0
         self._partition_merged = 0
         self._inner_parts = []  # a list of inner partitions (e.g. nodes)
         # for visualisation only
@@ -71,23 +74,29 @@
         self._merge_parts = False
         self._island_labels = ["Data", "Compute"]
         self._data_movement = None
         self._reprodata = {}
 
     def _can_merge(self, new_num_parts):
         if new_num_parts <= 0:
-            raise GPGTException("Invalid new_num_parts {0}".format(new_num_parts))
+            raise GPGTException(
+                "Invalid new_num_parts {0}".format(new_num_parts)
+            )
         if not self._merge_parts:
             raise GPGTException(
-                "This {0} PGTP is not made for merging".format(self.__class__.__name__)
+                "This {0} PGTP is not made for merging".format(
+                    self.__class__.__name__
+                )
             )
         if self._num_parts_done <= new_num_parts:
             raise GPGTNoNeedMergeException(
                 "No need to merge this {0} PGTP: {1} <= {2}".format(
-                    self.__class__.__name__, self._num_parts_done, new_num_parts
+                    self.__class__.__name__,
+                    self._num_parts_done,
+                    new_num_parts,
                 )
             )
         if self._partition_merged == new_num_parts:
             return False
         else:
             return True
 
@@ -151,18 +160,22 @@
         """
         Return the TOTAL data movement
         """
         if self._data_movement is not None:
             return self._data_movement
         elif self.dag is not None:
             G = self.dag
-            self._data_movement = sum(e[2].get("weight", 0) for e in G.edges(data=True))
+            self._data_movement = sum(
+                e[2].get("weight", 0) for e in G.edges(data=True)
+            )
         return self._data_movement
 
-    def pred_exec_time(self, app_drop_only=False, wk="weight", force_answer=False):
+    def pred_exec_time(
+        self, app_drop_only=False, wk="weight", force_answer=False
+    ):
         """
         Predict execution time using the longest path length
         """
         G = self.dag
         if G is None:
             if force_answer:
                 self._dag = DAGUtil.build_dag_from_drops(self._drop_list)
@@ -197,15 +210,20 @@
 
     def merge_partitions(
         self, new_num_parts, form_island=False, island_type=0, visual=False
     ):
         raise Exception("Not implemented. Call sub-class")
 
     def to_pg_spec(
-        self, node_list, ret_str=True, num_islands=1, tpl_nodes_len=0, co_host_dim=True
+        self,
+        node_list,
+        ret_str=True,
+        num_islands=1,
+        tpl_nodes_len=0,
+        co_host_dim=True,
     ):
         """
         convert pgt to pg specification, and map that to the hardware resources
 
         node_list:
             A list of nodes (list), whose length == (num_islands + num_node_mgrs)
             if co_locate_islands = False.
@@ -217,41 +235,45 @@
               depending on the length of node_list
             - num_islands can't be < 1
 
         tpl_nodes_len: if this is given we generate a pg_spec template
             The pg_spec template is what needs to be send to a deferred deployemnt
             where the daliuge system is started up afer submission (e.g. SLURM)
         """
-        logger.debug("tpl_nodes_len: %s, node_list: %s", tpl_nodes_len, node_list)
+        logger.debug(
+            "tpl_nodes_len: %s, node_list: %s", tpl_nodes_len, node_list
+        )
         if tpl_nodes_len > 0:  # generate pg_spec template
             node_list = range(tpl_nodes_len)  # create a fake list for now
 
         if 0 == self._num_parts_done:
             raise GPGTException("The graph has not been partitioned yet")
 
         if node_list is None or 0 == len(node_list):
             raise GPGTException("Node list is empty!")
         nodes_len = len(node_list)
 
         try:
             num_islands = int(num_islands)
         except:
-            raise GPGTException("Invalid num_islands spec: {0}".format(num_islands))
+            raise GPGTException(
+                "Invalid num_islands spec: {0}".format(num_islands)
+            )
         if num_islands < 1:
             num_islands = 1  # need at least one island manager
         if num_islands > nodes_len:
             raise GPGTException(
                 "Number of islands must be <= number of specified nodes!"
             )
         form_island = num_islands > 1
         if nodes_len < 1:  # we allow to run everything on a single node now!
             raise GPGTException("Too few nodes: {0}".format(nodes_len))
 
         num_parts = self._num_parts_done
-        drop_list = self._drop_list + self._extra_drops
+        drop_list = self.drops
 
         # deal with the co-hosting of DIMs
         if not co_host_dim:
             if form_island and num_parts > nodes_len:
                 raise GPGTException(
                     "Insufficient number of nodes: {0}".format(nodes_len)
                 )
@@ -263,15 +285,18 @@
                     "Insufficient number of nodes: {0}".format(nodes_len)
                 )
             is_list = node_list
             nm_list = node_list
         nm_len = len(nm_list)
         logger.info(
             "Drops count: %d, partitions count: %d, nodes count: %d, island count: %d",
-            len(drop_list), num_parts, nodes_len, len(is_list)
+            len(drop_list),
+            num_parts,
+            nodes_len,
+            len(is_list),
         )
 
         if form_island:
             self.merge_partitions(num_islands, form_island=True)
             # from Eq.1 we know that num_parts <= nm_len
             # so no need to update its value
         elif nm_len < num_parts:
@@ -286,22 +311,21 @@
         # then the test_metis_pgtp_gen_pg_island fails. This needs more investigation
         # but is a corner case.
         # values = set(dict(lm).values()) # old unique values
         # values = dict(zip(values,range(len(values)))) # dict with new values
         # lm = {k:values[v] for (k, v) in lm.items()} # replace old values with new
 
         if tpl_nodes_len:
-            nm_list = ["#%s" % x for x in range(nm_len)]  # so that nm_list[i] == '#i'
+            nm_list = [
+                "#%s" % x for x in range(nm_len)
+            ]  # so that nm_list[i] == '#i'
             is_list = [
                 "#%s" % x for x in range(len(is_list))
             ]  # so that is_list[i] == '#i'
 
-        logger.info(
-            "nm_list: %s, is_list: %s, lm: %s, lm2: %s", nm_list, is_list, lm, lm2
-        )
         for drop in drop_list:
             oid = drop["oid"]
             # For now, simply round robin, but need to consider
             # nodes cross COMPUTE islands which has
             # TODO consider distance between a pair of nodes
             gid = lm[oid]
             drop["node"] = nm_list[gid]
@@ -329,69 +353,69 @@
 
         for i, drop in enumerate(self._drop_list):
             oid = drop["oid"]
             node = dict()
             node["key"] = i + 1
             key_dict[oid] = i + 1
             node["oid"] = oid
-            tt = drop["type"]
-            if DropType.DATA == tt:
-                node["category"] = Categories.DATA
-            elif DropType.APP == tt:
-                node["category"] = Categories.COMPONENT
-            node["text"] = drop["nm"]
+            tt = drop["categoryType"]
+            if CategoryType.DATA == tt:
+                node["category"] = "Data"
+            elif CategoryType.APPLICATION == tt:
+                node["category"] = "Application"
+            node["name"] = drop["name"]
             nodes.append(node)
 
         if self._extra_drops is None:
             extra_drops = []
             remove_edges = []
             add_edges = []  # a list of tuples
             add_nodes = []
             for drop in self._drop_list:
                 oid = drop["oid"]
                 myk = key_dict[oid]
                 for i, oup in enumerate(G.successors(myk)):
                     link = dict()
                     link["from"] = myk
-                    from_dt = 0 if drop["type"] == DropType.DATA else 1
-                    to_dt = G.nodes[oup]["dt"]
+                    from_dt = (
+                        0
+                        if drop["categoryType"] in [CategoryType.DATA, "data"]
+                        else 1
+                    )
+                    to_dt = G.nodes[oup]["drop_type"]
                     if from_dt == to_dt:
                         to_drop = G.nodes[oup]["drop_spec"]
                         if from_dt == 0:
                             # add an extra app DROP
                             extra_oid = "{0}_TransApp_{1}".format(oid, i)
                             dropSpec = dropdict(
                                 {
                                     "oid": extra_oid,
-                                    "type": DropType.APP,
                                     "categoryType": CategoryType.APPLICATION,
-                                    "app": "dlg.drop.BarrierAppDROP",
-                                    "nm": "go_app",
-                                    "text": "go_app",
-                                    "tw": 1,
+                                    "dropclass": "dlg.drop.BarrierAppDROP",
+                                    "name": "go_app",
+                                    "weight": 1,
                                 }
                             )
                             # create links
                             drop.addConsumer(dropSpec)
                             dropSpec.addInput(drop)
                             dropSpec.addOutput(to_drop)
                             to_drop.addProducer(dropSpec)
                             mydt = 1
                         else:
                             # add an extra data DROP
                             extra_oid = "{0}_TransData_{1}".format(oid, i)
                             dropSpec = dropdict(
                                 {
                                     "oid": extra_oid,
-                                    "type": DropType.DATA,
                                     "categoryType": CategoryType.DATA,
-                                    "storage": Categories.MEMORY,
-                                    "nm": "go_data",
-                                    "text": "go_data",
-                                    "dw": 1,
+                                    "dropclass": "dlg.data.drops.memory.InMemoryDROP",
+                                    "name": "go_data",
+                                    "weight": 1,
                                 }
                             )
                             drop.addOutput(dropSpec)
                             dropSpec.addProducer(drop)
                             dropSpec.addConsumer(to_drop)
                             to_drop.addInput(dropSpec)
                             mydt = 0
@@ -401,25 +425,37 @@
                         endlink = dict()
                         endlink["from"] = lid
                         endlink["to"] = oup
                         links.append(endlink)
                         # global graph updates
                         # the new drop must have the same gid as the to_drop
                         add_nodes.append(
-                            (lid, 1, mydt, dropSpec, G.nodes[oup].get("gid", None))
+                            (
+                                lid,
+                                1,
+                                mydt,
+                                dropSpec,
+                                G.nodes[oup].get("gid", None),
+                            )
                         )
                         remove_edges.append((myk, oup))
                         add_edges.append((myk, lid))
                         add_edges.append((lid, oup))
                     else:
                         link["to"] = oup
                     links.append(link)
             for gn in add_nodes:
                 # logger.debug("added gid = {0} for new node {1}".format(gn[4], gn[0]))
-                G.add_node(gn[0], weight=gn[1], dt=gn[2], drop_spec=gn[3], gid=gn[4])
+                G.add_node(
+                    gn[0],
+                    weight=gn[1],
+                    drop_type=gn[2],
+                    drop_spec=gn[3],
+                    gid=gn[4],
+                )
             G.remove_edges_from(remove_edges)
             G.add_edges_from(add_edges)
             self._extra_drops = extra_drops
         else:
             for drop in self._drop_list:
                 oid = drop["oid"]
                 myk = key_dict[oid]
@@ -431,21 +467,20 @@
 
         # going through the extra_drops
         for i, drop in enumerate(self._extra_drops):
             oid = drop["oid"]
             node = dict()
             node["key"] = (i + 1) * -1
             node["oid"] = oid
-            tt = drop["type"]
-            if DropType.DATA == tt:
-                node["category"] = Categories.DATA
-            elif DropType.APP == tt:
-                node["category"] = Categories.COMPONENT
-            node["text"] = drop["nm"]
-            node["text"] = drop["text"]
+            tt = drop["categoryType"]
+            if tt == CategoryType.DATA:
+                node["category"] = "Data"
+            elif tt == CategoryType.APPLICATION:
+                node["category"] = "PythonApp"  # might not be correct
+            node["name"] = drop["name"]
             nodes.append(node)
 
         ret["nodeDataArray"] = nodes
         ret["linkDataArray"] = links
         self._gojs_json_obj = ret
         if string_rep:
             return json.dumps(ret, indent=2)
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/pgtp.py` & `daliuge-translator-3.0.0/dlg/dropmake/pgtp.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from dlg.dropmake.pgt import PGT, GPGTException
 from dlg.dropmake.scheduler import (
     MySarkarScheduler,
     DAGUtil,
     MinNumPartsScheduler,
     PSOScheduler,
 )
-from dlg.common import DropType
+from dlg.common import CategoryType
 
 logger = logging.getLogger(__name__)
 
 
 class MetisPGTP(PGT):
     """
     DROP and GOJS representations of Physical Graph Template with Partitions
@@ -96,23 +96,23 @@
         both upstream and downstream nodes to fit its input format
         """
         key_dict = dict()  # key - oid, value - GOJS key
         droplist = self._drop_list
 
         G = nx.Graph()
         G.graph["edge_weight_attr"] = "weight"
-        G.graph["node_weight_attr"] = "tw"
-        G.graph["node_size_attr"] = "sz"
+        G.graph["node_weight_attr"] = "weight"
+        G.graph["node_size_attr"] = "size"
 
         for i, drop in enumerate(droplist):
             try:
                 oid = drop["oid"]
             except KeyError:
                 logger.debug("Drop does not have oid: %s", drop)
-                continue
+                droplist.pop(i)
             key_dict[oid] = i + 1  # METIS index starts from 1
 
         logger.info("Metis partition input progress - dropdict is built")
 
         if self._drop_list_len > 1e7:
             import resource
 
@@ -120,39 +120,39 @@
                 "self._drop_list, max RSS: %.2f GB",
                 resource.getrusage(resource.RUSAGE_SELF)[2] / 1024.0**2,
             )
 
         for i, drop in enumerate(droplist):
             oid = drop["oid"]
             myk = i + 1
-            tt = drop["type"]
-            if DropType.DATA == tt:
+            tt = drop["categoryType"]
+            if tt in [CategoryType.DATA, "data"]:
                 dst = "consumers"  # outbound keyword
                 ust = "producers"
                 tw = 1  # task weight is zero for a Data DROP
-                sz = drop.get("dw", 1)  # size
-            elif DropType.APP == tt:
+                sz = drop.get("weight", 1)  # size
+            elif tt in [CategoryType.APPLICATION, "app"]:
                 dst = "outputs"
                 ust = "inputs"
-                tw = drop["tw"]
+                tw = drop.get("weight", 1)
                 sz = 1
-            G.add_node(myk, tw=tw, sz=sz, oid=oid)
+            G.add_node(myk, weight=tw, size=sz, oid=oid)
             adj_drops = []  # adjacent drops (all neighbours)
             if dst in drop:
                 adj_drops += drop[dst]
             if ust in drop:
                 adj_drops += drop[ust]
 
             for inp in adj_drops:
                 key = list(inp.keys())[0] if isinstance(inp, dict) else inp
-                if DropType.DATA == tt:
-                    lw = drop["dw"]
-                elif DropType.APP == tt:
-                    # lw = drop_dict[inp].get('dw', 1)
-                    lw = droplist[key_dict[key] - 1].get("dw", 1)
+                if tt in [CategoryType.DATA, "data"]:
+                    lw = drop["weight"]
+                elif tt in [CategoryType.APPLICATION, "app"]:
+                    # get the weight of the previous drop
+                    lw = droplist[key_dict[key] - 1].get("weight", 1)
                 if lw <= 0:
                     lw = 1
                 G.add_edge(myk, key_dict[key], weight=lw)
         # for e in G.edges(data=True):
         #     if (e[2]['weight'] == 0):
         #         e[2]['weight'] = 1
         if self._drop_list_len > 1e7:
@@ -208,30 +208,34 @@
 
         # the following is for potential partition merging into islands
         if self._merge_parts:
             for gid in groups:
                 group_weight[gid] = [0, 0]
             for gnode in G.nodes(data=True):
                 tt = group_weight[gnode[1]["gid"]]
-                tt[0] += gnode[1]["tw"]
-                tt[1] += gnode[1]["sz"]
+                try:
+                    tt[0] += int(gnode[1]["weight"])
+                    tt[1] += int(gnode[1]["size"])
+                except ValueError:
+                    tt[0] = 1
+                    tt[1] = 1
         # the following is for visualisation using GOJS
         if jsobj is not None:
             node_list = jsobj["nodeDataArray"]
             for node in node_list:
                 nid = int(node["key"])
                 gid = metis_out[nid - 1]
                 node["group"] = gid + start_k
 
             inner_parts = []
             for gid in groups:
                 gn = dict()
                 gn["key"] = start_k + gid
                 gn["isGroup"] = True
-                gn["text"] = "{1}_{0}".format(gid + 1, self._par_label)
+                gn["name"] = "{1}_{0}".format(gid + 1, self._par_label)
                 node_list.append(gn)
                 inner_parts.append(gn)
 
             self._inner_parts = inner_parts
             self._node_list = node_list
 
     def to_gojs_json(self, string_rep=True, outdict=None, visual=False):
@@ -323,21 +327,21 @@
             k = "{0}**{1}".format(from_gid, to_gid)
             part_edges[k] += e[2]["weight"]
 
         # 1. build the bi-directional graph again
         # with each partition being a node
         G = nx.Graph()
         G.graph["edge_weight_attr"] = "weight"
-        G.graph["node_weight_attr"] = "tw"
-        G.graph["node_size_attr"] = "sz"
+        G.graph["node_weight_attr"] = "weight"
+        G.graph["node_size_attr"] = "size"
         for gid, v in self._group_workloads.items():
             # for compute islands, we need to count the # of nodes instead of
             # the actual workload
             twv = 1 if (island_type == 1) else v[0]
-            G.add_node(gid, tw=twv, sz=v[1])
+            G.add_node(gid, weight=twv, size=v[1])
         for glinks, v in part_edges.items():
             gl = glinks.split("**")
             G.add_edge(int(gl[0]), int(gl[1]), weight=v)
 
         if new_num_parts == 1:
             (edgecuts, metis_parts) = (0, [0] * len(G.nodes()))
         else:
@@ -386,15 +390,15 @@
                 start_i = start_k + self._num_parts_done
                 node_list = self._node_list
                 for island_id in islands:
                     # print('island_id = ', island_id)
                     gn = dict()
                     gn["key"] = island_id + start_i
                     gn["isGroup"] = True
-                    gn["text"] = "{1}_{0}".format(island_id + 1, island_label)
+                    gn["name"] = "{1}_{0}".format(island_id + 1, island_label)
                     node_list.append(gn)
                 inner_parts = self._inner_parts
                 for ip in inner_parts:
                     ip["group"] = tmp_map[ip["key"] - start_k] + start_i
 
 
 class MySarkarPGTP(PGT):
@@ -532,15 +536,15 @@
                     self._island_labels[island_type % len(self._island_labels)]
                 )
                 node_list = self._node_list
                 for island_id in outer_groups:
                     gn = dict()
                     gn["key"] = island_id + start_i
                     gn["isGroup"] = True
-                    gn["text"] = "{1}_{0}".format(island_id + 1, island_label)
+                    gn["name"] = "{1}_{0}".format(island_id + 1, island_label)
                     node_list.append(gn)
 
                 for ip in inner_parts:
                     ip["group"] = (
                         in_out_part_map[ip["key"] - start_k] + start_i
                     )
 
@@ -616,15 +620,15 @@
             for gid in groups:
                 gn = dict()
                 gn["key"] = gid
                 # logger.debug("group key = {0}".format(gid))
                 gn["isGroup"] = True
                 # gojs group_id label starts from 1
                 # so "gid - leng" instead of "gid - start_k"
-                gn["text"] = "{1}_{0}".format(
+                gn["name"] = "{1}_{0}".format(
                     (gid - start_k + 1), self._par_label
                 )
                 node_list.append(gn)
                 inner_parts.append(gn)
 
             self._node_list = node_list
             self._inner_parts = inner_parts
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/scheduler.py` & `daliuge-translator-3.0.0/dlg/dropmake/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import networkx as nx
 import numpy as np
 import pkg_resources
 from pyswarm import pso
 
 from .utils.antichains import get_max_weighted_antichain
-from ..common import dropdict, get_roots, DropType
+from ..common import dropdict, get_roots, CategoryType
 
 logger = logging.getLogger(__name__)
 
 DEBUG = 0
 
 
 class SchedulerException(Exception):
@@ -46,15 +46,17 @@
 class Schedule(object):
     """
     The scheduling solution with schedule-related properties
     """
 
     def __init__(self, dag, max_dop):
         self._dag = dag
-        self._max_dop = max_dop if type(max_dop) == int else max_dop.get("num_cpus", 1)
+        self._max_dop = (
+            max_dop if type(max_dop) == int else max_dop.get("num_cpus", 1)
+        )
         DAGUtil.label_schedule(self._dag)
         self._lpl = DAGUtil.get_longest_path(
             self._dag, default_weight=0, show_path=True
         )
         self._wkl = None
         self._sma = None
 
@@ -135,15 +137,17 @@
             the mean # of resource units per time unit consumed by the graph/partition
         """
         if self._wkl is None:
             ma = self.schedule_matrix
             c = []
             for i in range(ma.shape[1]):
                 c.append(np.count_nonzero(ma[:, i]))
-            self._wkl = int(np.mean(np.array(c)))  # since METIS only accepts integer
+            self._wkl = int(
+                np.mean(np.array(c))
+            )  # since METIS only accepts integer
         return self._wkl
 
     @property
     def efficiency(self):
         """
         resource usage percentage (integer)
         """
@@ -170,15 +174,14 @@
         self._lpl = None
         self._schedule = None
         self._max_dop = None
         self._parent_id = None
         self._child_parts = None
         self._tmp_merge_dag = None
         self._tmp_new_ac = None
-        logger.debug("My dop = %r", self._ask_max_dop)
 
     @property
     def parent_id(self):
         return self._parent_id
 
     @parent_id.setter
     def parent_id(self, value):
@@ -255,23 +258,25 @@
             mydop = DAGUtil.get_max_dop(self._dag)
         else:
             mydop = self.probe_max_dop(u, v, unew, vnew)
             # TODO - put the following code in a unit test!
             if DEBUG:
                 mydop_slow = DAGUtil.get_max_dop(self._dag)  #
                 if mydop_slow != mydop:
-                    err_msg = "u = {0}, v = {1}, unew = {2}, vnew = {3}".format(
-                        u, v, unew, vnew
+                    err_msg = (
+                        "u = {0}, v = {1}, unew = {2}, vnew = {3}".format(
+                            u, v, unew, vnew
+                        )
                     )
                     raise SchedulerException(
                         "{2}: mydop = {0}, mydop_slow = {1}".format(
                             mydop, mydop_slow, err_msg
                         )
                     )
-        ret = False if mydop > self._ask_max_dop.get('num_cpus', 1) else True
+        ret = False if mydop > self._ask_max_dop.get("num_cpus", 1) else True
         if unew:
             self.remove(u)
         if vnew:
             self.remove(v)
         return (ret, unew, vnew)
 
     def add(self, u, v, gu, gv, sequential=False, global_dag=None):
@@ -439,32 +444,39 @@
         self_global_dag = self._global_dag
         for _w_attr in self._w_attr:
             u_aw = self_global_dag.nodes[u].get(_w_attr, 1)
             kwargs[_w_attr] = u_aw
         kwargs["weight"] = self_global_dag.nodes[u].get("weight", 5)
         self._dag.add_node(u, **kwargs)
         for k in self._w_attr:
-            self._tmp_max_dop[k] = get_max_weighted_antichain(self._dag, w_attr=k)[0]
+            self._tmp_max_dop[k] = get_max_weighted_antichain(
+                self._dag, w_attr=k
+            )[0]
         self._max_dop = self._tmp_max_dop
 
     def can_merge(self, that, u, v):
         """"""
         dag = nx.compose(self._dag, that._dag)
         if u is not None:
             dag.add_edge(u, v)
         tmp_max_dop = copy.deepcopy(self._tmp_max_dop)
 
         for _w_attr in self._w_attr:
+            ask_max_dop = (
+                self._ask_max_dop[_w_attr]
+                if self._ask_max_dop[_w_attr] is not None
+                else 1
+            )
             mydop = get_max_weighted_antichain(dag, w_attr=_w_attr)[0]
-            curr_max = max(self._max_dop[_w_attr], that._max_dop[_w_attr])
+            curr_max = max(ask_max_dop, that._max_dop[_w_attr])
 
             if mydop <= curr_max:
                 # if you don't increase DoP, we accept that immediately
                 tmp_max_dop[_w_attr] = curr_max
-            elif mydop > self._ask_max_dop[_w_attr]:
+            elif mydop > ask_max_dop:
                 return False
             else:
                 tmp_max_dop[_w_attr] = mydop
 
         self._tmp_max_dop = tmp_max_dop  # only change it when returning True
         return True
 
@@ -521,22 +533,26 @@
         metis = DAGUtil.import_metis()
         G = nx.Graph()
         st_gid = len(self._drop_list) + len(self._parts) + 1
         if bal_cond == 0:
             G.graph["node_weight_attr"] = ["wkl", "eff"]
             for part in self._parts:
                 sc = part.schedule
-                G.add_node(part.partition_id, wkl=sc.workload, eff=sc.efficiency)
+                G.add_node(
+                    part.partition_id, wkl=sc.workload, eff=sc.efficiency
+                )
         else:
             G.graph["node_weight_attr"] = "cc"
             for part in self._parts:
                 # sc = part.schedule
                 pdop = part._max_dop
                 # TODO add memory as one of the LB condition too
-                cc_eval = pdop if type(pdop) == int else pdop.get("num_cpus", 1)
+                cc_eval = (
+                    pdop if type(pdop) == int else pdop.get("num_cpus", 1)
+                )
                 G.add_node(part.partition_id, cc=cc_eval)
 
         for e in self._part_edges:
             u = e[0]
             v = e[1]
             ugid = self._dag.nodes[u].get("gid", None)
             vgid = self._dag.nodes[v].get("gid", None)
@@ -548,15 +564,17 @@
                 G[ugid][vgid]["weight"] = ew
         # DAGUtil.metis_part(G, 15)
         # since METIS does not allow zero edge weight, reset them to one
         for e in G.edges(data=True):
             if e[2]["weight"] == 0:
                 e[2]["weight"] = 1
         # logger.debug(G.nodes(data=True))
-        (edgecuts, metis_parts) = metis.part_graph(G, nparts=num_partitions, ufactor=1)
+        (edgecuts, metis_parts) = metis.part_graph(
+            G, nparts=num_partitions, ufactor=1
+        )
 
         for node, pt in zip(G.nodes(), metis_parts):  # note min(pt) == 0
             parent_id = pt + st_gid
             child_part = self._part_dict[node]
             child_part.parent_id = parent_id
             # logger.debug("Part {0} --> Cluster {1}".format(child_part.partition_id, parent_id))
             # parent_part = Partition(parent_id, None)
@@ -586,15 +604,17 @@
     3. adjustable for local schedulers
 
     Similar ideas:
     http://stackoverflow.com/questions/3974731
     """
 
     def __init__(self, drop_list, max_dop=8, dag=None, dump_progress=False):
-        super(MySarkarScheduler, self).__init__(drop_list, max_dop=max_dop, dag=dag)
+        super(MySarkarScheduler, self).__init__(
+            drop_list, max_dop=max_dop, dag=dag
+        )
         self._sspace = [3] * len(self._dag.edges())  # all edges are not zeroed
         self._dump_progress = dump_progress
 
     def override_cannot_add(self):
         """
         Whether this scheduler will override the False result from `Partition.can_add()`
         """
@@ -669,22 +689,32 @@
         # TODO consider other w_attrs other than CPUs!
         parts.sort(key=lambda x: x._max_dop["num_cpus"])
         while not done_reduction:
             for i, partA in enumerate(parts):
                 if i < len(parts) - 1:
                     partB = parts[i + 1]
                     new_part = self._merge_two_parts(
-                        partA._gid, partB._gid, None, None, None, None, g_dict, parts, G
+                        partA._gid,
+                        partB._gid,
+                        None,
+                        None,
+                        None,
+                        None,
+                        g_dict,
+                        parts,
+                        G,
                     )
                     if new_part is not None:
                         num_reductions += 1
                         break  # force re-sorting
                 else:
                     done_reduction = True
-                    logger.info("Performed reductions %d times", num_reductions)
+                    logger.info(
+                        "Performed reductions %d times", num_reductions
+                    )
                     break
 
     def partition_dag(self):
         """
         Return a tuple of
             1. the # of partitions formed (int)
             2. the parallel time (longest path, int)
@@ -716,15 +746,17 @@
             v = e[1]
             gv = G.nodes[v]
             ow = G.adj[u][v]["weight"]
             G.adj[u][v]["weight"] = 0  # edge zeroing
             ugid = gu.get("gid", None)
             vgid = gv.get("gid", None)
             if ugid != vgid:  # merge existing parts
-                part = self._merge_two_parts(ugid, vgid, u, v, gu, gv, g_dict, parts, G)
+                part = self._merge_two_parts(
+                    ugid, vgid, u, v, gu, gv, g_dict, parts, G
+                )
                 if part is not None:
                     st_gid -= 1
                     self._sspace[i] = 1
                 else:
                     G.adj[u][v]["weight"] = ow
                     self._part_edges.append(e)
             if dump_progress:
@@ -749,16 +781,20 @@
 class MinNumPartsScheduler(MySarkarScheduler):
     """
     A special type of partition that aims to schedule the DAG on time but at minimum cost.
     In this particular case, the cost is the number of partitions that will be generated.
     The assumption is # of partitions (with certain DoP) more or less represents resource footprint.
     """
 
-    def __init__(self, drop_list, deadline, max_dop=8, dag=None, optimistic_factor=0.5):
-        super(MinNumPartsScheduler, self).__init__(drop_list, max_dop=max_dop, dag=dag)
+    def __init__(
+        self, drop_list, deadline, max_dop=8, dag=None, optimistic_factor=0.5
+    ):
+        super(MinNumPartsScheduler, self).__init__(
+            drop_list, max_dop=max_dop, dag=dag
+        )
         self._deadline = deadline
         self._optimistic_factor = optimistic_factor
 
     def override_cannot_add(self):
         return True
 
     def is_time_critical(self, u, uw, unew, v, vw, vnew, curr_lpl, ow, rem_el):
@@ -834,28 +870,38 @@
         the objective function sets up a partition scheme such that
             (1) DoP constrints for each partiiton are satisfied
                 based on X[i] value, reject or linearisation
             (2) returns makespan
     """
 
     def __init__(
-        self, drop_list, max_dop=8, dag=None, deadline=None, topk=30, swarm_size=40
+        self,
+        drop_list,
+        max_dop=8,
+        dag=None,
+        deadline=None,
+        topk=30,
+        swarm_size=40,
     ):
         super(PSOScheduler, self).__init__(drop_list, max_dop=max_dop, dag=dag)
         self._deadline = deadline
         # search space: key - combination of X[i] (string),
         # val - a tuple of (critical_path (int), num_parts (int))
         self._sspace_dict = dict()
         self._topk = topk
-        self._swarm_size = swarm_size
-        self._lite_dag = DAGUtil.build_dag_from_drops(self._drop_list, embed_drop=False)
+        self._swarm_size = swarm_size if swarm_size is not None else 40
+        self._lite_dag = DAGUtil.build_dag_from_drops(
+            self._drop_list, embed_drop=False
+        )
         self._call_counts = 0
         leng = len(self._lite_dag.edges())
         self._leng = leng
-        self._topk = leng if self._topk is None or leng < self._topk else self._topk
+        self._topk = (
+            leng if self._topk is None or leng < self._topk else self._topk
+        )
 
     def partition_dag(self):
         """
         Returns a tuple of:
             1. the # of partitions formed (int)
             2. the parallel time (longest path, int)
             3. partition time (seconds, float)
@@ -863,15 +909,17 @@
         """
         # trigger the PSO algorithm
         G = self._dag
         lb = [0.99] * self._leng
         ub = [3.01] * self._leng
         stt = time.time()
         if self._deadline is None:
-            xopt, fopt = pso(self.objective_func, lb, ub, swarmsize=self._swarm_size)
+            xopt, fopt = pso(
+                self.objective_func, lb, ub, swarmsize=self._swarm_size
+            )
         else:
             xopt, fopt = pso(
                 self.objective_func,
                 lb,
                 ub,
                 ieqcons=[self.constrain_func],
                 swarmsize=self._swarm_size,
@@ -913,15 +961,17 @@
             if pos == 3:  # 10 non_zero + 1
                 continue
             elif pos == 2:  # 01 zero with linearisation + 1
                 linear = True
             elif pos == 1:  # 00 zero without linearisation + 1
                 linear = False
             else:
-                raise SchedulerException("PSO position out of bound: {0}".format(pos))
+                raise SchedulerException(
+                    "PSO position out of bound: {0}".format(pos)
+                )
 
             u = e[0]
             gu = G.nodes[u]
             v = e[1]
             gv = G.nodes[v]
             ow = G.adj[u][v]["weight"]
             G.adj[u][v]["weight"] = 0  # edge zeroing
@@ -973,15 +1023,17 @@
         )
 
     def constrain_func(self, x):
         """
         Deadline - critical_path >= 0
         """
         if self._deadline is None:
-            raise SchedulerException("Deadline is None, cannot apply constraints!")
+            raise SchedulerException(
+                "Deadline is None, cannot apply constraints!"
+            )
 
         sk = "".join([str(int(round(xi))) for xi in x[0 : self._topk]])
         stuff = self._sspace_dict.get(sk, None)
         if stuff is None:
             G = self._lite_dag.copy()
             stuff = self._partition_G(G, x)
             self._sspace_dict[sk] = stuff[0:2]
@@ -991,15 +1043,17 @@
     def objective_func(self, x):
         """
         x is a list of values, each taking one of the 3 integers: 0,1,2 for an edge
         indices of x is identical to the indices in G.edges().sort(key='weight')
         """
         # first check if the solution is already available in the search space
         sk = "".join([str(int(round(xi))) for xi in x[0 : self._topk]])
-        stuff = self._sspace_dict.get(sk, None)  # TODO is this atomic operation?
+        stuff = self._sspace_dict.get(
+            sk, None
+        )  # TODO is this atomic operation?
         if stuff is None:
             # make a deep copy to avoid mix up multiple particles,
             # each of which has multiple iterations
             G = self._lite_dag.copy()
             stuff = self._partition_G(G, x)
             self._sspace_dict[sk] = stuff[0:2]
             del G
@@ -1129,15 +1183,17 @@
             parents = list(G.predecessors(v))
             if len(parents) == 0:
                 gv["stt"] = 0
             else:
                 # get the latest end time of one of its parents
                 ledt = -1
                 for parent in parents:
-                    pedt = G.nodes[parent]["edt"] + G.adj[parent][v].get(weight, 0)
+                    pedt = G.nodes[parent]["edt"] + G.adj[parent][v].get(
+                        weight, 0
+                    )
                     if pedt > ledt:
                         ledt = pedt
                 gv["stt"] = ledt
             gv["edt"] = gv["stt"] + gv.get(weight, 0)
 
     @staticmethod
     def ganttchart_matrix(G, topo_sort=None):
@@ -1163,15 +1219,17 @@
             # print i, n, stt, edt
             leng = edt - stt
             if edt == stt:
                 continue
             try:
                 ma[i, stt:edt] = np.ones((1, leng))
             except:
-                logger.error("i, stt, edt, leng = %d, %d, %d, %d", i, stt, edt, leng)
+                logger.error(
+                    "i, stt, edt, leng = %d, %d, %d, %d", i, stt, edt, leng
+                )
                 logger.error("N, M = %d, %d", M, N)
                 raise
             # print ma[i, :]
         return ma
 
     @staticmethod
     def import_metis():
@@ -1191,24 +1249,27 @@
             mt._part_graph = mt.part_graph
 
             def logged_part_graph(*args, **kwargs):
                 logger.info("Starting metis partitioning")
                 start = time.time()
                 ret = mt._part_graph(*args, **kwargs)  # @UndefinedVariable
                 logger.info(
-                    "Finished metis partitioning in %.3f [s]", time.time() - start
+                    "Finished metis partitioning in %.3f [s]",
+                    time.time() - start,
                 )
                 return ret
 
             mt.part_graph = logged_part_graph
             mt._dlg_patched = True
         return mt
 
     @staticmethod
-    def build_dag_from_drops(drop_list, embed_drop=True, fake_super_root=False):
+    def build_dag_from_drops(
+        drop_list, embed_drop=True, fake_super_root=False
+    ):
         """
         return a networkx Digraph (DAG)
         :param: fake_super_root whether to create a fake super root node in the DAG
         If set to True, it enables edge zero-based scheduling agorithms to make
         more aggressive merging
         """
         # tw - task weight
@@ -1220,67 +1281,93 @@
             oid = drop["oid"]
             key_dict[oid] = i + 1  # starting from 1
             drop_dict[oid] = drop
         G = nx.DiGraph()
         for i, drop in enumerate(drop_list):
             oid = drop["oid"]
             myk = i + 1
-            tt = drop["type"]
-            if DropType.DATA == tt:
+            tt = drop["categoryType"]
+            if tt in [CategoryType.DATA, "data"]:
                 # if (drop['nm'] == 'StreamNull'):
                 #     obk = 'streamingConsumers'
                 # else:
                 #     obk = 'consumers' # outbound keyword
                 tw = 0
                 dtp = 0
-            elif DropType.APP == tt:
+            elif tt in [CategoryType.APPLICATION, "app"]:
                 # obk = 'outputs'
-                tw = int(drop["tw"])
+                try:
+                    tw = int(drop["weight"])
+                except (ValueError, KeyError):
+                    tw = 1
                 dtp = 1
-            elif DropType.SERVICE_APP == tt:
-                tw = int(drop["tw"])
+            elif tt in [CategoryType.SERVICE, "serviceapp"]:
+                try:
+                    tw = int(drop["weight"])
+                except (ValueError, KeyError):
+                    tw = 1
                 dtp = 1
             else:
-                raise SchedulerException("Drop Type '{0}' not supported".format(tt))
+                raise SchedulerException(
+                    "Drop Type '{0}' not supported".format(tt)
+                )
             num_cpus = drop.get("num_cpus", 1)
             if embed_drop:
                 G.add_node(
                     myk,
                     weight=tw,
-                    # text=drop["nm"],
-                    text=drop["text"],
-                    dt=dtp,
+                    text=drop["name"],
+                    drop_type=dtp,
                     drop_spec=drop,
                     num_cpus=num_cpus,
                 )
             else:
                 G.add_node(
-                    myk, weight=tw, text=drop["text"], dt=dtp, num_cpus=num_cpus)
+                    myk,
+                    weight=tw,
+                    text=drop["name"],
+                    drop_type=dtp,
+                    num_cpus=num_cpus,
+                )
             for obk in out_bound_keys:
                 if obk in drop:
                     for oup in drop[obk]:
-                        key = list(oup.keys())[0] if isinstance(oup, dict) else oup
-                        if DropType.DATA == tt:
+                        key = (
+                            list(oup.keys())[0]
+                            if isinstance(oup, dict)
+                            else oup
+                        )
+                        if CategoryType.DATA == tt:
                             G.add_weighted_edges_from(
-                                [(myk, key_dict[key], int(drop["dw"]))]
+                                [(myk, key_dict[key], int(drop["weight"]))]
                             )
-                        elif DropType.APP == tt:
+                        elif CategoryType.APPLICATION == tt:
                             G.add_weighted_edges_from(
-                                [(myk, key_dict[key], int(drop_dict[key].get("dw", 5)))]
+                                [
+                                    (
+                                        myk,
+                                        key_dict[key],
+                                        int(drop_dict[key].get("weight", 5)),
+                                    )
+                                ]
                             )
 
         if fake_super_root:
             super_root = dropdict(
-                {"oid": "-92", "type": DropType.DATA, "storage": "null"}
+                {
+                    "oid": "-92",
+                    "categoryType": CategoryType.DATA,
+                    "dropclass": "dlg.data.drops.data_base.NullDROP",
+                }
             )
             super_k = len(drop_list) + 1
             G.add_node(
                 super_k,
                 weight=0,
-                dtp=0,
+                drop_type=0,
                 drop_spec=super_root,
                 num_cpus=0,
                 text="fake_super_root",
             )
 
             for oup in get_roots(drop_list):
                 G.add_weighted_edges_from([(super_k, key_dict[oup], 1)])
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/utils/__init__.py` & `daliuge-translator-3.0.0/dlg/dropmake/web/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/utils/anneal.py` & `daliuge-translator-3.0.0/dlg/dropmake/utils/anneal.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/utils/antichains.py` & `daliuge-translator-3.0.0/dlg/dropmake/utils/antichains.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/utils/bash_parameter.py` & `daliuge-translator-3.0.0/dlg/dropmake/utils/bash_parameter.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/utils/heft/base.py` & `daliuge-translator-3.0.0/dlg/dropmake/utils/heft/base.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/LICENSE` & `daliuge-translator-3.0.0/dlg/dropmake/web/LICENSE`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/__init__.py` & `daliuge-translator-3.0.0/test/dropmake/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#
 #    ICRAR - International Centre for Radio Astronomy Research
 #    (c) UWA - The University of Western Australia, 2015
 #    Copyright by UWA (in the framework of the ICRAR)
 #    All rights reserved
 #
 #    This library is free software; you can redistribute it and/or
 #    modify it under the terms of the GNU Lesser General Public
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/d3.v3.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/graph_init.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/graph_init.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -226,15 +226,15 @@
 
     if (g.hasNode(g)) {
         return false;
     }
 
     var typeClass = node.category;
     var typeShape = TYPE_SHAPES[node.category];
-    var notes = node.text;
+    var notes = node.name;
 
     var oid = node.oid;
     var html = '<div class="drop-label ' + typeShape + '" id="id_' + oid + '">';
     html += '<span class="notes">' + notes + '</span>';
     html += '<span style="font-size: 13px;">' + oid + '</span>';
     html += "</div>";
     g.setNode(oid, {
@@ -282,17 +282,17 @@
     // var nodeCount = 0
     var renderer = 'canvas'
     var fontSize = 10
     data.nodeDataArray.forEach(element => {
         newElement = {};
         if (!element.hasOwnProperty("isGroup")) {
             // helper map to fix the links later
-            keyIndex.set(element.key, element.text + '-' + element.key.toString());
+            keyIndex.set(element.key, element.name + '-' + element.key.toString());
             //data options
-            newElement.name = element.text + '-' + element.key.toString();
+            newElement.name = element.name + '-' + element.key.toString();
 
             newElement.label = {
                 'rotate': 45,
                 'fontSize': fontSize,
                 'offset': [-20, -20],
                 'fontWeight': 400,
                 'color': element.group.toString(),
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/img/jsoneditor-icons.png` & `daliuge-translator-3.0.0/dlg/dropmake/web/img/jsoneditor-icons.png`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/license.html` & `daliuge-translator-3.0.0/dlg/dropmake/web/license.html`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/main.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/main.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/matrix_vis.html` & `daliuge-translator-3.0.0/dlg/dropmake/web/matrix_vis.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <!DOCTYPE html>
 <meta charset="utf-8">
+
 <head>
     <!-- <script src="http://d3js.org/d3.v3.min.js"></script> -->
     <script src="/static/d3.v3.min.js"></script>
     <script src="/static/jquery.min.js"></script>
     <script id="code">
         /*
         function loadGanttMatrix() {
@@ -11,68 +12,68 @@
         }
 
         function loadScheduleMatrix() {
           loadMatrix("pgt_schedule_mat");
         }
         */
 
-  function loadMatrix() {
-    //given a logical graph name, get its JSON from the server
-    //alert("Previous lg name = " + window.curr_lg_name);
-    //alert("Requesting " + pgtName.toString());
-    var action = "{{vis_action}}";
-    var gantt = false;
-    if (action == "pgt_gantt_chart") {
-      gantt = true;
-    }
-    $.ajax({
-      //url: "/pgt_gantt_chart?pgt_id={{pgt_view_json_name}}",
-      url: "/" + action.toString() + "?pgt_id={{pgt_view_json_name}}",
-      //url: "/pgt_gantt_chart?pgt_id=lofar_cal1_pgt.graph",
-      type: 'get',
-      error: function(XMLHttpRequest, textStatus, errorThrown) {
-        alert('status:' + XMLHttpRequest.status + ', status text: ' + XMLHttpRequest.statusText);
-      },
-      success: function(data){
-        //console.log(data);
-        // show the matrix
-        var gm = JSON.parse(data)
-        var numrows = gm.length;
-        var numcols = gm[0].length;
-        var matrix = new Array(numrows);
-        var min = Number.MAX_SAFE_INTEGER;
-        var max = -1;
-        for (var i = 0; i < numrows; i++) {
-          matrix[i] = new Array(numcols);
-          for (var j = 0; j < numcols; j++) {
-            var t = gm[i][j];
-            if (gantt && t == 1) {
-              t = i;
-            }
-            if (t < min) {
-              min = t;
-            }
-            if (t > max) {
-              max = t;
-            }
-            matrix[i][j] = t;
-          }
+        function loadMatrix() {
+            //given a logical graph name, get its JSON from the server
+            //alert("Previous lg name = " + window.curr_lg_name);
+            //alert("Requesting " + pgtName.toString());
+            var action = "{{vis_action}}";
+            var gantt = false;
+            if (action == "pgt_gantt_chart") {
+                gantt = true;
+            }
+            $.ajax({
+                //url: "/pgt_gantt_chart?pgt_id={{pgt_view_json_name}}",
+                url: "/" + action.toString() + "?pgt_id={{pgt_view_json_name}}",
+                //url: "/pgt_gantt_chart?pgt_id=lofar_cal1_pgt.graph",
+                type: 'get',
+                error: function (XMLHttpRequest, textStatus, errorThrown) {
+                    alert('status:' + XMLHttpRequest.status + ', status text: ' + XMLHttpRequest.statusText);
+                },
+                success: function (data) {
+                    //console.log(data);
+                    // show the matrix
+                    var gm = JSON.parse(data)
+                    var numrows = gm.length;
+                    var numcols = gm[0].length;
+                    var matrix = new Array(numrows);
+                    var min = Number.MAX_SAFE_INTEGER;
+                    var max = -1;
+                    for (var i = 0; i < numrows; i++) {
+                        matrix[i] = new Array(numcols);
+                        for (var j = 0; j < numcols; j++) {
+                            var t = gm[i][j];
+                            if (gantt && t == 1) {
+                                t = i;
+                            }
+                            if (t < min) {
+                                min = t;
+                            }
+                            if (t > max) {
+                                max = t;
+                            }
+                            matrix[i][j] = t;
+                        }
+                    }
+                    var colorMap = d3.scale.linear()
+                        //var colorMap = d3.scale.log()
+                        //.domain([-1, 0, 1])
+                        .domain([min, Math.round((min + max) / 2), max])
+                        //.domain([min, max])
+                        .range(["white", "blue", "red"]);
+                    //.range(["red", "black", "green"]);
+                    //.range(["brown", "#ddd", "darkgreen"]);
+                    showMatrix(numrows, numcols, matrix, colorMap);
+                }
+            });
         }
-        var colorMap = d3.scale.linear()
-        //var colorMap = d3.scale.log()
-            //.domain([-1, 0, 1])
-            .domain([min, Math.round((min + max) / 2), max])
-            //.domain([min, max])
-            .range(["white", "blue", "red"]);
-            //.range(["red", "black", "green"]);
-            //.range(["brown", "#ddd", "darkgreen"]);
-        showMatrix(numrows, numcols, matrix, colorMap);
-      }
-    });
-}
 
         function init() {
             /*
             var numrows = 15;
             var numcols = 10;
             var matrix = new Array(numrows);
             for (var i = 0; i < numrows; i++) {
@@ -85,15 +86,15 @@
             */
             //loadGanttMatrix();
             loadMatrix();
         }
 
         function showMatrix(numrows, numcols, matrix, colorMap) {
 
-            var margin = {top: 100, right: 100, bottom: 100, left: 100},
+            var margin = { top: 100, right: 100, bottom: 100, left: 100 },
                 width = 1024,
                 height = 768;
 
             var svg = d3.select("body").append("svg")
                 .attr("width", width + margin.left + margin.right)
                 .attr("height", height + margin.top + margin.bottom)
                 .style("margin-left", -margin.left + "px")
@@ -191,10 +192,11 @@
                 })
                 .style("fill", colorMap);
 
         }
 
     </script>
 </head>
+
 <body onload="init()">
 
-</body>
+</body>
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/pg_viewer.html` & `daliuge-translator-3.0.0/dlg/dropmake/web/pg_viewer.html`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/pure-min.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/pure-min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/FileSaver.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/FileSaver.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/d3.v5.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/dagre-d3.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/dagre-d3.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/d3/dagre-d3.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/d3/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/data_prep.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/data_prep.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/echarts-dagre.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/echarts-dagre.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.eot`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/fonts/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/html2canvas.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/liu.svg` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/liu.svg`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/liuFavIcon.svg` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/liuFavIcon.svg`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/settings_white_24dp.svg` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/settings_white_24dp.svg`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/icons/translate_green.png` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/icons/translate_green.png`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/jquery-ui.min.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/jquery.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/jquery.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/canteen.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/canteen.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/caseFrame.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/caseFrame.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/caseFrame.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/caseFrame.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/config.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/config.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/countup.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/countup.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/dat.gui.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/dat.gui.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/draggable.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/draggable.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecSimpleOptionPlayer.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecSimpleTransform.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecSimpleTransform.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecStat-1.1.1.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/ecStat.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/ecStat.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/echarts-dagre.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/echarts-dagre.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/echarts.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/echarts.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/esl.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/esl.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/facePrint.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/facePrint.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/fflate/index.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/fflate/index.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/frameInsight.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/frameInsight.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/jquery.min.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/perlin.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/perlin.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/rearrange.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/rearrange.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/require.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/require.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/requireES.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/requireES.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/reset.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/reset.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/rollup.browser.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/rollup.browser.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/lib/testHelper.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/lib/testHelper.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/main.css` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/main.css`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/src/require.js` & `daliuge-translator-3.0.0/dlg/dropmake/web/src/require.js`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/translator_rest.py` & `daliuge-translator-3.0.0/dlg/dropmake/web/translator_rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,35 +34,62 @@
 from enum import Enum
 from json import JSONDecodeError
 from typing import Union
 from urllib.parse import urlparse
 
 import uvicorn
 from fastapi import FastAPI, Request, Body, Query, HTTPException, Form
-from fastapi.responses import HTMLResponse, StreamingResponse, JSONResponse, RedirectResponse
+from fastapi.responses import (
+    HTMLResponse,
+    StreamingResponse,
+    JSONResponse,
+    RedirectResponse,
+)
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from jsonschema import validate, ValidationError
 from pydantic import BaseModel
 
 import dlg.constants
 import dlg.dropmake.pg_generator
 from dlg import restutils, common
 from dlg.clients import CompositeManagerClient
-from dlg.common.reproducibility.constants import REPRO_DEFAULT, ALL_RMODES, ReproducibilityFlags
-from dlg.common.reproducibility.reproducibility import init_lgt_repro_data, init_lg_repro_data, \
-    init_pgt_partition_repro_data, init_pgt_unroll_repro_data, init_pg_repro_data
+from dlg.common.reproducibility.constants import (
+    REPRO_DEFAULT,
+    ALL_RMODES,
+    ReproducibilityFlags,
+)
+from dlg.common.reproducibility.reproducibility import (
+    init_lgt_repro_data,
+    init_lg_repro_data,
+    init_pgt_partition_repro_data,
+    init_pgt_unroll_repro_data,
+    init_pg_repro_data,
+)
+
+from dlg import utils
 from dlg.common.deployment_methods import DeploymentMethods
 from dlg.common.k8s_utils import check_k8s_env
 from dlg.dropmake.lg import GraphException
 from dlg.dropmake.pg_manager import PGManager
 from dlg.dropmake.scheduler import SchedulerException
-from dlg.dropmake.web.translator_utils import file_as_string, lg_repo_contents, lg_path, lg_exists, \
-    pgt_exists, pgt_path, pgt_repo_contents, prepare_lgt, unroll_and_partition_with_params, \
-    make_algo_param_dict, get_mgr_deployment_methods, parse_mgr_url
+from dlg.dropmake.web.translator_utils import (
+    file_as_string,
+    lg_repo_contents,
+    lg_path,
+    lg_exists,
+    pgt_exists,
+    pgt_path,
+    pgt_repo_contents,
+    prepare_lgt,
+    unroll_and_partition_with_params,
+    make_algo_param_dict,
+    get_mgr_deployment_methods,
+    parse_mgr_url,
+)
 
 APP_DESCRIPTION = """
 DALiuGE LG Web interface translates and deploys logical graphs.
 
 The interface is split into two parts, refer to the main DALiuGE documentation 
 [DALiuGE documentation](https://daliuge.readthedocs.io/) for more information
 
@@ -74,79 +101,94 @@
 than query parameters.
 
 However, a new API for deployment is yet to be implemented
 
 Original author: chen.wu@icrar.org
 """
 APP_TAGS_METADATA = [
-    {"name": "Original", "description": "The original DALiuGE LG_web endpoints."},
-    {"name": "Updated", "description": "The new post-centric style mirror of CLI interface."}
+    {
+        "name": "Original",
+        "description": "The original DALiuGE LG_web endpoints.",
+    },
+    {
+        "name": "Updated",
+        "description": "The new post-centric style mirror of CLI interface.",
+    },
 ]
 
 file_location = pathlib.Path(__file__).parent.absolute()
 templates = Jinja2Templates(directory=file_location)
 
 app = FastAPI(
     title="DALiuGE LG Web Interface",
     description=APP_DESCRIPTION,
     openapi_tags=APP_TAGS_METADATA,
-    contact={
-        "name": "pritchardn",
-        "email": "nicholas.pritchard@icrar.org"
-    },
+    contact={"name": "pritchardn", "email": "nicholas.pritchard@icrar.org"},
     version=dlg.version.version,
     license_info={
         "name": "LGPLv2+",
-        "url": "https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html"
-    }
+        "url": "https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html",
+    },
 )
 app.mount("/static", StaticFiles(directory=file_location), name="static")
 logger = logging.getLogger(__name__)
 
 post_sem = threading.Semaphore(1)
 gen_pgt_sem = threading.Semaphore(1)
 
 global lg_dir
 global pgt_dir
 global pg_mgr
-LG_SCHEMA = json.loads(file_as_string("lg.graph.schema", package="dlg.dropmake"))
+LG_SCHEMA = json.loads(
+    file_as_string("lg.graph.schema", package="dlg.dropmake")
+)
 
 
 @app.post("/jsonbody", tags=["Original"])
 def jsonbody_post_lg(
-        lg_name: str = Form(description="The name of the lg to use"),
-        lg_content: str = Form(description="The content of the lg to save to file"),
-        rmode: str = Form(default=str(REPRO_DEFAULT.value)),
+    lg_name: str = Form(description="The name of the lg to use"),
+    lg_content: str = Form(
+        description="The content of the lg to save to file"
+    ),
+    rmode: str = Form(default=str(REPRO_DEFAULT.value)),
 ):
     """
     Post a logical graph JSON.
     """
     if not lg_exists(lg_dir, lg_name):
-        raise HTTPException(status_code=404,
-                            detail="Creating new graphs through this API is not supported")
+        raise HTTPException(
+            status_code=404,
+            detail="Creating new graphs through this API is not supported",
+        )
     try:
         lg_content = json.loads(lg_content)
     except JSONDecodeError:
         logger.warning("Could not decode lgt %s", lg_name)
     lg_content = init_lgt_repro_data(lg_content, rmode)
     lg_path = pathlib.Path(lg_dir, lg_name)
     post_sem.acquire()
     try:
         with open(lg_path, "w") as lg_file:
             lg_file.write(json.dumps(lg_content))
     except Exception as e:
-        raise HTTPException(status_code=500,
-                            detail="Failed to save logical graph {0}:{1}".format(lg_name, str(e)))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to save logical graph {0}:{1}".format(
+                lg_name, str(e)
+            ),
+        )
     finally:
         post_sem.release()
 
 
 @app.get("/jsonbody", tags=["Original"])
 def jsonbody_get_lg(
-        lg_name: str = Query(default=None, description="The name of the lg to load from file")
+    lg_name: str = Query(
+        default=None, description="The name of the lg to load from file"
+    )
 ):
     """
     Returns JSON representation of saved logical graph.
     """
     if lg_name is None or len(lg_name) == 0:
         all_lgs = lg_repo_contents(lg_dir)
         try:
@@ -158,209 +200,294 @@
     if lg_exists(lg_dir, lg_name):
         # print "Loading {0}".format(name)
         lgp = lg_path(lg_dir, lg_name)
         with open(lgp, "r") as f:
             data = json.load(f)
         return JSONResponse(data)
     else:
-        raise HTTPException(status_code=404, detail="JSON graph {0} not found\n".format(lg_name))
+        raise HTTPException(
+            status_code=404,
+            detail="JSON graph {0} not found\n".format(lg_name),
+        )
 
 
 @app.get("/pgt_jsonbody", response_class=JSONResponse, tags=["Original"])
 def jsonbody_get_pgt(
-        pgt_name: str = Query(description="The name of the pgt to load from file")
+    pgt_name: str = Query(description="The name of the pgt to load from file"),
 ):
     """
     Return JSON representation of a physical graph template
     """
     if pgt_exists(pgt_dir, pgt_name):
         # print "Loading {0}".format(name)
         pgt = pgt_path(pgt_dir, pgt_name)
         with open(pgt, "r") as f:
             data = f.read()
         return JSONResponse(data)
     else:
-        raise HTTPException(status_code=404, detail="JSON graph {0} not found".format(pgt_name))
+        raise HTTPException(
+            status_code=404, detail="JSON graph {0} not found".format(pgt_name)
+        )
 
 
 @app.get("/pg_viewer", response_class=HTMLResponse, tags=["Original"])
-def load_pg_viewer(request: Request,
-                   pgt_view_name: str = Query(default=None,
-                                              description="The string of the type of view to provide")
-                   ):
+def load_pg_viewer(
+    request: Request,
+    pgt_view_name: str = Query(
+        default=None, description="The string of the type of view to provide"
+    ),
+):
     """
     Loads the physical graph viewer
     """
     if pgt_view_name is None or len(pgt_view_name) == 0:
         all_pgts = pgt_repo_contents(pgt_dir)
         try:
             first_dir = next(iter(all_pgts))
             pgt_view_name = first_dir + os.sep + all_pgts[first_dir][0]
         except StopIteration:
             pgt_view_name = None
     if pgt_exists(pgt_dir, pgt_view_name):
-        tpl = templates.TemplateResponse("pg_viewer.html", {
-            "request": request,
-            "pgt_view_json_name": pgt_view_name,
-            "partition_info": None,
-            "title": "Physical Graph Template",
-            "error": None
-        })
+        tpl = templates.TemplateResponse(
+            "pg_viewer.html",
+            {
+                "request": request,
+                "pgt_view_json_name": pgt_view_name,
+                "partition_info": None,
+                "title": "Physical Graph Template",
+                "error": None,
+            },
+        )
         return tpl
     else:
-        raise HTTPException(status_code=404,
-                            detail="Physical graph template view {0} not found {1}".format(
-                                pgt_view_name, pgt_dir))
+        raise HTTPException(
+            status_code=404,
+            detail="Physical graph template view {0} not found {1}".format(
+                pgt_view_name, pgt_dir
+            ),
+        )
 
 
 @app.get("/show_gantt_chart", response_class=HTMLResponse, tags=["Original"])
 def show_gantt_chart(
-        request: Request,
-        pgt_id: str = Query(description="The pgt_id used to internally reference this graph")
+    request: Request,
+    pgt_id: str = Query(
+        description="The pgt_id used to internally reference this graph"
+    ),
 ):
     """
     Interface to show the gantt chart
     """
-    tpl = templates.TemplateResponse("matrix_vis.html", {
-        "request": request,
-        "pgt_view_json_name": pgt_id,
-        "vis_action": "pgt_gantt_chart"
-    })
+    tpl = templates.TemplateResponse(
+        "matrix_vis.html",
+        {
+            "request": request,
+            "pgt_view_json_name": pgt_id,
+            "vis_action": "pgt_gantt_chart",
+        },
+    )
     return tpl
 
 
 @app.get("/pgt_gantt_chart", tags=["Original"])
 def get_gantt_chart(
-        pgt_id: str = Query(description="The pgt_id used to internally reference this graph")
+    pgt_id: str = Query(
+        description="The pgt_id used to internally reference this graph"
+    ),
 ):
     """
     Interface to retrieve a Gantt Chart matrix associated with a PGT
     """
     try:
         ret = pg_mgr.get_gantt_chart(pgt_id)
         return ret
     except GraphException as ge:
-        raise HTTPException(status_code=500, detail="Failed to generate Gantt chart for {0}: {1}"
-                            .format(pgt_id, ge))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to generate Gantt chart for {0}: {1}".format(
+                pgt_id, ge
+            ),
+        )
 
 
 @app.get("/show_schedule_mat", response_class=HTMLResponse, tags=["Original"])
 def show_schedule_matrix(
-        request: Request,
-        pgt_id: str = Query(description="The pgt_id used to internally reference this graph")
+    request: Request,
+    pgt_id: str = Query(
+        description="The pgt_id used to internally reference this graph"
+    ),
 ):
     """
     Interface to show the schedule mat
     """
-    tpl = templates.TemplateResponse("matrix_vis.html", {
-        "request": request,
-        "pgt_view_json_name": pgt_id,
-        "vis_action": "pgt_schedule_mat"
-    })
+    tpl = templates.TemplateResponse(
+        "matrix_vis.html",
+        {
+            "request": request,
+            "pgt_view_json_name": pgt_id,
+            "vis_action": "pgt_schedule_mat",
+        },
+    )
     return tpl
 
 
 @app.get("/get_schedule_matrices", tags=["Original"])
 def get_schedule_matrices(
-        pgt_id: str = Query(description="The pgt_id used to internally reference this graph")
+    pgt_id: str = Query(
+        description="The pgt_id used to internally reference this graph"
+    ),
 ):
     """
     Interface to return all schedule matrices for a single pgt_id
     """
     try:
         ret = pg_mgr.get_schedule_matrices(pgt_id)
         return ret
     except Exception as e:
-        raise HTTPException(status_code=500, detail="Failed to get schedule matrices for {0}: {1}"
-                            .format(pgt_id, e))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to get schedule matrices for {0}: {1}".format(
+                pgt_id, e
+            ),
+        )
 
 
 # ------ Graph deployment methods ------ #
 
+
 @app.get("/gen_pgt", tags=["Original"])
 def gen_pgt(
-        request: Request,
-        lg_name: str = Query(
-            description="If present, translator will attempt to load this lg from file"),
-        rmode: str = Query(default=str(REPRO_DEFAULT.value),
-                           description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information"),
-        test: str = Query(default="false",
-                          description="If 'true', will replace all apps with sleeps"),
-        num_par: int = Query(default=1, description="The number of data partitions in the graph"),
-        algo: str = Query(default="metis",
-                          description="The scheduling algorithm used when unrolling the graph"),
-        num_islands: int = Query(default=0, description="The number of data-islands to partition"),
-        par_label: str = Query(default="Partition",
-                               description="The label prefixed to each generated partition"),
+    request: Request,
+    lg_name: str = Query(
+        description="If present, translator will attempt to load this lg from file"
+    ),
+    rmode: str = Query(
+        default=str(REPRO_DEFAULT.value),
+        description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information",
+    ),
+    test: str = Query(
+        default="false",
+        description="If 'true', will replace all apps with sleeps",
+    ),
+    num_par: int = Query(
+        default=1, description="The number of data partitions in the graph"
+    ),
+    algo: str = Query(
+        default="metis",
+        description="The scheduling algorithm used when unrolling the graph",
+    ),
+    num_islands: int = Query(
+        default=0, description="The number of data-islands to partition"
+    ),
+    par_label: str = Query(
+        default="Partition",
+        description="The label prefixed to each generated partition",
+    ),
 ):
     if not lg_exists(lg_dir, lg_name):
-        raise HTTPException(status_code=404,
-                            detail="Logical graph '{0}' not found".format(lg_name))
+        raise HTTPException(
+            status_code=404,
+            detail="Logical graph '{0}' not found".format(lg_name),
+        )
     try:
         lgt = prepare_lgt(lg_path(lg_dir, lg_name), rmode)
         test = test.lower() == "true"
-        pgt = unroll_and_partition_with_params(lgt, test, algo, num_par, num_islands,
-                                               par_label, request.query_params.items())
+        pgt = unroll_and_partition_with_params(
+            lgt,
+            test,
+            algo,
+            num_par,
+            num_islands,
+            par_label,
+            request.query_params.items(),
+        )
         num_partitions = 0  # pgt._num_parts;
 
         pgt_id = pg_mgr.add_pgt(pgt, lg_name)
 
         part_info = " - ".join(
             ["{0}:{1}".format(k, v) for k, v in pgt.result().items()]
         )
-        tpl = templates.TemplateResponse("pg_viewer.html", {
-            "request": request,
-            "pgt_view_json_name": pgt_id,
-            "partition_info": part_info,
-            "title": "Physical Graph Template%s"
-                     % ("" if num_partitions == 0 else "Partitioning"),
-            "error": None
-        })
+        tpl = templates.TemplateResponse(
+            "pg_viewer.html",
+            {
+                "request": request,
+                "pgt_view_json_name": pgt_id,
+                "partition_info": part_info,
+                "title": "Physical Graph Template%s"
+                % ("" if num_partitions == 0 else "Partitioning"),
+                "error": None,
+            },
+        )
         return tpl
     except GraphException as ge:
         logger.info("Graph Exception")
-        raise HTTPException(status_code=500,
-                            detail="Invalid Logical Graph {1}: {0}".format(str(ge), lg_name))
+        raise HTTPException(
+            status_code=500,
+            detail="Invalid Logical Graph {1}: {0}".format(str(ge), lg_name),
+        )
     except SchedulerException as se:
         logger.info("Schedule Exception")
-        raise HTTPException(status_code=500,
-                            detail="Graph scheduling exception {1}: {0}".format(str(se), lg_name))
+        raise HTTPException(
+            status_code=500,
+            detail="Graph scheduling exception {1}: {0}".format(
+                str(se), lg_name
+            ),
+        )
     except Exception:
         logger.info("Partition / Other exception")
         trace_msg = traceback.format_exc()
-        raise HTTPException(status_code=500,
-                            detail="Graph partition exception {1}: {0}".format(trace_msg, lg_name))
+        raise HTTPException(
+            status_code=500,
+            detail="Graph partition exception {1}: {0}".format(
+                trace_msg, lg_name
+            ),
+        )
 
 
 @app.post("/gen_pgt", response_class=HTMLResponse, tags=["Original"])
 async def gen_pgt_post(
-        request: Request,
-        lg_name: str = Form(
-            description="If present, translator will attempt to load this lg from file"),
-        json_data: str = Form(description="The graph data used as the graph if supplied"),
-        rmode: str = Form(str(REPRO_DEFAULT.value),
-                          description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information"),
-        test: str = Form(default="false",
-                         description="If 'true', will replace all apps with sleeps"),
-        algo: str = Form(default="metis",
-                         description="The scheduling algorithm used when unrolling the graph"),
-        num_par: int = Form(default=1, description="The number of data partitions in the graph"),
-        num_islands: int = Form(default=0, description="The number of data-islands to partition"),
-        par_label: str = Form(default="Partition",
-                              description="The label prefixed to each generated partition"),
-        min_goal: Union[int, None] = Form(default=None),
-        ptype: Union[int, None] = Form(default=None),
-        max_load_imb: Union[int, None] = Form(default=None),
-        max_cpu: Union[int, None] = Form(default=None),
-        time_greedy: Union[int, None] = Form(default=None),
-        deadline: Union[int, None] = Form(default=None),
-        topk: Union[int, None] = Form(default=None),
-        swarm_size: Union[int, None] = Form(default=None),
-        max_mem: Union[int, None] = Form(default=None)
-
+    request: Request,
+    lg_name: str = Form(
+        description="If present, translator will attempt to load this lg from file"
+    ),
+    json_data: str = Form(
+        description="The graph data used as the graph if supplied"
+    ),
+    rmode: str = Form(
+        str(REPRO_DEFAULT.value),
+        description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information",
+    ),
+    test: str = Form(
+        default="false",
+        description="If 'true', will replace all apps with sleeps",
+    ),
+    algo: str = Form(
+        default="metis",
+        description="The scheduling algorithm used when unrolling the graph",
+    ),
+    num_par: int = Form(
+        default=1, description="The number of data partitions in the graph"
+    ),
+    num_islands: int = Form(
+        default=0, description="The number of data-islands to partition"
+    ),
+    par_label: str = Form(
+        default="Partition",
+        description="The label prefixed to each generated partition",
+    ),
+    min_goal: Union[int, None] = Form(default=None),
+    ptype: Union[int, None] = Form(default=None),
+    max_load_imb: Union[int, None] = Form(default=None),
+    max_cpu: Union[int, None] = Form(default=None),
+    time_greedy: Union[int, None] = Form(default=None),
+    deadline: Union[int, None] = Form(default=None),
+    topk: Union[int, None] = Form(default=None),
+    swarm_size: Union[int, None] = Form(default=None),
+    max_mem: Union[int, None] = Form(default=None),
 ):
     """
     Translating Logical Graphs to Physical Graphs.
     Differs from get_pgt above by the fact that the logical graph data is POSTed
     to this route in a HTTP form, whereas gen_pgt loads the logical graph data
     from a local file
     """
@@ -372,79 +499,123 @@
         except ValidationError as ve:
             error = "Validation Error {1}: {0}".format(str(ve), lg_name)
             logger.error(error)
             # raise HTTPException(status_code=500, detail=error)
         logical_graph = prepare_lgt(logical_graph, rmode)
         # LG -> PGT
         # TODO: Warning: I dislike doing it this way with a passion, however without changing the tests/ usage of the api getting all form fields is difficult.
-        algo_params = make_algo_param_dict(min_goal, ptype, max_load_imb, max_cpu, time_greedy,
-                                           deadline, topk, swarm_size, max_mem)
-        pgt = unroll_and_partition_with_params(logical_graph, test, algo, num_par,
-                                               num_islands, par_label, algo_params)
+        algo_params = make_algo_param_dict(
+            min_goal,
+            ptype,
+            max_load_imb,
+            max_cpu,
+            time_greedy,
+            deadline,
+            topk,
+            swarm_size,
+            max_mem,
+        )
+        pgt = unroll_and_partition_with_params(
+            logical_graph,
+            test,
+            algo,
+            num_par,
+            num_islands,
+            par_label,
+            algo_params,
+        )
         pgt_id = pg_mgr.add_pgt(pgt, lg_name)
         part_info = " - ".join(
             ["{0}:{1}".format(k, v) for k, v in pgt.result().items()]
         )
-        tpl = templates.TemplateResponse("pg_viewer.html", {
-            "request": request,
-            "pgt_view_json_name": pgt_id,
-            "partition_info": part_info,
-            "title": "Physical Graph Template%s"
-                     % ("" if num_par == 0 else "Partitioning"),
-            "error": None
-        })
+        tpl = templates.TemplateResponse(
+            "pg_viewer.html",
+            {
+                "request": request,
+                "pgt_view_json_name": pgt_id,
+                "partition_info": part_info,
+                "title": "Physical Graph Template%s"
+                % ("" if num_par == 0 else "Partitioning"),
+                "error": None,
+            },
+        )
         return tpl
     except GraphException as ge:
         logger.info("GRAPH EXCEPTION")
-        raise HTTPException(status_code=500,
-                            detail="Invalid Logical Graph {1}: {0}".format(str(ge), lg_name))
+        raise HTTPException(
+            status_code=500,
+            detail="Invalid Logical Graph {1}: {0}".format(str(ge), lg_name),
+        )
     except SchedulerException as se:
         logger.info("SCHEDULE EXCEPTION")
-        raise HTTPException(status_code=500,
-                            detail="Graph scheduling exception {1}: {0}".format(str(se), lg_name))
+        raise HTTPException(
+            status_code=500,
+            detail="Graph scheduling exception {1}: {0}".format(
+                str(se), lg_name
+            ),
+        )
     except Exception:
         logger.info("OTHER EXCEPTION")
         trace_msg = traceback.format_exc()
-        raise HTTPException(status_code=500,
-                            detail="Graph partition exception {1}: {0}".format(trace_msg, lg_name))
+        raise HTTPException(
+            status_code=500,
+            detail="Graph partition exception {1}: {0}".format(
+                trace_msg, lg_name
+            ),
+        )
 
 
 @app.get("/gen_pg", response_class=JSONResponse, tags=["Original"])
 def gen_pg(
-        request: Request,
-        pgt_id: str = Query(description="The pgt_id used to internally reference this graph"),
-        dlg_mgr_deploy: Union[str, None] = Query(default=None,
-                                                 description="If supplied, this endpoint will attempt to deploy the graph is the dlg_pgt_url or dlg_mgr_host/port endpoint"),
-        dlg_mgr_url: Union[str, None] = Query(default=None,
-                                              description="The DALiuGE manager to deploy the graph to"),
-        dlg_mgr_host: Union[str, None] = Query(default=None,
-                                               description="The DALiuGE manager base IP to deploy the graph to"),
-        dlg_mgr_port: Union[int, None] = Query(default=None,
-                                               description="The DALiuGE manager port to deploy the graph to"),
-        tpl_nodes_len: int = Query(default=0,
-                                   description="The number of nodes to unroll the graph partition for")
+    request: Request,
+    pgt_id: str = Query(
+        description="The pgt_id used to internally reference this graph"
+    ),
+    dlg_mgr_deploy: Union[str, None] = Query(
+        default=None,
+        description="If supplied, this endpoint will attempt to deploy the graph is the dlg_pgt_url or dlg_mgr_host/port endpoint",
+    ),
+    dlg_mgr_url: Union[str, None] = Query(
+        default=None, description="The DALiuGE manager to deploy the graph to"
+    ),
+    dlg_mgr_host: Union[str, None] = Query(
+        default=None,
+        description="The DALiuGE manager base IP to deploy the graph to",
+    ),
+    dlg_mgr_port: Union[int, None] = Query(
+        default=None,
+        description="The DALiuGE manager port to deploy the graph to",
+    ),
+    tpl_nodes_len: int = Query(
+        default=0,
+        description="The number of nodes to unroll the graph partition for",
+    ),
 ):
     """
     RESTful interface to convert a PGT(P) into PG by mapping
     PGT(P) onto a given set of available resources
     """
     # if the 'deploy' checkbox is not checked,
     # then the form submission will NOT contain a 'dlg_mgr_deploy' field
     deploy = dlg_mgr_deploy is not None
     mprefix = ""
     pgtp = pg_mgr.get_pgt(pgt_id)
     if pgtp is None:
-        raise HTTPException(status_code=404,
-                            detail="PGT(P) with id {0} not found in the Physical Graph Manager"
-                            .format(pgt_id))
+        raise HTTPException(
+            status_code=404,
+            detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
+                pgt_id
+            ),
+        )
 
     pgtpj = pgtp._gojs_json_obj
     reprodata = pgtp.reprodata
-    logger.info("PGTP: %s", pgtpj)
-    num_partitions = len(list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"])))
+    num_partitions = len(
+        list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"]))
+    )
     mport = 443
     if dlg_mgr_url is not None:
         mparse = urlparse(dlg_mgr_url)
         try:
             (mhost, mport) = mparse.netloc.split(":")
             mport = int(mport)
         except:
@@ -467,16 +638,18 @@
     logger.debug("Manager port: %s", mport)
     logger.debug("Manager prefix: %s", mprefix)
 
     if mhost is None:
         if tpl_nodes_len > 0:
             nnodes = num_partitions
         else:
-            raise HTTPException(status_code=500,
-                                detail="Must specify DALiuGE manager host or tpl_nodes_len")
+            raise HTTPException(
+                status_code=500,
+                detail="Must specify DALiuGE manager host or tpl_nodes_len",
+            )
 
         pg_spec = pgtp.to_pg_spec([], ret_str=False, tpl_nodes_len=nnodes)
         pg_spec.append(reprodata)
         return JSONResponse(pg_spec)
     try:
         mgr_client = CompositeManagerClient(
             host=mhost, port=mport, url_prefix=mprefix, timeout=30
@@ -497,105 +670,142 @@
             pg_spec.append(reprodata)
             mgr_client.append_graph(ssid, pg_spec)
             # print "graph appended"
             mgr_client.deploy_session(ssid, completed_uids=completed_uids)
             # mgr_client.deploy_session(ssid, completed_uids=[])
             # print "session deployed"
             # 3. redirect to the master drop manager
-            return RedirectResponse("http://{0}:{1}{2}/session?sessionId={3}".format(
-                mhost, mport, mprefix, ssid
-            ))
+            return RedirectResponse(
+                "http://{0}:{1}{2}/session?sessionId={3}".format(
+                    mhost, mport, mprefix, ssid
+                )
+            )
         else:
             return JSONResponse(pg_spec)
     except restutils.RestClientException as re:
-        raise HTTPException(status_code=500,
-                            detail="Failed to interact with DALiUGE Drop Manager: {0}".format(re))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to interact with DALiUGE Drop Manager: {0}".format(
+                re
+            ),
+        )
     except Exception as ex:
         logger.error(traceback.format_exc())
-        raise HTTPException(status_code=500,
-                            detail="Failed to deploy physical graph: {0}".format(ex))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to deploy physical graph: {0}".format(ex),
+        )
 
 
 @app.get("/gen_pg_spec", tags=["Original"])
 def gen_pg_spec(
-        pgt_id: str = Body(description="The pgt_id used to internally reference this graph"),
-        node_list: list = Body(default=[],
-                               description="The list of daliuge nodes to submit the graph to"),
-        manager_host: str = Body(
-            description="The address of the manager host where the graph will be deployed to."),
+    pgt_id: str = Body(
+        description="The pgt_id used to internally reference this graph"
+    ),
+    node_list: list = Body(
+        default=[],
+        description="The list of daliuge nodes to submit the graph to",
+    ),
+    manager_host: str = Body(
+        description="The address of the manager host where the graph will be deployed to."
+    ),
 ):
     """
     Interface to convert a PGT(P) into pg_spec
     """
     try:
         if manager_host == "localhost":
             manager_host = "localhost"
         logger.debug("pgt_id: %s", str(pgt_id))
         logger.debug("node_list: %s", str(node_list))
     except Exception as ex:
         logger.error("%s", traceback.format_exc())
-        raise HTTPException(status_code=500,
-                            detail="Unable to parse json body of request for pg_spec: {0}".format(
-                                ex))
+        raise HTTPException(
+            status_code=500,
+            detail="Unable to parse json body of request for pg_spec: {0}".format(
+                ex
+            ),
+        )
     pgtp = pg_mgr.get_pgt(pgt_id)
     if pgtp is None:
-        raise HTTPException(status_code=404,
-                            detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
-                                pgt_id
-                            ))
+        raise HTTPException(
+            status_code=404,
+            detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
+                pgt_id
+            ),
+        )
     if node_list is None:
-        raise HTTPException(status_code=500, detail="Must specify DALiuGE nodes list")
+        raise HTTPException(
+            status_code=500, detail="Must specify DALiuGE nodes list"
+        )
 
     try:
         pg_spec = pgtp.to_pg_spec([manager_host] + node_list, ret_str=False)
         root_uids = common.get_roots(pg_spec)
-        response = StreamingResponse(json.dumps({"pg_spec": pg_spec, "root_uids": list(root_uids)}))
+        response = StreamingResponse(
+            json.dumps({"pg_spec": pg_spec, "root_uids": list(root_uids)})
+        )
         response.content_type = "application/json"
         return response
     except Exception as ex:
         logger.error("%s", traceback.format_exc())
-        raise HTTPException(status_code=500, detail="Failed to generate pg_spec: {0}".format(ex))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to generate pg_spec: {0}".format(ex),
+        )
 
 
 @app.get("/gen_pg_helm", tags=["Original"])
 def gen_pg_helm(
-        pgt_id: str = Body(description="The pgt_id used to internally reference this graph")
+    pgt_id: str = Body(
+        description="The pgt_id used to internally reference this graph"
+    ),
 ):
     """
     Deploys a PGT as a K8s helm chart.
     """
     # Get pgt_data
     from ...deploy.start_helm_cluster import start_helm
+
     pgtp = pg_mgr.get_pgt(pgt_id)
     if pgtp is None:
-        raise HTTPException(status_code=404,
-                            detail="PGT(P) with id {0} not found in the Physical Graph Manager"
-                            .format(pgt_id))
+        raise HTTPException(
+            status_code=404,
+            detail="PGT(P) with id {0} not found in the Physical Graph Manager".format(
+                pgt_id
+            ),
+        )
 
     pgtpj = pgtp._gojs_json_obj
     logger.info("PGTP: %s", pgtpj)
-    num_partitions = len(list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"])))
+    num_partitions = len(
+        list(filter(lambda n: "isGroup" in n, pgtpj["nodeDataArray"]))
+    )
     # Send pgt_data to helm_start
     try:
         start_helm(pgtp, num_partitions, pgt_dir)
     except restutils.RestClientException as ex:
         logger.error(traceback.format_exc())
-        raise HTTPException(status_code=500,
-                            detail="Failed to deploy physical graph: {0}".format(ex))
+        raise HTTPException(
+            status_code=500,
+            detail="Failed to deploy physical graph: {0}".format(ex),
+        )
     # TODO: Not sure what to redirect to yet
     return "Inspect your k8s dashboard for deployment status"
 
 
 # ------ Methods from translator CLI ------ #
 
+
 class AlgoParams(BaseModel):
     """
     Set of scheduling algorithm parameters, not all apply to all algorithms.
     Refer to main documentation for more information.
     """
+
     min_goal: Union[int, None]
     ptype: Union[int, None]
     max_load_imb: Union[int, None]
     max_cpu: Union[int, None]
     time_greedy: Union[int, None]
     deadline: Union[int, None]
     topk: Union[int, None]
@@ -604,236 +814,331 @@
 
 
 class KnownAlgorithms(str, Enum):
     """
     List of known scheduling algorithms.
     Will need to be updated manually.
     """
-    ALGO_NONE = "none",
-    ALGO_METIS = "metis",
-    ALGO_MY_SARKAR = "mysarkar",
-    ALGO_MIN_NUM_PARTS = "min_num_parts",
+
+    ALGO_NONE = ("none",)
+    ALGO_METIS = ("metis",)
+    ALGO_MY_SARKAR = ("mysarkar",)
+    ALGO_MIN_NUM_PARTS = ("min_num_parts",)
     ALGO_PSO = "pso"
 
 
 def load_graph(graph_content: str, graph_name: str):
     out_graph = {}
     if graph_content is not None and graph_name is not None:
-        raise HTTPException(status_code=400,
-                            detail="Need to supply either an name or content but not both")
+        raise HTTPException(
+            status_code=400,
+            detail="Need to supply either an name or content but not both",
+        )
     if not lg_exists(lg_dir, graph_name):
         if not graph_content:
-            raise HTTPException(status_code=400, detail="LG content is nonexistent")
+            raise HTTPException(
+                status_code=400, detail="LG content is nonexistent"
+            )
         else:
             try:
                 out_graph = json.loads(graph_content)
             except JSONDecodeError as jerror:
                 logger.error(jerror)
-                raise HTTPException(status_code=400,
-                                    detail="LG content is malformed")
+                raise HTTPException(
+                    status_code=400, detail="LG content is malformed"
+                )
     else:
         lgp = lg_path(lg_dir, graph_name)
         with open(lgp, "r") as f:
             try:
                 out_graph = json.load(f)
             except JSONDecodeError as jerror:
                 logger.error(jerror)
-                raise HTTPException(status_code=500,
-                                    detail="LG graph on file cannot be loaded")
+                raise HTTPException(
+                    status_code=500, detail="LG graph on file cannot be loaded"
+                )
     return out_graph
 
 
 @app.post("/lg_fill", response_class=JSONResponse, tags=["Updated"])
 def lg_fill(
-        lg_name: str = Form(default=None,
-                            description="If present, translator will attempt to load this lg from file"),
-        lg_content: str = Form(default=None,
-                               description="If present, translator will use this string as the graph content"),
-        parameters: str = Form(default="{}", description="JSON key: value store of graph paramter"),
-        rmode: str = Form(REPRO_DEFAULT.name, enum=[roption.name for roption in
-                                                    [ReproducibilityFlags.NOTHING] + ALL_RMODES],
-                          description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information")
+    lg_name: str = Form(
+        default=None,
+        description="If present, translator will attempt to load this lg from file",
+    ),
+    lg_content: str = Form(
+        default=None,
+        description="If present, translator will use this string as the graph content",
+    ),
+    parameters: str = Form(
+        default="{}", description="JSON key: value store of graph paramter"
+    ),
+    rmode: str = Form(
+        REPRO_DEFAULT.name,
+        enum=[
+            roption.name
+            for roption in [ReproducibilityFlags.NOTHING] + ALL_RMODES
+        ],
+        description="Reproducibility mode setting level of provenance tracking. Refer to main documentation for more information",
+    ),
 ):
     """
     Will fill a logical graph by replacing fields with supplied parameters.
 
     One of lg_name or lg_content, but not both, must be specified.
     """
     lg_graph = load_graph(lg_content, lg_name)
     try:
         params = json.loads(parameters)
     except JSONDecodeError as jerror:
         logger.error(jerror)
-        raise HTTPException(status_code=400,
-                            detail="Parameter string is invalid")
+        raise HTTPException(
+            status_code=400, detail="Parameter string is invalid"
+        )
     output_graph = dlg.dropmake.pg_generator.fill(lg_graph, params)
     output_graph = init_lg_repro_data(init_lgt_repro_data(output_graph, rmode))
     return JSONResponse(output_graph)
 
 
 @app.post("/unroll", response_class=JSONResponse, tags=["Updated"])
 def lg_unroll(
-        lg_name: str = Form(default=None,
-                            description="If present, translator will attempt to load this lg from file"),
-        lg_content: str = Form(default=None,
-                               description="If present, translator will use this string as the graph content"),
-        oid_prefix: str = Form(default=None, description="ID prefix appended to unrolled nodes"),
-        zero_run: bool = Form(default=None,
-                              description="If true, apps will be replaced with sleep apps"),
-        default_app: str = Form(default=None,
-                                description="If set, will change all apps to this app class"),
+    lg_name: str = Form(
+        default=None,
+        description="If present, translator will attempt to load this lg from file",
+    ),
+    lg_content: str = Form(
+        default=None,
+        description="If present, translator will use this string as the graph content",
+    ),
+    oid_prefix: str = Form(
+        default=None, description="ID prefix appended to unrolled nodes"
+    ),
+    zero_run: bool = Form(
+        default=None,
+        description="If true, apps will be replaced with sleep apps",
+    ),
+    default_app: str = Form(
+        default=None,
+        description="If set, will change all apps to this app class",
+    ),
 ):
     """
     Will unroll a logical graph into a physical graph template.
 
     One of lg_name or lg_content, but not both, needs to be specified.
     """
     lg_graph = load_graph(lg_content, lg_name)
-    pgt = dlg.dropmake.pg_generator.unroll(lg_graph, oid_prefix, zero_run, default_app)
+    pgt = dlg.dropmake.pg_generator.unroll(
+        lg_graph, oid_prefix, zero_run, default_app
+    )
     pgt = init_pgt_unroll_repro_data(pgt)
     return JSONResponse(pgt)
 
 
 @app.post("/partition", response_class=JSONResponse, tags=["Updated"])
 def pgt_partition(
-        pgt_name: str = Form(default=None,
-                             description="If specified, translator will attempt to load graph from file"),
-        pgt_content: str = Form(default=None,
-                                description="If present, translator will use this string as the graph content"),
-        num_partitions: int = Form(default=1,
-                                   description="Number of partitions to unroll the graph across"),
-        num_islands: int = Form(default=1, description="Number of data islands to partition for"),
-        algorithm: KnownAlgorithms = Form(default="metis",
-                                          description="The selected scheduling algorithm"),
-        algo_params: AlgoParams = Form(default=AlgoParams(),
-                                       description="The parameter values passed to the scheduling algorithm. Required parameters varies per algorithm.")
+    pgt_name: str = Form(
+        default=None,
+        description="If specified, translator will attempt to load graph from file",
+    ),
+    pgt_content: str = Form(
+        default=None,
+        description="If present, translator will use this string as the graph content",
+    ),
+    num_partitions: int = Form(
+        default=1,
+        description="Number of partitions to unroll the graph across",
+    ),
+    num_islands: int = Form(
+        default=1, description="Number of data islands to partition for"
+    ),
+    algorithm: KnownAlgorithms = Form(
+        default="metis", description="The selected scheduling algorithm"
+    ),
+    algo_params: AlgoParams = Form(
+        default=AlgoParams(),
+        description="The parameter values passed to the scheduling algorithm. Required parameters varies per algorithm.",
+    ),
 ):
     """
     Uses scheduling algorithms to partition an unrolled pgt across several partitions and data islands.
 
     One of pgt_name or pgt_content, but not both, must be specified.
     """
     graph = load_graph(pgt_content, pgt_name)
     reprodata = {}
     if not graph[-1].get("oid"):
         reprodata = graph.pop()
-    pgt = dlg.dropmake.pg_generator.partition(graph, algorithm, num_partitions, num_islands,
-                                              algo_params.dict())
+    pgt = dlg.dropmake.pg_generator.partition(
+        graph, algorithm, num_partitions, num_islands, algo_params.dict()
+    )
     pgt.append(reprodata)
     pgt = init_pgt_partition_repro_data(pgt)
     return JSONResponse(pgt)
 
 
-@app.post("/unroll_and_partition", response_class=JSONResponse, tags=["Updated"])
+@app.post(
+    "/unroll_and_partition", response_class=JSONResponse, tags=["Updated"]
+)
 def lg_unroll_and_partition(
-        lg_name: str = Form(default=None,
-                            description="If present, translator will attempt to load this lg from file"),
-        lg_content: str = Form(default=None,
-                               description="If present, translator will use this string as the graph content"),
-        oid_prefix: str = Form(default=None, description="ID prefix appended to unrolled nodes"),
-        zero_run: bool = Form(default=None,
-                              description="If true, apps will be replaced with sleep apps"),
-        default_app: str = Form(default=None,
-                                description="If set, will change all apps to this app class"),
-        num_partitions: int = Form(default=1,
-                                   description="Number of partitions to unroll the graph across"),
-        num_islands: int = Form(default=1, description="Number of data islands to partition for"),
-        algorithm: KnownAlgorithms = Form(default="metis",
-                                          description="The selected scheduling algorithm"),
-        algo_params: AlgoParams = Form(default=AlgoParams(),
-                                       description="The parameter values passed to the scheduling algorithm. Required parameters varies per algorithm.")
+    lg_name: str = Form(
+        default=None,
+        description="If present, translator will attempt to load this lg from file",
+    ),
+    lg_content: str = Form(
+        default=None,
+        description="If present, translator will use this string as the graph content",
+    ),
+    oid_prefix: str = Form(
+        default=None, description="ID prefix appended to unrolled nodes"
+    ),
+    zero_run: bool = Form(
+        default=None,
+        description="If true, apps will be replaced with sleep apps",
+    ),
+    default_app: str = Form(
+        default=None,
+        description="If set, will change all apps to this app class",
+    ),
+    num_partitions: int = Form(
+        default=1,
+        description="Number of partitions to unroll the graph across",
+    ),
+    num_islands: int = Form(
+        default=1, description="Number of data islands to partition for"
+    ),
+    algorithm: KnownAlgorithms = Form(
+        default="metis", description="The selected scheduling algorithm"
+    ),
+    algo_params: AlgoParams = Form(
+        default=AlgoParams(),
+        description="The parameter values passed to the scheduling algorithm. Required parameters varies per algorithm.",
+    ),
 ):
     """
     Unrolls and partitions a logical graph with the provided various parameters.
 
     One of lg_name and lg_content, but not both, must be specified.
     """
     lg_graph = load_graph(lg_content, lg_name)
-    pgt = dlg.dropmake.pg_generator.unroll(lg_graph, oid_prefix, zero_run, default_app)
+    pgt = dlg.dropmake.pg_generator.unroll(
+        lg_graph, oid_prefix, zero_run, default_app
+    )
     pgt = init_pgt_unroll_repro_data(pgt)
     reprodata = pgt.pop()
-    pgt = dlg.dropmake.pg_generator.partition(pgt, algorithm, num_partitions, num_islands,
-                                              algo_params.dict())
+    pgt = dlg.dropmake.pg_generator.partition(
+        pgt, algorithm, num_partitions, num_islands, algo_params.dict()
+    )
     pgt.append(reprodata)
     pgt = init_pgt_partition_repro_data(pgt)
     return JSONResponse(pgt)
 
 
 @app.post("/map", response_class=JSONResponse, tags=["Updated"])
 def pgt_map(
-        pgt_name: str = Form(default=None,
-                             description="If supplied, this graph will attempted to be loaded from disk on the server"),
-        pgt_content: str = Form(default=None, description="If supplied, this is the graph content"),
-        nodes: str = Form(default=None,
-                          description="Comma separated list of IP addrs e.g. 'localhost, 127.0.0.2'"),
-        num_islands: int = Form(default=1, description="The number of data islands to launch"),
-        co_host_dim: bool = Form(default=True,
-                                 description="Whether to launch data island manager processes alongside node-managers"),
-        host: str = Form(default=None,
-                         description="If present, will attempt to query this address for node-managers"),
-        port: int = Form(default=dlg.constants.ISLAND_DEFAULT_REST_PORT,
-                         description="Port used by HOST manager process")
+    pgt_name: str = Form(
+        default=None,
+        description="If supplied, this graph will attempted to be loaded from disk on the server",
+    ),
+    pgt_content: str = Form(
+        default=None, description="If supplied, this is the graph content"
+    ),
+    nodes: str = Form(
+        default=None,
+        description="Comma separated list of IP addrs e.g. 'localhost, 127.0.0.2'",
+    ),
+    num_islands: int = Form(
+        default=1, description="The number of data islands to launch"
+    ),
+    co_host_dim: bool = Form(
+        default=True,
+        description="Whether to launch data island manager processes alongside node-managers",
+    ),
+    host: str = Form(
+        default=None,
+        description="If present, will attempt to query this address for node-managers",
+    ),
+    port: int = Form(
+        default=dlg.constants.ISLAND_DEFAULT_REST_PORT,
+        description="Port used by HOST manager process",
+    ),
 ):
     """
     Maps physical graph templates to node resources.
     """
     if not nodes:
         client = CompositeManagerClient(host, port, timeout=10)
         nodes = [host] + client.nodes()
     if len(nodes) <= num_islands:
         logger.error("Not enough nodes to fill all islands")
-        HTTPException(status_code=500,
-                      detail="#nodes (%d) should be larger than the number of islands (%d)" % (
-                          len(nodes), num_islands))
+        HTTPException(
+            status_code=500,
+            detail="#nodes (%d) should be larger than the number of islands (%d)"
+            % (len(nodes), num_islands),
+        )
     pgt = load_graph(pgt_content, pgt_name)
     reprodata = {}
     if not pgt[-1].get("oid"):
         reprodata = pgt.pop()
     logger.info(nodes)
-    pg = dlg.dropmake.pg_generator.resource_map(pgt, nodes, num_islands, co_host_dim)
+    pg = dlg.dropmake.pg_generator.resource_map(
+        pgt, nodes, num_islands, co_host_dim
+    )
     pg.append(reprodata)
     pg = init_pg_repro_data(pg)
     return JSONResponse(pg)
 
 
 @app.get("/api/submission_method")
 def get_submission_method(
-        dlg_mgr_url: str = Query(default=None,
-                                description="If present, translator will query this URL for its deployment options"),
-        dlg_mgr_host: str = Query(default=None,
-                                 description="If present with mport and mprefix, will be the base host for deployment"),
-        dlg_mgr_port: int = Query(default=None,
-                                 description="")
+    dlg_mgr_url: str = Query(
+        default=None,
+        description="If present, translator will query this URL for its deployment options",
+    ),
+    dlg_mgr_host: str = Query(
+        default=None,
+        description="If present with mport and mprefix, will be the base host for deployment",
+    ),
+    dlg_mgr_port: int = Query(default=None, description=""),
 ):
     logger.debug("Received submission_method request")
     if dlg_mgr_url:
         mhost, mport, mprefix = parse_mgr_url(dlg_mgr_url)
     else:
         mhost = dlg_mgr_host
         mport = dlg_mgr_port
         mprefix = ""
     available_methods = []
     if check_k8s_env():
         available_methods.append(DeploymentMethods.HELM)
     if mhost is not None:
-        host_available_methods = get_mgr_deployment_methods(mhost, mport, mprefix)
+        host_available_methods = get_mgr_deployment_methods(
+            mhost, mport, mprefix
+        )
         if DeploymentMethods.BROWSER in host_available_methods:
             available_methods.append(DeploymentMethods.SERVER)
     return {"methods": available_methods}
 
 
-@app.get("/", response_class=HTMLResponse, description="The page used to view physical graphs")
+@app.get(
+    "/",
+    response_class=HTMLResponse,
+    description="The page used to view physical graphs",
+)
 def index(request: Request):
-    tpl = templates.TemplateResponse("pg_viewer.html", {
-        "request": request,
-        "pgt_view_json_name": None,
-        "partition_info": None,
-        "title": "Physical Graph Template",
-        "error": None
-    })
+    tpl = templates.TemplateResponse(
+        "pg_viewer.html",
+        {
+            "request": request,
+            "pgt_view_json_name": None,
+            "partition_info": None,
+            "title": "Physical Graph Template",
+            "error": None,
+        },
+    )
     return tpl
 
 
 @app.head("/")
 def liveliness():
     return {}
 
@@ -845,22 +1150,24 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-d",
         "--lgdir",
         action="store",
         type=str,
         dest="lg_path",
+        default="/tmp",
         help="A path that contains at least one sub-directory, which contains logical graph files",
     )
     parser.add_argument(
         "-t",
         "--pgtdir",
         action="store",
         type=str,
         dest="pgt_path",
+        default="/tmp",
         help="physical graph template path (output)",
     )
     parser.add_argument(
         "-H",
         "--host",
         action="store",
         type=str,
@@ -881,35 +1188,53 @@
         "-v",
         "--verbose",
         action="store_true",
         dest="verbose",
         default=False,
         help="Enable more logging",
     )
+    parser.add_argument(
+        "-l",
+        "--log-dir",
+        action="store",
+        type=str,
+        dest="logdir",
+        help="The directory where the logging files will be stored",
+        default=utils.getDlgLogsDir(),
+    )
 
     options = parser.parse_args(args)
 
     if options.lg_path is None or options.pgt_path is None:
         parser.error("Graph paths missing (-d/-t)")
     elif not os.path.exists(options.lg_path):
         parser.error(f"{options.lg_path} does not exist")
 
-    if options.verbose:
+    if options.verbose or options.logdir:
         fmt = logging.Formatter(
             "%(asctime)-15s [%(levelname)5.5s] [%(threadName)15.15s] "
             "%(name)s#%(funcName)s:%(lineno)s %(message)s"
         )
         fmt.converter = time.gmtime
-        stream_handler = logging.StreamHandler(sys.stdout)
-        stream_handler.setFormatter(fmt)
-        logging.root.addHandler(stream_handler)
-        logging.root.setLevel(logging.DEBUG)
+        if options.verbose:
+            stream_handler = logging.StreamHandler(sys.stdout)
+            stream_handler.setFormatter(fmt)
+            logging.root.addHandler(stream_handler)
+            logging.root.setLevel(logging.DEBUG)
+        if options.logdir:
+            # This is the logfile we'll use from now on
+            logdir = options.logdir
+            utils.createDirIfMissing(logdir)
+            logfile = os.path.join(logdir, "dlgTranslator.log")
+            fileHandler = logging.FileHandler(logfile)
+            fileHandler.setFormatter(fmt)
+            logging.root.addHandler(fileHandler)
 
     try:
-        os.makedirs(options.pgt_path)
+        os.makedirs(options.pgt_path, exist_ok=True)
     except OSError:
         logging.warning("Cannot create path %s", options.pgt_path)
 
     global lg_dir
     global pgt_dir
     global pg_mgr
 
@@ -922,13 +1247,13 @@
 
     signal.signal(signal.SIGTERM, handler)
     signal.signal(signal.SIGINT, handler)
 
     uvicorn.run(
         app=app,
         host=options.host,
-        port=options.port
+        port=options.port,
     )
 
 
 if __name__ == "__main__":
     run(None, sys.argv[1:])
```

### Comparing `daliuge-translator-2.4.0/dlg/dropmake/web/translator_utils.py` & `daliuge-translator-3.0.0/dlg/dropmake/web/translator_utils.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/translator/__init__.py` & `daliuge-translator-3.0.0/dlg/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/dlg/translator/tool_commands.py` & `daliuge-translator-3.0.0/dlg/translator/tool_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,17 @@
     Unrolls the Logical Graph in `lg_graph` into a Physical Graph Template
     and return the latter.
     This method prepends `oid_prefix` to all generated Drop OIDs.
     """
     from ..dropmake.pg_generator import unroll
 
     logger.info("Start to unroll %s", lg_path)
-    return unroll(_open_i(lg_path), oid_prefix=oid_prefix, zerorun=zerorun, app=app)
+    return unroll(
+        _open_i(lg_path), oid_prefix=oid_prefix, zerorun=zerorun, app=app
+    )
 
 
 _param_types = {
     "min_goal": int,
     "ptype": int,
     "max_load_imb": int,
     "max_cpu": int,
@@ -115,24 +117,33 @@
         host=opts.host,
         port=opts.port,
         skip_deploy=opts.skip_deploy,
         session_id=opts.session_id,
     )
     if opts.wait:
         common.monitor_sessions(
-            session_id, host=opts.host, port=opts.port, poll_interval=opts.poll_interval
+            session_id,
+            host=opts.host,
+            port=opts.port,
+            poll_interval=opts.poll_interval,
         )
 
     if opts.reproducibility:
         dump = _setup_output(opts)
         common.monitor_sessions_repro(
-            session_id, host=opts.host, port=opts.port, poll_interval=opts.poll_interval
+            session_id,
+            host=opts.host,
+            port=opts.port,
+            poll_interval=opts.poll_interval,
         )
         repro_data = common.fetch_reproducibility(
-            session_id, host=opts.host, port=opts.port, poll_interval=opts.poll_interval
+            session_id,
+            host=opts.host,
+            port=opts.port,
+            poll_interval=opts.poll_interval,
         )
         dump(repro_data["graph"])
 
 
 def _add_output_options(parser):
     parser.add_option(
         "-o",
@@ -194,16 +205,20 @@
             return "kv"
         else:
             return None
 
     # putting all parameters together in a single dictionary
     for p in opts.parameter:
         if param_spec_type(p) is None:
-            parser.error("Parameter %s is neither JSON nor has it key=value form" % p)
-    params = [p.split("=") for p in opts.parameter if param_spec_type(p) == "kv"]
+            parser.error(
+                "Parameter %s is neither JSON nor has it key=value form" % p
+            )
+    params = [
+        p.split("=") for p in opts.parameter if param_spec_type(p) == "kv"
+    ]
     params = dict(params)
     for json_param in (
         json.loads(p) for p in opts.parameter if param_spec_type(p) == "json"
     ):
         params.update(json_param)
 
     from ..dropmake.pg_generator import fill
@@ -243,29 +258,34 @@
         "--app",
         action="store",
         type="int",
         dest="app",
         help="Force an app to be used in the Physical Graph. 0=Don't force, 1=SleepApp, 2=SleepAndCopy",
         default=0,
     )
-    apps = (None, "dlg.apps.simple.SleepApp", "dlg.apps.simple.SleepAndCopyApp")
+    apps = (
+        None,
+        "dlg.apps.simple.SleepApp",
+        "dlg.apps.simple.SleepAndCopyApp",
+    )
     return apps
 
 
 def dlg_unroll(parser, args):
     # Unroll Logical Graph
     tool.add_logging_options(parser)
     _add_output_options(parser)
     apps = _add_unroll_options(parser)
     (opts, args) = parser.parse_args(args)
     tool.setup_logging(opts)
     dump = _setup_output(opts)
     pgt = unroll(
         opts.lg_path, opts.oid_prefix, zerorun=opts.zerorun, app=apps[opts.app]
     )
+    logger.debug(">>> pgt: %s", pgt)
     dump(init_pgt_unroll_repro_data(pgt))
 
 
 def _add_partition_options(parser):
     from ..dropmake import pg_generator
 
     parser.add_option(
@@ -517,23 +537,29 @@
 
 def register_commands():
     tool.cmdwrap(
         "lgweb",
         "A Web server for the Logical Graph Editor",
         "dlg.dropmake.web.translator_rest:run",
     )
-    tool.cmdwrap("submit", "Submits a Physical Graph to a Drop Manager", dlg_submit)
+    tool.cmdwrap(
+        "submit", "Submits a Physical Graph to a Drop Manager", dlg_submit
+    )
     tool.cmdwrap(
         "map",
         "Maps a Physical Graph Template to resources and produces a Physical Graph",
         dlg_map,
     )
     tool.cmdwrap(
-        "unroll", "Unrolls a Logical Graph into a Physical Graph Template", dlg_unroll
+        "unroll",
+        "Unrolls a Logical Graph into a Physical Graph Template",
+        dlg_unroll,
     )
     tool.cmdwrap(
         "partition",
         "Divides a Physical Graph Template into N logical partitions",
         dlg_partition,
     )
-    tool.cmdwrap("unroll-and-partition", "unroll + partition", dlg_unroll_and_partition)
+    tool.cmdwrap(
+        "unroll-and-partition", "unroll + partition", dlg_unroll_and_partition
+    )
     tool.cmdwrap("fill", "Fill a Logical Graph with parameters", dlg_fill)
```

### Comparing `daliuge-translator-2.4.0/setup.py` & `daliuge-translator-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 # Version information
 # We do like numpy: we have a major/minor/patch hand-written version written
 # here. If we find the git commit (either via "git" command execution or in a
 # dlg/version.py file) we append it to the VERSION later.
 # The RELEASE flag allows us to create development versions properly supported
 # by setuptools/pkg_resources or "final" versions.
-MAJOR = 2
-MINOR = 4
+MAJOR = 3
+MINOR = 0
 PATCH = 0
 RELEASE = True
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, PATCH)
 VERSION_FILE = "dlg/translator/version.py"
 
 
 def get_git_version():
@@ -94,16 +94,18 @@
 
 install_requires = [
     "daliuge-common==%s" % (VERSION,),
     "fastapi",
     "jinja2",
     "jsonschema",
     "metis>=0.2a3",
+    "netifaces",
     "networkx",
     "numpy",
+    "parameterized",
     "psutil",
     "pyswarm",
     "python-multipart",
     # "ruamel.yaml.clib<=0.2.2",
     "uvicorn==0.18",
     "wheel",
 ]
```

### Comparing `daliuge-translator-2.4.0/test/__init__.py` & `daliuge-translator-3.0.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/test/dropmake/__init__.py` & `daliuge-translator-3.0.0/test/reproducibility/__init__.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/test/dropmake/test_lg_fill.py` & `daliuge-translator-3.0.0/test/dropmake/test_lg_fill.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,27 @@
 import pkg_resources
 from dlg.dropmake import pg_generator
 
 lg_dir = pkg_resources.resource_filename(
     __name__, "logical_graphs"
 )  # @UndefinedVariable
 
+
 # Test LGT to LG method: Filling parameter values in LG.
 class LGFillTest(unittest.TestCase):
     def test_fill_lg(self):
         params = {
             "param1": 1,
             "param2": "2",
             "param1.param2": True,
             "param4": {"what": "hi"},
         }
-        with open(os.path.join(lg_dir, "cont_img.graph")) as f:
+        with open(os.path.join(lg_dir, "cont_img_mvp.graph")) as f:
             lg = pg_generator.fill(json.load(f), params)
         for node_idx, value in zip((5, 12, 26, 34), ("1", "2", "True", "hi")):
             print(node_idx)
             node = lg["nodeDataArray"][node_idx]
             found = None
             for field in node["fields"]:
-                if field["name"] == "arg10":
+                if field["name"] == "dummy":
                     found = field["value"]
             self.assertEqual(found, value)
```

### Comparing `daliuge-translator-2.4.0/test/dropmake/test_lgweb.py` & `daliuge-translator-3.0.0/test/dropmake/test_lgweb.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,28 @@
 #
 
 import json
 import os
 import shutil
 import tempfile
 import unittest
+from parameterized import parameterized
 import urllib.parse
+import logging
 
 import pkg_resources
 
 from dlg import common
 from dlg.common import tool
 from dlg.dropmake.web.translator_utils import get_mgr_deployment_methods
 from dlg.restutils import RestClient, RestClientException
 
 lg_dir = pkg_resources.resource_filename(__name__, ".")  # @UndefinedVariable
 lgweb_port = 8086
+logger = logging.getLogger(__name__)
 
 
 class TestLGWeb(unittest.TestCase):
     def setUp(self):
         unittest.TestCase.setUp(self)
         self.temp_dir = tempfile.mkdtemp()
         args = [
@@ -47,33 +50,41 @@
             lg_dir,
             "-t",
             self.temp_dir,
             "-p",
             str(lgweb_port),
             "-H",
             "localhost",
+            "-vv",
+            # "-l",
+            # self.temp_dir,
         ]
-        self.devnull = open(os.devnull, "wb")
-        self.web_proc = tool.start_process(
-            "lgweb", args, stdout=self.devnull, stderr=self.devnull
-        )
+        # uncomment to capture local logs, but reverse before
+        # push to github.
+        # lf = f"{self.temp_dir}/dlgTrans.log"
+        lf = "/dev/null"
+        with open(lf, "wb") as self.logfile:
+            self.web_proc = tool.start_process(
+                "lgweb", args, stdout=self.logfile, stderr=self.logfile
+            )
 
     def tearDown(self):
-        shutil.rmtree(self.temp_dir)
-        self.devnull.close()
+        if self.logfile.name == "/dev/null":
+            shutil.rmtree(self.temp_dir)
+        else:
+            logger.info("Kept logfile in: %s", self.logfile.name)
         common.terminate_or_kill(self.web_proc, 10)
         unittest.TestCase.tearDown(self)
 
     def _generate_pgt(self, c):
         c._GET(
             "/gen_pgt?lg_name=logical_graphs/chiles_simple.graph&num_par=5&algo=metis&min_goal=0&ptype=0&max_load_imb=100"
         )
 
     def test_get_lgjson(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
 
         # a specific one
         lg = c._get_json(
             "/jsonbody?lg_name=logical_graphs/chiles_simple.graph"
         )
         self.assertIsNotNone(lg)
@@ -86,15 +97,14 @@
         self.assertRaises(
             RestClientException,
             c._get_json,
             "/jsonbody?lg_name=doesnt_exist.graph",
         )
 
     def test_post_lgjson(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
 
         # new graphs cannot currently be added
         form_data = {
             "lg_name": "new.graph",
             "lg_content": '{"id": 1, "name": "example"}',
             "rmode": "1",
@@ -123,15 +133,14 @@
             self.assertEqual(1, new["id"])
             self.assertEqual("example", new["name"])
             self.assertEqual("1", new["reprodata"]["rmode"])
         finally:
             shutil.move(copy_fname, original_fname)
 
     def test_gen_pgt(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
 
         # doesn't exist!
         self.assertRaises(
             RestClientException,
             c._GET,
             "/gen_pgt?lg_name=doesnt_exist.json&num_par=5&algo=metis&min_goal=0&ptype=0&max_load_imb=100",
@@ -142,15 +151,14 @@
             c._GET,
             "/gen_pgt?lg_name=logical_graphs/chiles_simple.graph&num_par=5&algo=noidea",
         )
         # this should work now
         self._generate_pgt(c)
 
     def test_get_pgtjson(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
         c._GET(
             "/gen_pgt?lg_name=logical_graphs/chiles_simple.graph&num_par=5&algo=metis&min_goal=0&ptype=0&max_load_imb=100"
         )
 
         # doesn't exist
         self.assertRaises(
@@ -160,15 +168,14 @@
         )
         # good!
         c._get_json(
             "/pgt_jsonbody?pgt_name=logical_graphs/chiles_simple1_pgt.graph"
         )
 
     def test_get_pgt_post(self, algo="metis", algo_options=None):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
 
         # an API call with an empty form should cause an error
         self.assertRaises(RestClientException, c._POST, "/gen_pgt")
 
         # new logical graph JSON
         fname = os.path.join(
@@ -198,16 +205,16 @@
                 "/gen_pgt",
                 content,
                 content_type="application/x-www-form-urlencoded",
             )
         except RestClientException as e:
             self.fail(e)
 
+    @unittest.skip("MKN does not work at this point")
     def test_mkn_pgt_post(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
 
         # an API call with an empty form should cause an error
         self.assertRaises(RestClientException, c._POST, "/gen_pgt")
 
         # new logical graph JSON
         fname = os.path.join(lg_dir, "logical_graphs", "simpleMKN.graph")
@@ -234,15 +241,14 @@
                 content,
                 content_type="application/x-www-form-urlencoded",
             )
         except RestClientException as e:
             self.fail(e)
 
     def test_loop_pgt_post(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
 
         # an API call with an empty form should cause an error
         self.assertRaises(RestClientException, c._POST, "/gen_pgt")
 
         # new logical graph JSON
         with open(
@@ -287,21 +293,21 @@
 
     def test_min_num_parts_translation(self):
         self.test_get_pgt_post(
             algo="min_num_parts",
             algo_options={"deadline": 300, "time_greedy": 50},
         )
 
+    @unittest.skip("This one fails sometimes with HTTP error 557.")
     def test_pso_translation(self):
         self.test_get_pgt_post(
             algo="pso", algo_options={"swarm_size": 10, "deadline": 300}
         )
 
     def test_pg_viewer(self):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
         self._generate_pgt(c)
 
         # doesn't exist
         self.assertRaises(
             RestClientException,
             c._GET,
@@ -311,15 +317,14 @@
         c._GET("/pg_viewer")
         # also fine, PGT exists
         c._GET(
             "/pg_viewer?pgt_view_name=logical_graphs/chiles_simple1_pgt.graph"
         )
 
     def _test_pgt_action(self, path, unknown_fails):
-
         c = RestClient("localhost", lgweb_port, timeout=10)
         self._generate_pgt(c)
 
         # doesn't exist
         if unknown_fails:
             self.assertRaises(
                 RestClientException,
@@ -385,30 +390,32 @@
             else:
                 try:
                     ret = client._POST(url)
                 except RestClientException as e:
                     self.fail(e)
             return json.load(ret)
 
-    def test_get_fill(self):
+    @parameterized.expand([("0", "testLoop.graph"), ("1", "ArrayLoop.graph")])
+    def test_get_fill(self, n, graph):
         c = RestClient("localhost", lgweb_port, timeout=10)
         test_url = "/lg_fill"
         with open(
-            os.path.join(lg_dir, "logical_graphs", "testLoop.graph"), "rb"
+            os.path.join(lg_dir, "logical_graphs", graph), "rb"
         ) as infile:
             json_data = infile.read()
+            logger.info("Logical graph %s loaded", infile.name)
         request_tests = [
             (None, True),  # Call with an empty form should cause an error
             ({"lg_name": "metis.graph"}, True),  # Invalid lg_name
             (
                 {"lg_name": "logical_graphs/chiles_simple.graph"},
                 False,
             ),  # Valid lg_name
             (
-                {"lg_name": "chiles_simple.graph", "lg_content": json_data},
+                {"lg_name": graph, "lg_content": json_data},
                 True,
             ),  # Both lg_name and lg_content
             ({"lg_content": "{'garbage: 3}"}, True),  # Invalid lg_content
             ({"lg_content": json_data}, False),  # Valid lg_content
             (
                 {"lg_content": json_data, "parameters": '{"nonsense: 3}'},
                 True,
@@ -418,46 +425,55 @@
                 False,
             ),  # Valid parameters
         ]
 
         for request in request_tests:
             self._test_post_request(c, test_url, request[0], request[1])
 
-    def test_lg_unroll(self):
+    @parameterized.expand(
+        [("testLoop", "testLoop.graph"), ("ArrayLoop", "ArrayLoop.graph")]
+    )
+    def test_lg_unroll(self, n, graph):
         c = RestClient("localhost", lgweb_port, timeout=10)
         test_url = "/unroll"
         with open(
-            os.path.join(lg_dir, "logical_graphs", "testLoop.graph"), "rb"
+            os.path.join(lg_dir, "logical_graphs", graph), "rb"
         ) as infile:
             json_data = infile.read()
 
         request_tests = [
-            (None, True),  # Call with an empty form should cause an error
+            (
+                None,
+                True,
+            ),  # Call with an empty form should cause an error
             ({"lg_name": "metis.graph"}, True),  # Invalid lg_name
             (
                 {"lg_name": "logical_graphs/chiles_simple.graph"},
                 False,
             ),  # Valid lg_name
             (
-                {"lg_name": "chiles_simple.graph", "lg_content": json_data},
+                {"lg_name": graph, "lg_content": json_data},
                 True,
             ),  # Both lg_name and lg_content
-            ({"lg_content": "{'garbage: 3}"}, True),  # Invalid lg_content
+            (
+                {"lg_content": "{'garbage: 3}"},
+                True,
+            ),  # Invalid lg_content
             ({"lg_content": json_data}, False),  # Valid lg_content
         ]
 
         for request in request_tests:
             self._test_post_request(c, test_url, request[0], request[1])
 
         # test default_app
         form_data = {"lg_content": json_data, "default_app": "test.app"}
         pgt = self._test_post_request(c, test_url, form_data, False)
         for dropspec in pgt:
-            if "app" in dropspec:
-                self.assertEqual(dropspec["app"], "test.app")
+            if "dropclass" in dropspec:
+                self.assertEqual(dropspec["dropclass"], "test.app")
 
     def test_pgt_partition(self):
         c = RestClient("localhost", lgweb_port, timeout=10)
         test_url = "/partition"
         with open(
             os.path.join(lg_dir, "logical_graphs", "testLoop.graph"), "rb"
         ) as infile:
```

### Comparing `daliuge-translator-2.4.0/test/dropmake/test_pg_gen.py` & `daliuge-translator-3.0.0/test/dropmake/test_pg_gen.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #    License along with this library; if not, write to the Free Software
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 #    MA 02111-1307  USA
 
 import unittest
 
 import pkg_resources
+from dlg.common import CategoryType
 from dlg.dropmake.lg import LG
 from dlg.dropmake.pgt import PGT, GPGTNoNeedMergeException
 from dlg.dropmake.pgtp import MetisPGTP, MySarkarPGTP, MinNumPartsPGTP
 
 """
 python -m unittest test.dropmake.test_pg_gen
 """
@@ -35,18 +36,18 @@
     return pkg_resources.resource_filename(
         __name__, "logical_graphs/{0}".format(lg_name)
     )  # @UndefinedVariable
 
 
 class TestPGGen(unittest.TestCase):
     def test_pg_generator(self):
-        fp = get_lg_fname("cont_img.graph")
+        fp = get_lg_fname("cont_img_mvp.graph")
         #        fp = get_lg_fname('testScatter.graph')
         lg = LG(fp)
-        self.assertEqual(len(lg._done_dict.keys()), 46)
+        self.assertEqual(len(lg._done_dict.keys()), 45)
         drop_list = lg.unroll_to_tpl()
         # print json.dumps(drop_list, indent=2)
         # pprint.pprint(drop_list)
         # pprint.pprint(dict(lg._drop_dict))
         # input_dict = defaultdict(list)
         # lg.to_pg_tpl(input_dict)
 
@@ -66,17 +67,17 @@
         pg_json = pgt.to_gojs_json()
         _dum = pg_json
         # we should really check the output here
 
     def test_metis_pgtp(self):
         lgnames = [
             "HelloWorld_simple.graph",
-            "simpleMKN.graph",
+            # "simpleMKN.graph",
             "testLoop.graph",
-            "cont_img.graph",
+            "cont_img_mvp.graph",
             "test_grpby_gather.graph",
             "chiles_simple.graph",
         ]
         tgt_partnum = [15, 15, 10, 10, 5]
         for i, lgn in enumerate(lgnames):
             fp = get_lg_fname(lgn)
             lg = LG(fp)
@@ -84,15 +85,15 @@
             pgtp = MetisPGTP(drop_list)
             pgtp.json
 
     def test_metis_pgtp_gen_pg(self):
         lgnames = [
             "HelloWorld_simple.graph",
             "testLoop.graph",
-            "cont_img.graph",
+            "cont_img_mvp.graph",
             "test_grpby_gather.graph",
             "chiles_simple.graph",
         ]
         tgt_partnum = [15, 15, 10, 10, 5]
         node_list = ["10.128.0.11", "10.128.0.12", "10.128.0.13"]
         for i, lgn in enumerate(lgnames):
             fp = get_lg_fname(lgn)
@@ -104,15 +105,15 @@
             pg_spec = pgtp.to_pg_spec(node_list)
             # with open('/tmp/met_{0}_pgspec.graph'.format(lgn.split('.')[0]), 'w') as f:
             #     f.write(pg_spec)
 
     def test_metis_pgtp_gen_pg_island(self):
         lgnames = [
             "testLoop.graph",
-            "cont_img.graph",
+            "cont_img_mvp.graph",
             "test_grpby_gather.graph",
             "chiles_simple.graph",
         ]
         tgt_partnum = [15, 15, 10, 10, 5]
         node_list = [
             "10.128.0.11",
             "10.128.0.12",
@@ -131,47 +132,48 @@
             pgtp.to_gojs_json(visual=False)
             pg_spec = pgtp.to_pg_spec(node_list, num_islands=nb_islands)
             pgtp.result(lazy=False)
 
     def test_mysarkar_pgtp(self):
         lgnames = [
             "testLoop.graph",
-            "cont_img.graph",
+            "cont_img_mvp.graph",
             "test_grpby_gather.graph",
             "chiles_simple.graph",
         ]
-        tgt_partnum = [15, 15, 10, 10, 5]
+        # tgt_partnum = [15, 15, 10, 10, 5]
         for i, lgn in enumerate(lgnames):
             fp = get_lg_fname(lgn)
             lg = LG(fp)
             drop_list = lg.unroll_to_tpl()
             pgtp = MySarkarPGTP(drop_list)
             pgtp.json
 
     def test_mysarkar_pgtp_gen_pg(self):
-        # TODO: cont_img.graph causes random failures in this test.
-        # ERROR: dlg.dropmake.scheduler.SchedulerException: Cannot find a idle PID, max_dop provided: 8
-
-        # lgnames = ['testLoop.graph', 'cont_img.graph', 'test_grpby_gather.graph', 'chiles_simple.graph']
-        lgnames = ["testLoop.graph", "test_grpby_gather.graph", "chiles_simple.graph"]
+        lgnames = [
+            "testLoop.graph",
+            "cont_img_mvp.graph",
+            "test_grpby_gather.graph",
+            "chiles_simple.graph",
+        ]
         tgt_partnum = [15, 15, 10, 10, 5]
         node_list = ["10.128.0.11", "10.128.0.12", "10.128.0.13"]
         for i, lgn in enumerate(lgnames):
             fp = get_lg_fname(lgn)
             lg = LG(fp)
             drop_list = lg.unroll_to_tpl()
             pgtp = MySarkarPGTP(drop_list, 3, merge_parts=True)
             # pgtp.json
             pgtp.to_gojs_json(visual=False)
             pg_spec = pgtp.to_pg_spec(node_list)
 
     def test_mysarkar_pgtp_gen_pg_island(self):
         lgnames = [
             "testLoop.graph",
-            "cont_img.graph",
+            "cont_img_mvp.graph",
             "test_grpby_gather.graph",
             "chiles_simple.graph",
         ]
         node_list = [
             "10.128.0.11",
             "10.128.0.12",
             "10.128.0.13",
@@ -184,24 +186,26 @@
             lg = LG(fp)
             drop_list = lg.unroll_to_tpl()
             pgtp = MySarkarPGTP(drop_list, None, merge_parts=True)
             pgtp.to_gojs_json(visual=False)
             nb_islands = 2
             # print(lgn)
             try:
-                pgtp.merge_partitions(len(node_list) - nb_islands, form_island=False)
+                pgtp.merge_partitions(
+                    len(node_list) - nb_islands, form_island=False
+                )
             except GPGTNoNeedMergeException as ge:
                 continue
             pg_spec = pgtp.to_pg_spec(node_list, num_islands=nb_islands)
             pgtp.result()
 
     def test_minnumparts_pgtp(self):
         lgnames = [
             "testLoop.graph",
-            "cont_img.graph",
+            "cont_img_mvp.graph",
             "test_grpby_gather.graph",
             "chiles_simple.graph",
         ]
         # tgt_partnum = [15, 15, 10, 10, 5]
         tgt_deadline = [200, 300, 90, 80, 160]
         for i, lgn in enumerate(lgnames):
             fp = get_lg_fname(lgn)
@@ -233,9 +237,9 @@
         # Test loading of shared memory graph
         lgs = ["SharedMemoryTest.graph"]
         for lg in lgs:
             fp = get_lg_fname(lg)
             lg = LG(fp)
             out = lg.unroll_to_tpl()
             for drop in out:
-                if drop["type"] == "data":
-                    self.assertEqual("SharedMemory", drop["storage"])
+                if drop["categoryType"] in [CategoryType.DATA, "data"]:
+                    self.assertEqual("SharedMemory", drop["category"])
```

### Comparing `daliuge-translator-2.4.0/test/dropmake/test_scheduler.py` & `daliuge-translator-3.0.0/test/dropmake/test_scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,38 +51,38 @@
     )  # @UndefinedVariable
 
 
 class TestScheduler(unittest.TestCase):
     def test_incremental_antichain(self):
         part = Partition(100, 8)
         G = part._dag
-        assert part.probe_max_dop(1, 2, True, True, True) == DAGUtil.get_max_dop(
-            part._dag
-        )
+        assert part.probe_max_dop(
+            1, 2, True, True, True
+        ) == DAGUtil.get_max_dop(part._dag)
         G.add_edge(2, 3)
-        assert part.probe_max_dop(2, 3, False, True, True) == DAGUtil.get_max_dop(
-            part._dag
-        )
+        assert part.probe_max_dop(
+            2, 3, False, True, True
+        ) == DAGUtil.get_max_dop(part._dag)
         # G.add_edge(1, 4)
         # assert(part.probe_max_dop(1, 4, False, True, True) == DAGUtil.get_max_dop(part._dag))
         # G.add_edge(2, 5)
         l = part.probe_max_dop(2, 5, False, True, True)
         r = DAGUtil.get_max_dop(part._dag)
         assert l == r, "l = {0}, r = {1}".format(l, r)
 
     def test_basic_scheduler(self):
-        fp = get_lg_fname("cont_img.graph")
+        fp = get_lg_fname("cont_img_mvp.graph")
         lg = LG(fp)
         drop_list = lg.unroll_to_tpl()
         Scheduler(drop_list)
 
     def test_minnumparts_scheduler(self):
         lgs = {
-            "cont_img.graph": 500,
-            "cont_img.graph": 200,
+            "cont_img_mvp.graph": 500,
+            "cont_img_mvp.graph": 200,
             "test_grpby_gather.graph": 90,
             "chiles_simple.graph": 160,
         }
         mdp = 8
         ofa = 0.5
         for lgn, deadline in lgs.items():
             fp = get_lg_fname(lgn)
@@ -91,16 +91,16 @@
             mps = MinNumPartsScheduler(
                 drop_list, deadline, max_dop=mdp, optimistic_factor=ofa
             )
             mps.partition_dag()
 
     def test_mysarkar_scheduler(self):
         lgs = {
-            "cont_img.graph": 20,
-            "cont_img.graph": 15,
+            "cont_img_mvp.graph": 20,
+            "cont_img_mvp.graph": 15,
             "test_grpby_gather.graph": 10,
             "chiles_simple.graph": 5,
         }
         mdp = 8
         for lgn, numparts in lgs.items():
             fp = get_lg_fname(lgn)
             lg = LG(fp)
@@ -118,16 +118,16 @@
 
     @unittest.skipIf(
         skip_long_tests,
         "Skipping because they take too long. Chen to eventually shorten them",
     )
     def test_pso_scheduler(self):
         lgs = {
-            "cont_img.graph": 540,
-            "cont_img.graph": 450,
+            "cont_img_mvp.graph": 540,
+            "cont_img_mvp.graph": 450,
             "test_grpby_gather.graph": 70,
             "chiles_simple.graph": 160,
         }
         mdp = 2
         for lgn, deadline in lgs.items():
             fp = get_lg_fname(lgn)
             lg = LG(fp)
```

### Comparing `daliuge-translator-2.4.0/test/reproducibility/test_accumulatedata.py` & `daliuge-translator-3.0.0/test/reproducibility/test_accumulatedata.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,109 +26,155 @@
 """
 
 import os
 import json
 import optparse
 import tempfile
 import unittest
+import pytest
 
-from asyncio.log import logger
+# from asyncio.log import logger
+import logging
 import pkg_resources
 
 from dlg.common.reproducibility.constants import ReproducibilityFlags
 from dlg.common.reproducibility.reproducibility import (
     accumulate_lgt_drop_data,
     accumulate_lg_drop_data,
     accumulate_pgt_unroll_drop_data,
     accumulate_pgt_partition_drop_data,
     accumulate_pg_drop_data,
 )
-from dlg.translator.tool_commands import dlg_fill, dlg_unroll, dlg_partition, dlg_map
+from dlg.translator.tool_commands import (
+    dlg_fill,
+    dlg_unroll,
+    dlg_partition,
+    dlg_map,
+)
 
 SUPPORTED_WORKFLOWS = ["apps", "files", "misc", "groups"]
 
+logger = logging.getLogger("__name__")
+
+
+@pytest.fixture(scope="session")
+def log_level(pytestconfig):
+    return pytestconfig.getoption("--log-cli-level")
+
 
 def _fill_workflow(
-        rmode: ReproducibilityFlags, workflow: str, workflow_loc="./", scratch_loc="./"
+    rmode: ReproducibilityFlags,
+    workflow: str,
+    workflow_loc="./",
+    scratch_loc="./",
+    log_level=log_level,
 ):
     workflow_loc = pkg_resources.resource_filename("test", workflow_loc)
-    logger.debug(workflow_loc)
+    # # logger.debug(workflow_loc)
     lgt = workflow_loc + workflow + ".graph"
     lgr = scratch_loc + "/" + workflow + "LG.graph"
 
     rmodes = str(rmode.value)
 
     parser = optparse.OptionParser()
-    dlg_fill(parser, ["-L", lgt, "-R", rmodes, "-o", lgr, "-f", "newline"])
+    ll = "-v" if log_level else "-vv"
+    dlg_fill(parser, ["-L", lgt, "-R", rmodes, "-o", lgr, "-f", "newline", ll])
 
 
 def _run_full_workflow(
-        rmode: ReproducibilityFlags, workflow: str, workflow_loc="./", scratch_loc="./"
+    rmode: ReproducibilityFlags,
+    workflow: str,
+    workflow_loc="./",
+    scratch_loc="./",
+    log_level=log_level,
 ):
     lgr = scratch_loc + "/" + workflow + "LG.graph"
     pgs = scratch_loc + "/" + workflow + "PGS.graph"
     pgt = scratch_loc + "/" + workflow + "PGT.graph"
     pgr = scratch_loc + "/" + workflow + "PG.graph"
 
+    ll = "-v" if log_level.__repr__ else "-vv"
     _fill_workflow(rmode, workflow, workflow_loc, scratch_loc)
     parser = optparse.OptionParser()
-    dlg_unroll(parser, ["-L", lgr, "-o", pgs, "-f", "newline"])
+    dlg_unroll(parser, ["-L", lgr, "-o", pgs, "-f", "newline", ll])
     parser = optparse.OptionParser()
-    dlg_partition(parser, ["-P", pgs, "-o", pgt, "-f", "newline"])
+    dlg_partition(parser, ["-P", pgs, "-o", pgt, "-f", "newline", ll])
     parser = optparse.OptionParser()
     dlg_map(
-        parser, ["-P", pgt, "-N", "localhost, localhost", "-o", pgr, "-f", "newline"]
+        parser,
+        [
+            "-P",
+            pgt,
+            "-N",
+            "localhost, localhost",
+            "-o",
+            pgr,
+            "-f",
+            "newline",
+            ll,
+        ],
     )
 
 
-def _run_workflows(rmode: ReproducibilityFlags, root_file: str, names: list,
-                   temp_out: tempfile.TemporaryDirectory):
+def _run_workflows(
+    rmode: ReproducibilityFlags,
+    root_file: str,
+    names: list,
+    temp_out: tempfile.TemporaryDirectory,
+):
     for wflow_name in names:
         _run_full_workflow(rmode, wflow_name, root_file, temp_out.name)
 
 
-def _extract_reprodata(temp_out: tempfile.TemporaryDirectory, names: list, suffix: str):
+def _extract_reprodata(
+    temp_out: tempfile.TemporaryDirectory, names: list, suffix: str
+):
     output = {}
     for wflow_name in names:
         file = open(f"{temp_out.name}{os.sep}{wflow_name}{suffix}")
         output[wflow_name] = json.load(file)[0:-1]
         file.close()
     return output
 
+
 class AccumulateLGTRerunData(unittest.TestCase):
     """
     Tests the rerun standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.RERUN
     expected = {
         "category",
         "categoryType",
-        "inputPorts",
-        "inputLocalPorts",
-        "outputLocalPorts",
-        "outputPorts",
     }
     ddGraph = "graphs/ddTest.graph"
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt rerun data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -172,27 +218,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -206,18 +261,18 @@
 
     def test_all_accumulate(self):
         """
         Tests that lg rerun data is collected correctly (should not contain any information)
         """
         self._setup()
         for drop in enumerate(
-                self.lg_node_data
-                + self.lg_files_data
-                + self.lg_group_data
-                + self.lg_misc_data
+            self.lg_node_data
+            + self.lg_files_data
+            + self.lg_group_data
+            + self.lg_misc_data
         ):
             hash_data = accumulate_lg_drop_data(drop[1], self.rmode)
             self.assertEqual(self.expected, dict(hash_data.keys()))
 
 
 class AccumulatePGTUnrollRerunData(unittest.TestCase):
     """
@@ -229,45 +284,51 @@
     rmode = ReproducibilityFlags.RERUN
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         The the application type matters for rerunning
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only the storage type matters for rerunning
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only the drop type and input app type matters for rerunning
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -295,45 +356,51 @@
     rmode = ReproducibilityFlags.RERUN
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only application type matters for rerunning.
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only storage type matters for rerunning.
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only drop type matters for rerunning.
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -362,17 +429,23 @@
     rmode = ReproducibilityFlags.RERUN
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Nothing matters for rerunning.
         """
         expected = {}
@@ -391,16 +464,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, dict(hash_data[self.rmode.name].keys()))
 
     def test_group_accumulate(self):
         """
         Nothing matters for rerunning.
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -426,35 +499,39 @@
     Tests the repeat standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.REPEAT
     expected = {
         "category",
         "categoryType",
-        "inputPorts",
-        "inputLocalPorts",
-        "outputPorts",
-        "outputLocalPorts",
     }
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt repeat data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -497,27 +574,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -555,15 +641,15 @@
             "removeContainer",
             "additionalBindings",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _component(self, drop):
-        expected = {"execution_time", "num_cpus", "appclass"}
+        expected = {"execution_time", "num_cpus", "dropclass"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _memory(self, drop):
         expected = {"data_volume"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
@@ -595,15 +681,19 @@
             "num_of_copies",
             "scatter_axis",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def _loop(self, drop):
-        expected = {"inputApplicationName", "inputApplicationType", "num_of_iter"}
+        expected = {
+            "inputApplicationName",
+            "inputApplicationType",
+            "num_of_iter",
+        }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def test_all_accumulate(self):
         """
         We make the data expected for each accounted for drop type explicit.
         """
@@ -628,45 +718,51 @@
     rmode = ReproducibilityFlags.REPEAT
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -695,45 +791,51 @@
     rmode = ReproducibilityFlags.REPEAT
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters when repeating.
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only type matters when repeating.
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only type matters when repeating.
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -762,17 +864,23 @@
     rmode = ReproducibilityFlags.REPEAT
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Nothing matters for repeating.
         """
         expected = {}
@@ -791,16 +899,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, dict(hash_data[self.rmode.name].keys()))
 
     def test_group_accumulate(self):
         """
         Nothing matters for repeating.
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -826,35 +934,39 @@
     Tests the recompute standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.RECOMPUTE
     expected = {
         "category",
         "categoryType",
-        "inputPorts",
-        "inputLocalPorts",
-        "outputPorts",
-        "outputLocalPorts",
     }
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt recompute data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -897,27 +1009,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -955,25 +1076,30 @@
             "removeContainer",
             "additionalBindings",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _component(self, drop):
-        expected = {"execution_time", "num_cpus", "appclass"}
+        expected = {"execution_time", "num_cpus", "dropclass"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _memory(self, drop):
         expected = {"data_volume"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _file(self, drop):
-        expected = {"data_volume", "check_filepath_exists", "filepath", "dirname"}
+        expected = {
+            "data_volume",
+            "check_filepath_exists",
+            "filepath",
+            "dirname",
+        }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _ngas(self, drop):
         expected = {"data_volume"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
@@ -995,15 +1121,19 @@
             "num_of_copies",
             "scatter_axis",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def _loop(self, drop):
-        expected = {"inputApplicationName", "inputApplicationType", "num_of_iter"}
+        expected = {
+            "inputApplicationName",
+            "inputApplicationType",
+            "num_of_iter",
+        }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def test_all_accumulate(self):
         """
         We make the data expected for each accounted for drop type explicit.
         """
@@ -1028,45 +1158,51 @@
     rmode = ReproducibilityFlags.RECOMPUTE
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Type and rank matters.
         """
-        expected = {"type", "dt", "rank"}
+        expected = {"categoryType", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Type and rank matters.
         """
-        expected = {"type", "storage", "rank"}
+        expected = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Type and rank matters.
         """
-        expected_app = {"type", "dt", "rank"}
-        expected_file = {"type", "storage", "rank"}
+        expected_app = {"categoryType", "dt", "rank"}
+        expected_file = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1095,45 +1231,57 @@
     rmode = ReproducibilityFlags.RECOMPUTE
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Type, rank and machine information matters
         """
-        expected = ["type", "dt", "rank", "node", "island"]
+        expected = ["categoryType", "rank", "node", "island"]
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
-            self.assertEqual(sorted(expected), sorted(list(hash_data[self.rmode.name].keys())))
+            self.assertEqual(
+                sorted(expected),
+                sorted(list(hash_data[self.rmode.name].keys())),
+            )
 
     def test_data_accumulate(self):
         """
         Type, rank and machine information matters
         """
-        expected = ["type", "storage", "rank", "node", "island"]
+        expected = ["categoryType", "storage", "rank", "node", "island"]
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
-            self.assertEqual(sorted(expected), sorted(list(hash_data[self.rmode.name].keys())))
+            self.assertEqual(
+                sorted(expected),
+                sorted(list(hash_data[self.rmode.name].keys())),
+            )
 
     def test_group_accumulate(self):
         """
         Type, rank and machine information matters
         """
-        expected_app = {"type", "dt", "rank"}
-        expected_file = {"type", "storage", "rank"}
+        expected_app = {"categoryType", "rank"}
+        expected_file = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1162,17 +1310,23 @@
     rmode = ReproducibilityFlags.RECOMPUTE
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Machine information matters when recomputing
         """
         expected = {"node", "island"}
@@ -1191,16 +1345,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Machine information matters when recomputing
         """
-        expected_app = {"type", "dt", "rank"}
-        expected_file = {"type", "storage", "rank"}
+        expected_app = {"categoryType", "rank"}
+        expected_file = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1226,28 +1380,36 @@
     Tests the reproduce standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.REPRODUCE
     expected = {"category", "categoryType"}
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt reproduce data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -1291,27 +1453,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -1403,45 +1574,51 @@
     rmode = ReproducibilityFlags.REPRODUCE
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1470,45 +1647,51 @@
     rmode = ReproducibilityFlags.REPRODUCE
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters
         """
-        expected = ["type"]
+        expected = ["categoryType"]
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, list(hash_data[self.rmode.name].keys()))
 
     def test_data_accumulate(self):
         """
         Only type matters
         """
-        expected = ["type", "storage"]
+        expected = ["categoryType", "storage"]
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, list(hash_data[self.rmode.name].keys()))
 
     def test_group_accumulate(self):
         """
         Only type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1537,17 +1720,23 @@
     rmode = ReproducibilityFlags.REPRODUCE
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         App information does not matter when reproducing
         """
         expected = {}
@@ -1566,16 +1755,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, dict(hash_data[self.rmode.name].keys()))
 
     def test_group_accumulate(self):
         """
         Group information does not matter when reproducing
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1601,35 +1790,39 @@
     Tests the replicate-sci standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.REPLICATE_SCI
     expected = {
         "category",
         "categoryType",
-        "inputPorts",
-        "inputLocalPorts",
-        "outputPorts",
-        "outputLocalPorts",
     }
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt replicate-sci data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -1672,27 +1865,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -1706,18 +1908,18 @@
 
     def test_all_accumulate(self):
         """
         Similar to rerunning. Nothing matters
         """
         self._setup()
         for drop in enumerate(
-                self.lg_node_data
-                + self.lg_files_data
-                + self.lg_group_data
-                + self.lg_misc_data
+            self.lg_node_data
+            + self.lg_files_data
+            + self.lg_group_data
+            + self.lg_misc_data
         ):
             hash_data = accumulate_lg_drop_data(drop[1], self.rmode)
             self.assertEqual(self.expected, dict(hash_data.keys()))
 
 
 class AccumulatePGTUnrollReplicateSciData(unittest.TestCase):
     """
@@ -1729,45 +1931,51 @@
     rmode = ReproducibilityFlags.REPLICATE_SCI
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1796,45 +2004,51 @@
     rmode = ReproducibilityFlags.REPLICATE_SCI
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1863,17 +2077,23 @@
     rmode = ReproducibilityFlags.REPLICATE_SCI
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Nothing matters.
         """
         expected = {}
@@ -1892,16 +2112,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, dict(hash_data[self.rmode.name].keys()))
 
     def test_group_accumulate(self):
         """
         Nothing matters.
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -1927,35 +2147,39 @@
     Tests the replicate-comp standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.REPLICATE_COMP
     expected = {
         "category",
         "categoryType",
-        "inputPorts",
-        "inputLocalPorts",
-        "outputPorts",
-        "outputLocalPorts",
     }
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt replicate-comp data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -1998,27 +2222,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -2056,25 +2289,30 @@
             "removeContainer",
             "additionalBindings",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _component(self, drop):
-        expected = {"execution_time", "num_cpus", "appclass"}
+        expected = {"execution_time", "num_cpus", "dropclass"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _memory(self, drop):
         expected = {"data_volume"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _file(self, drop):
-        expected = {"data_volume", "check_filepath_exists", "filepath", "dirname"}
+        expected = {
+            "data_volume",
+            "check_filepath_exists",
+            "filepath",
+            "dirname",
+        }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _ngas(self, drop):
         expected = {"data_volume"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
@@ -2096,15 +2334,19 @@
             "num_of_copies",
             "scatter_axis",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def _loop(self, drop):
-        expected = {"inputApplicationName", "inputApplicationType", "num_of_iter"}
+        expected = {
+            "inputApplicationName",
+            "inputApplicationType",
+            "num_of_iter",
+        }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def test_all_accumulate(self):
         """
         We make the data expected for each accounted for drop type explicit.
         """
@@ -2129,45 +2371,51 @@
     rmode = ReproducibilityFlags.REPLICATE_COMP
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Type and rank matter
         """
-        expected = {"type", "dt", "rank"}
+        expected = {"categoryType", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Type and rank matter
         """
-        expected = {"type", "storage", "rank"}
+        expected = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Type and rank matter
         """
-        expected_app = {"type", "dt", "rank"}
-        expected_file = {"type", "storage", "rank"}
+        expected_app = {"categoryType", "dt", "rank"}
+        expected_file = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -2195,45 +2443,51 @@
     rmode = ReproducibilityFlags.REPLICATE_COMP
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Type, rank and machine information matters.
         """
-        expected = {"type", "dt", "rank", "node", "island"}
+        expected = {"categoryType", "rank", "node", "island"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Type, rank and machine information matters.
         """
-        expected = {"type", "storage", "rank", "node", "island"}
+        expected = {"categoryType", "storage", "rank", "node", "island"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Type, rank and machine information matters.
         """
-        expected_app = {"type", "dt", "rank"}
-        expected_file = {"type", "storage", "rank"}
+        expected_app = {"categoryType", "dt", "rank"}
+        expected_file = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -2262,17 +2516,23 @@
     rmode = ReproducibilityFlags.REPLICATE_COMP
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Machine information matters.
         """
         expected = {"node", "island"}
@@ -2291,16 +2551,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Machine information matters.
         """
-        expected_app = {"type", "dt", "rank"}
-        expected_file = {"type", "storage", "rank"}
+        expected_app = {"categoryType", "dt", "rank"}
+        expected_file = {"categoryType", "storage", "rank"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -2326,35 +2586,39 @@
     Tests the replicate-total standard at the logical graph template level.
     """
 
     rmode = ReproducibilityFlags.REPLICATE_TOTAL
     expected = {
         "category",
         "categoryType",
-        "inputPorts",
-        "inputLocalPorts",
-        "outputPorts",
-        "outputLocalPorts",
     }
 
     file = "reproducibility/reproGraphs/apps.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_node_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/files.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_files_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/groups.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_groups_data = json.load(f)["nodeDataArray"]
     file = "reproducibility/reproGraphs/misc.graph"
-    with pkg_resources.resource_stream("test", file) as f:  # @UndefinedVariable
-        logger.debug(f"Loading graph: {f}")
+    with pkg_resources.resource_stream(
+        "test", file
+    ) as f:  # @UndefinedVariable
+        # logger.debug(f"Loading graph: {f}")
         lgt_misc_data = json.load(f)["nodeDataArray"]
 
     def test_app_accumulate(self):
         """
         Tests that lgt replicate-total data is collected for application types
         """
         for drop in enumerate(self.lgt_node_data):
@@ -2397,27 +2661,36 @@
     lg_node_data = None
     lg_files_data = None
     lg_group_data = None
     lg_misc_data = None
 
     def _setup(self):
         _fill_workflow(
-            self.rmode, "apps", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "apps",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "files", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "files",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
         _fill_workflow(
             self.rmode,
             "groups",
             "reproducibility/reproGraphs/",
             self.temp_out.name,
         )
         _fill_workflow(
-            self.rmode, "misc", "reproducibility/reproGraphs/", self.temp_out.name
+            self.rmode,
+            "misc",
+            "reproducibility/reproGraphs/",
+            self.temp_out.name,
         )
 
         file = open(self.temp_out.name + "/" + "apps" + "LG.graph")
         self.lg_node_data = json.load(file)["nodeDataArray"]
         file.close()
         file = open(self.temp_out.name + "/" + "files" + "LG.graph")
         self.lg_files_data = json.load(file)["nodeDataArray"]
@@ -2455,15 +2728,15 @@
             "removeContainer",
             "additionalBindings",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _component(self, drop):
-        expected = {"execution_time", "num_cpus", "appclass"}
+        expected = {"execution_time", "num_cpus", "dropclass"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
 
     def _memory(self, drop):
         expected = {"data_volume"}
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data.keys())
@@ -2495,15 +2768,19 @@
             "num_of_copies",
             "scatter_axis",
         }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def _loop(self, drop):
-        expected = {"inputApplicationName", "inputApplicationType", "num_of_iter"}
+        expected = {
+            "inputApplicationName",
+            "inputApplicationType",
+            "num_of_iter",
+        }
         hash_data = accumulate_lg_drop_data(drop, self.rmode)
         self.assertEqual(expected, hash_data)
 
     def test_all_accumulate(self):
         """
         We make the data expected for each accounted for drop type explicit.
         """
@@ -2528,45 +2805,51 @@
     rmode = ReproducibilityFlags.REPLICATE_TOTAL
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGS.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Type matters
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Type matters
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -2595,45 +2878,51 @@
     rmode = ReproducibilityFlags.REPLICATE_TOTAL
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PGT.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "dt"}
+        expected = {"categoryType"}
         self._setup()
         for drop in enumerate(self.graph_data["apps"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_data_accumulate(self):
         """
         Only type matters
         """
-        expected = {"type", "storage"}
+        expected = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["files"]):
             hash_data = accumulate_pgt_partition_drop_data(drop[1])
             self.assertEqual(expected, hash_data[self.rmode.name].keys())
 
     def test_group_accumulate(self):
         """
         Only type matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
@@ -2662,17 +2951,23 @@
     rmode = ReproducibilityFlags.REPLICATE_TOTAL
     temp_out = tempfile.TemporaryDirectory()
     setup = False
     graph_data = None
 
     def _setup(self):
         if not self.setup:
-            _run_workflows(self.rmode, "reproducibility/reproGraphs/", SUPPORTED_WORKFLOWS,
-                           self.temp_out)
-            self.graph_data = _extract_reprodata(self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph")
+            _run_workflows(
+                self.rmode,
+                "reproducibility/reproGraphs/",
+                SUPPORTED_WORKFLOWS,
+                self.temp_out,
+            )
+            self.graph_data = _extract_reprodata(
+                self.temp_out, SUPPORTED_WORKFLOWS, "PG.graph"
+            )
             self.setup = True
 
     def test_app_accumulate(self):
         """
         Nothing matters
         """
         expected = {}
@@ -2691,16 +2986,16 @@
             hash_data = accumulate_pg_drop_data(drop[1])
             self.assertEqual(expected, dict(hash_data[self.rmode.name].keys()))
 
     def test_group_accumulate(self):
         """
         Nothing matters
         """
-        expected_app = {"type", "dt"}
-        expected_file = {"type", "storage"}
+        expected_app = {"categoryType", "dt"}
+        expected_file = {"categoryType", "storage"}
         self._setup()
         for drop in enumerate(self.graph_data["groups"]):
             hash_data = accumulate_pgt_unroll_drop_data(drop[1])
             if "dt" in hash_data.keys():
                 self.assertEqual(expected_app, hash_data.keys())
             if "storage" in hash_data.keys():
                 self.assertEqual(expected_file, hash_data.keys())
```

### Comparing `daliuge-translator-2.4.0/test/reproducibility/test_integration.py` & `daliuge-translator-3.0.0/test/reproducibility/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,39 +24,66 @@
 happen.
 """
 import json
 import optparse
 import tempfile
 import unittest
 import pkg_resources
+import logging
 
-from dlg.common.reproducibility.constants import ReproducibilityFlags, ALL_RMODES
-from dlg.translator.tool_commands import dlg_fill, dlg_unroll, dlg_partition, dlg_map
+
+from dlg.common.reproducibility.constants import (
+    ReproducibilityFlags,
+    ALL_RMODES,
+)
+from dlg.translator.tool_commands import (
+    dlg_fill,
+    dlg_unroll,
+    dlg_partition,
+    dlg_map,
+)
+
+logger = logging.getLogger("__name__")
 
 
 def _run_full_workflow(
-        rmode: ReproducibilityFlags, workflow: str, workflow_loc="./", scratch_loc="./"
+    rmode: ReproducibilityFlags,
+    workflow: str,
+    workflow_loc="./",
+    scratch_loc="./",
 ):
     workflow_loc = pkg_resources.resource_filename("test", workflow_loc)
     lgt = workflow_loc + "/" + workflow + ".graph"
     lgr = scratch_loc + "/" + workflow + "_" + str(rmode.value) + "LG.graph"
     pgs = scratch_loc + "/" + workflow + "_" + str(rmode.value) + "PGS.graph"
     pgt = scratch_loc + "/" + workflow + "_" + str(rmode.value) + "PGT.graph"
     pgr = scratch_loc + "/" + workflow + "_" + str(rmode.value) + "PG.graph"
 
     rmodes = str(rmode.value)
     parser = optparse.OptionParser()
-    dlg_fill(parser, ["-L", lgt, "-R", rmodes, "-o", lgr, "-f", "newline"])
+    ll = ""
+    dlg_fill(parser, ["-L", lgt, "-R", rmodes, "-o", lgr, "-f", "newline", ll])
     parser = optparse.OptionParser()
-    dlg_unroll(parser, ["-L", lgr, "-o", pgs, "-f", "newline"])
+    dlg_unroll(parser, ["-L", lgr, "-o", pgs, "-f", "newline", ll])
     parser = optparse.OptionParser()
-    dlg_partition(parser, ["-P", pgs, "-o", pgt, "-f", "newline"])
+    dlg_partition(parser, ["-P", pgs, "-o", pgt, "-f", "newline", ll])
     parser = optparse.OptionParser()
     dlg_map(
-        parser, ["-P", pgt, "-N", "localhost, localhost", "-o", pgr, "-f", "newline"]
+        parser,
+        [
+            "-P",
+            pgt,
+            "-N",
+            "localhost, localhost",
+            "-o",
+            pgr,
+            "-f",
+            "newline",
+            ll,
+        ],
     )
 
 
 def _read_graph(filename):
     file = open(filename)
     graph = json.load(file)
     file.close()
@@ -82,27 +109,36 @@
         _run_full_workflow(
             rmode=rmode,
             workflow=graph_name,
             workflow_loc=graph_loc,
             scratch_loc=self.temp_out.name,
         )
 
-        for filename in ['PGS', 'PGT', 'PG']:
+        for filename in ["PGS", "PGT", "PG"]:
             pgr = (
-                    self.temp_out.name + "/" + graph_name + "_" + str(
-                rmode.value) + f"{filename}.graph"
+                self.temp_out.name
+                + "/"
+                + graph_name
+                + "_"
+                + str(rmode.value)
+                + f"{filename}.graph"
             )
             graph = _read_graph(pgr)
             for drop in graph:
                 if "reprodata" in drop:
                     self.assertIn("0", drop["reprodata"]["rmode"])
                 else:
                     self.assertIn("rmode", drop)
         lgr = (
-                self.temp_out.name + "/" + graph_name + "_" + str(rmode.value) + "LG.graph"
+            self.temp_out.name
+            + "/"
+            + graph_name
+            + "_"
+            + str(rmode.value)
+            + "LG.graph"
         )
         graph = _read_graph(lgr)
         for drop in graph["nodeDataArray"]:
             self.assertIn("reprodata", drop)
 
 
 class IntegrationHelloWorldTest(unittest.TestCase):
@@ -484,30 +520,32 @@
         self._process_graphs(rmode)
         for rmode in ALL_RMODES:
             self._process_graphs(rmode)
         for graph in self.graphs:
             for rmode in ALL_RMODES:
                 self.assertEqual(
                     self.graphs[graph][rmode.value],
-                    self.graphs[graph][ReproducibilityFlags.ALL.value][rmode.name][
-                        "signature"
-                    ],
+                    self.graphs[graph][ReproducibilityFlags.ALL.value][
+                        rmode.name
+                    ]["signature"],
                 )
 
 
 class IntegrationSplitRmode(unittest.TestCase):
     """
     It is not unreasonable for different reproducibility standards enforced on different drops in
     a single workflow.
     This test class tests this functionality.
     """
 
     temp_out = tempfile.TemporaryDirectory("out")
 
-    @unittest.skip("Individual rmodes not yet supported again (needs re-working)")
+    @unittest.skip(
+        "Individual rmodes not yet supported again (needs re-working)"
+    )
     def test_split_lgt(self):
         """
         Tests a simple 'hello world' graph (HelloWorldBash) where a single component has
         a pre-existing rmode in the graph file set (Replicate Computationally).
         The rest are run with a NOTHING standard.
         We should be able to tell:
           - This graph's signature should be different to the standard graph run completely in
@@ -521,44 +559,63 @@
         _run_full_workflow(
             rmode=rmode,
             workflow=graph_name,
             workflow_loc=graph_loc,
             scratch_loc=self.temp_out.name,
         )
         pgr = (
-                self.temp_out.name + "/" + graph_name + "_" + str(rmode.value) + "PG.graph"
+            self.temp_out.name
+            + "/"
+            + graph_name
+            + "_"
+            + str(rmode.value)
+            + "PG.graph"
         )
         _run_full_workflow(
             rmode=rmode,
             workflow=control_graph_name,
             workflow_loc=graph_loc,
             scratch_loc=self.temp_out.name,
         )
         pgr_2 = (
-                self.temp_out.name
-                + "/"
-                + control_graph_name
-                + "_"
-                + str(rmode.value)
-                + "PG.graph"
+            self.temp_out.name
+            + "/"
+            + control_graph_name
+            + "_"
+            + str(rmode.value)
+            + "PG.graph"
         )
 
         graph = _read_graph(pgr)
         graph_reprodata = graph[-1]
         graph = graph[0:-1]
         control_graph = _read_graph(pgr_2)
         control_signature = control_graph[-1]["signature"]
         self.assertEqual(
             ReproducibilityFlags.RERUN.value, int(graph_reprodata["rmode"])
         )
 
         for drop in graph:
-            if drop["reprodata"]["rmode"] == str(ReproducibilityFlags.RERUN.value):
-                self.assertIsNotNone(drop["reprodata"]["lgt_data"]["merkleroot"])
+            if drop["reprodata"]["rmode"] == str(
+                ReproducibilityFlags.RERUN.value
+            ):
+                self.assertIsNotNone(
+                    drop["reprodata"]["lgt_data"]["merkleroot"]
+                )
                 self.assertIsNone(drop["reprodata"]["lg_data"]["merkleroot"])
-                self.assertIsNotNone(drop["reprodata"]["pgt_data"]["merkleroot"])
+                self.assertIsNotNone(
+                    drop["reprodata"]["pgt_data"]["merkleroot"]
+                )
                 self.assertIsNone(drop["reprodata"]["pg_data"]["merkleroot"])
             else:
-                self.assertIsNotNone(drop["reprodata"]["lgt_data"]["merkleroot"])
-                self.assertIsNotNone(drop["reprodata"]["lg_data"]["merkleroot"])
-                self.assertIsNotNone(drop["reprodata"]["pgt_data"]["merkleroot"])
-                self.assertIsNotNone(drop["reprodata"]["pg_data"]["merkleroot"])
+                self.assertIsNotNone(
+                    drop["reprodata"]["lgt_data"]["merkleroot"]
+                )
+                self.assertIsNotNone(
+                    drop["reprodata"]["lg_data"]["merkleroot"]
+                )
+                self.assertIsNotNone(
+                    drop["reprodata"]["pgt_data"]["merkleroot"]
+                )
+                self.assertIsNotNone(
+                    drop["reprodata"]["pg_data"]["merkleroot"]
+                )
```

### Comparing `daliuge-translator-2.4.0/test/reproducibility/test_json_output.py` & `daliuge-translator-3.0.0/test/reproducibility/test_json_output.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/test/reproducibility/test_repro_inits.py` & `daliuge-translator-3.0.0/test/reproducibility/test_repro_inits.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/test/reproducibility/test_reprodata_compare.py` & `daliuge-translator-3.0.0/test/reproducibility/test_reprodata_compare.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/test/reproducibility/test_scatter_blockdag.py` & `daliuge-translator-3.0.0/test/reproducibility/test_scatter_blockdag.py`

 * *Files identical despite different names*

### Comparing `daliuge-translator-2.4.0/test/test_tool_trans.py` & `daliuge-translator-3.0.0/test/test_tool_trans.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,27 +28,53 @@
 from dlg.common import tool
 
 
 class TestTool(unittest.TestCase):
     def test_pipeline(self):
         """A pipeline from an LG all the way to a finished graph execution"""
         lg = pkg_resources.resource_filename(  # @UndefinedVariable
-            "test.dropmake", "logical_graphs/cont_img.graph"
+            "test.dropmake", "logical_graphs/ArrayLoop.graph"
         )
 
-        fill = tool.start_process("fill", ["-L", lg], stdout=subprocess.PIPE)
+        # first fill the LGT parameters
+        fill = tool.start_process(
+            "fill",
+            [
+                "-vv",
+                "-L",
+                lg,
+                "-p",
+                "param1=hello",
+                "-p",
+                "param2=1",
+                "-p",
+                "param1.param2=hi",
+                "-p",
+                "param4.what=False",
+            ],
+            stdout=subprocess.PIPE,
+        )
+
+        # unroll the resulting LG
         unroll = tool.start_process(
-            "unroll", ["-z", "--app", "1"], stdin=fill.stdout, stdout=subprocess.PIPE
+            "unroll",
+            ["-z", "--app", "1", "-vv"],
+            stdin=fill.stdout,
+            stdout=subprocess.PIPE,
         )
+
+        # partition the PGT
         partition = tool.start_process(
             "partition", stdin=unroll.stdout, stdout=subprocess.PIPE
         )
+
+        # map PGT to resources to construct PG
         map_ = tool.start_process(
             "map",
-            ["-N", "localhost,localhost"],
+            ["-vv", "-N", "localhost,localhost"],
             stdin=partition.stdout,
             stdout=subprocess.PIPE,
         )
         mapped_graph, _ = map_.communicate()
 
         for proc in fill, unroll, partition, map_:
             self.assertEqual(proc.wait(), 0)
```

