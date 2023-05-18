# Comparing `tmp/singlestoredb-0.6.0.tar.gz` & `tmp/singlestoredb-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-0.6.0.tar", last modified: Wed May 17 16:26:00 2023, max compression
+gzip compressed data, was "singlestoredb-0.6.1.tar", last modified: Thu May 18 20:51:00 2023, max compression
```

## Comparing `singlestoredb-0.6.0.tar` & `singlestoredb-0.6.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.839447 singlestoredb-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-05-17 16:26:00.839447 singlestoredb-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-05-17 16:26:00.839447 singlestoredb-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.827447 singlestoredb-0.6.0/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7502 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    42815 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12165 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.827447 singlestoredb-0.6.0/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27455 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.831447 singlestoredb-0.6.0/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.831447 singlestoredb-0.6.0/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8052 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/accel.c
--rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (122)    58654 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.831447 singlestoredb-0.6.0/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.835447 singlestoredb-0.6.0/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.835447 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.835447 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/mysql/times.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.835447 singlestoredb-0.6.0/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/empty.sql
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8718 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test.sql
--rwxr-xr-x   0 runner    (1001) docker     (122)    36300 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    49962 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_management.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.839447 singlestoredb-0.6.0/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23746 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-05-17 16:25:35.000000 singlestoredb-0.6.0/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 16:26:00.827447 singlestoredb-0.6.0/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-05-17 16:26:00.000000 singlestoredb-0.6.0/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-17 16:26:00.000000 singlestoredb-0.6.0/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 16:26:00.000000 singlestoredb-0.6.0/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-17 16:26:00.000000 singlestoredb-0.6.0/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-17 16:26:00.000000 singlestoredb-0.6.0/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-05-18 20:51:00.596263 singlestoredb-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.572262 singlestoredb-0.6.1/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7502 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42815 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12165 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.572262 singlestoredb-0.6.1/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27455 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.576262 singlestoredb-0.6.1/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.580262 singlestoredb-0.6.1/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/accel.c
+-rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58505 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.580262 singlestoredb-0.6.1/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.584262 singlestoredb-0.6.1/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.584262 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.588263 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/empty.sql
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     8718 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test.sql
+-rwxr-xr-x   0 runner    (1001) docker     (122)    36300 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    49962 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.592263 singlestoredb-0.6.1/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23746 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-05-18 20:50:36.000000 singlestoredb-0.6.1/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:51:00.572262 singlestoredb-0.6.1/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-18 20:51:00.000000 singlestoredb-0.6.1/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-0.6.0/LICENSE` & `singlestoredb-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/PKG-INFO` & `singlestoredb-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-0.6.0/README.md` & `singlestoredb-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/setup.cfg` & `singlestoredb-0.6.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 0.6.0
+version = 0.6.1
 description = Interface to the SingleStore database and cluster management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-0.6.0/setup.py` & `singlestoredb-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/__init__.py` & `singlestoredb-0.6.1/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '0.6.0'
+__version__ = '0.6.1'
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
     IntegrityError, InternalError, ProgrammingError, NotSupportedError,
     DataError, ManagementError,
```

### Comparing `singlestoredb-0.6.0/singlestoredb/auth.py` & `singlestoredb-0.6.1/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/config.py` & `singlestoredb-0.6.1/singlestoredb/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/connection.py` & `singlestoredb-0.6.1/singlestoredb/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/converters.py` & `singlestoredb-0.6.1/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/exceptions.py` & `singlestoredb-0.6.1/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/http/__init__.py` & `singlestoredb-0.6.1/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/http/connection.py` & `singlestoredb-0.6.1/singlestoredb/http/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/management/cluster.py` & `singlestoredb-0.6.1/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/management/manager.py` & `singlestoredb-0.6.1/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/management/region.py` & `singlestoredb-0.6.1/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/management/utils.py` & `singlestoredb-0.6.1/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/management/workspace.py` & `singlestoredb-0.6.1/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/__init__.py` & `singlestoredb-0.6.1/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/_auth.py` & `singlestoredb-0.6.1/singlestoredb/mysql/_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # type: ignore
 """
 Implements auth methods
 """
-import getpass
-
 from .err import OperationalError
 
 try:
     from cryptography.hazmat.backends import default_backend
     from cryptography.hazmat.primitives import serialization, hashes
     from cryptography.hazmat.primitives.asymmetric import padding
 
@@ -272,30 +270,27 @@
         if DEBUG:
             print(conn.server_public_key.decode('ascii'))
 
     data = sha2_rsa_encrypt(conn.password, conn.salt, conn.server_public_key)
     pkt = _roundtrip(conn, data)
 
 
-def gssapi_auth(user):
+def gssapi_auth(data):
     try:
         import gssapi.raw
     except ImportError:
         raise ImportError(
             'The `gssapi` package must be '
             'installed for Kerberos authentication',
         )
 
-    if not user:
-        user = getpass.getuser()
-
     ctx = None
     try:
         ctx = gssapi.raw.init_sec_context(
-            gssapi.raw.import_name(user, gssapi.raw.NameType.user),
+            gssapi.raw.import_name(data, gssapi.raw.NameType.user),
             flags=[0], lifetime=0,
         )
         return ctx.token
 
     finally:
         if ctx is not None:
             gssapi.raw.delete_sec_context(ctx.context)
```

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/accel.c` & `singlestoredb-0.6.1/singlestoredb/mysql/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/charset.py` & `singlestoredb-0.6.1/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/connection.py` & `singlestoredb-0.6.1/singlestoredb/mysql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1107,17 +1107,14 @@
             plugin_name = b'sha256_password'
             if self.ssl and self.server_capabilities & CLIENT.SSL:
                 authresp = self.password + b'\0'
             elif self.password:
                 authresp = b'\1'  # request public key
             else:
                 authresp = b'\0'  # empty password
-        elif self._auth_plugin_name == b'auth_gssapi_client':
-            plugin_name = b'auth_gssapi_client'
-            authresp = _auth.gssapi_auth(self.user)
 
         if self.server_capabilities & CLIENT.PLUGIN_AUTH_LENENC_CLIENT_DATA:
             data += _lenenc_int(len(authresp)) + authresp
         elif self.server_capabilities & CLIENT.SECURE_CONNECTION:
             data += struct.pack('B', len(authresp)) + authresp
         else:  # pragma: no cover - no testing against servers w/o secure auth (>=5.0)
             data += authresp + b'\0'
@@ -1199,15 +1196,15 @@
                 _auth.scramble_old_password(self.password, auth_packet.read_all())
                 + b'\0'
             )
         elif plugin_name == b'mysql_clear_password':
             # https://dev.mysql.com/doc/internals/en/clear-text-authentication.html
             data = self.password + b'\0'
         elif plugin_name == b'auth_gssapi_client':
-            data = _auth.gssapi_auth(self.user)
+            data = _auth.gssapi_auth(auth_packet.read_all())
         elif plugin_name == b'dialog':
             pkt = auth_packet
             while True:
                 flag = pkt.read_uint8()
                 echo = (flag & 0x06) == 0x02
                 last = (flag & 0x01) == 0x01
                 prompt = pkt.read_all()
```

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-0.6.1/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-0.6.1/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/constants/CR.py` & `singlestoredb-0.6.1/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/constants/ER.py` & `singlestoredb-0.6.1/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/converters.py` & `singlestoredb-0.6.1/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/cursors.py` & `singlestoredb-0.6.1/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/err.py` & `singlestoredb-0.6.1/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/optionfile.py` & `singlestoredb-0.6.1/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/protocol.py` & `singlestoredb-0.6.1/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/base.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-0.6.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test.sql` & `singlestoredb-0.6.1/singlestoredb/tests/test.sql`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_basics.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_config.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_connection.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_dbapi.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_exceptions.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_http.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_management.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_results.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_types.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/test_xdict.py` & `singlestoredb-0.6.1/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/tests/utils.py` & `singlestoredb-0.6.1/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/types.py` & `singlestoredb-0.6.1/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/utils/config.py` & `singlestoredb-0.6.1/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/utils/convert_rows.py` & `singlestoredb-0.6.1/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/utils/results.py` & `singlestoredb-0.6.1/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb/utils/xdict.py` & `singlestoredb-0.6.1/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.6.0/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-0.6.1/singlestoredb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-0.6.0/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-0.6.1/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

