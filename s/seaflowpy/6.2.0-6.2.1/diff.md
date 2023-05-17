# Comparing `tmp/seaflowpy-6.2.0.tar.gz` & `tmp/seaflowpy-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaflowpy-6.2.0.tar", last modified: Mon Oct 31 23:38:08 2022, max compression
+gzip compressed data, was "seaflowpy-6.2.1.tar", last modified: Wed May 17 22:09:20 2023, max compression
```

## Comparing `seaflowpy-6.2.0.tar` & `seaflowpy-6.2.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:08.007410 seaflowpy-6.2.0/
--rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-6.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-6.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6808 2022-10-31 23:38:08.007410 seaflowpy-6.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-6.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)      245 2022-10-31 23:38:08.008410 seaflowpy-6.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-6.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.968410 seaflowpy-6.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:08.008410 seaflowpy-6.2.0/src/seaflowpy/
--rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-6.2.0/src/seaflowpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-10-31 23:38:08.008410 seaflowpy-6.2.0/src/seaflowpy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.981410 seaflowpy-6.2.0/src/seaflowpy/cli/
--rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-6.2.0/src/seaflowpy/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-6.2.0/src/seaflowpy/cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.985410 seaflowpy-6.2.0/src/seaflowpy/cli/commands/
--rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/dayofyear_cmd.py
--rw-r--r--   0 root         (0) root         (0)     5296 2020-07-19 21:48:09.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/db_cmd.py
--rw-r--r--   0 root         (0) root         (0)    12247 2022-10-28 22:17:48.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/evt_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/filter_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/opp_cmd.py
--rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-6.2.0/src/seaflowpy/cli/commands/version_cmd.py
--rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-6.2.0/src/seaflowpy/cloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.986410 seaflowpy-6.2.0/src/seaflowpy/data/
--rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-6.2.0/src/seaflowpy/data/popcycle.sql
--rw-r--r--   0 root         (0) root         (0)    11780 2022-02-18 01:01:04.000000 seaflowpy-6.2.0/src/seaflowpy/db.py
--rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-6.2.0/src/seaflowpy/errors.py
--rw-r--r--   0 root         (0) root         (0)    13696 2022-08-22 23:54:55.000000 seaflowpy-6.2.0/src/seaflowpy/fileio.py
--rw-r--r--   0 root         (0) root         (0)    13776 2022-04-21 21:40:19.000000 seaflowpy-6.2.0/src/seaflowpy/filterevt.py
--rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-6.2.0/src/seaflowpy/geo.py
--rw-r--r--   0 root         (0) root         (0)    11162 2022-10-31 23:04:02.000000 seaflowpy-6.2.0/src/seaflowpy/particleops.py
--rw-r--r--   0 root         (0) root         (0)    10280 2022-10-31 23:12:46.000000 seaflowpy-6.2.0/src/seaflowpy/sample.py
--rw-r--r--   0 root         (0) root         (0)     9411 2022-08-18 22:28:13.000000 seaflowpy-6.2.0/src/seaflowpy/seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)    19660 2022-02-18 18:25:23.000000 seaflowpy-6.2.0/src/seaflowpy/sfl.py
--rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-6.2.0/src/seaflowpy/time.py
--rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-6.2.0/src/seaflowpy/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.980410 seaflowpy-6.2.0/src/seaflowpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6808 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2961 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-31 23:38:07.000000 seaflowpy-6.2.0/src/seaflowpy.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.989410 seaflowpy-6.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-6.2.0/tests/file_dates.parquet
--rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-6.2.0/tests/sfl.parquet
--rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-6.2.0/tests/test_evtopp.py
--rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-6.2.0/tests/test_geo.py
--rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-6.2.0/tests/test_sample.py
--rw-r--r--   0 root         (0) root         (0)    18787 2022-02-18 18:39:19.000000 seaflowpy-6.2.0/tests/test_seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-6.2.0/tests/test_time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.969410 seaflowpy-6.2.0/tests/testcruise_evt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.997410 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:07.969410 seaflowpy-6.2.0/tests/testcruise_evt_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:08.005410 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
--rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-6.2.0/tests/testcruise_full_one_param.db
--rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-6.2.0/tests/testcruise_full_plan.db
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:08.006410 seaflowpy-6.2.0/tests/testcruise_opp_one_param/
--rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-6.2.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-6.2.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-31 23:38:08.007410 seaflowpy-6.2.0/tests/testcruise_opp_plan/
--rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-6.2.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-6.2.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-6.2.0/tests/testcruise_paramsonly_one_param.db
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-6.2.0/tests/testcruise_paramsonly_plan.db
--rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-6.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.614244 seaflowpy-6.2.1/
+-rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-6.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-6.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-05-17 22:09:20.614244 seaflowpy-6.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-6.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-17 22:09:20.614244 seaflowpy-6.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-6.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.579244 seaflowpy-6.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.615244 seaflowpy-6.2.1/src/seaflowpy/
+-rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-6.2.1/src/seaflowpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 22:09:20.615244 seaflowpy-6.2.1/src/seaflowpy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.589244 seaflowpy-6.2.1/src/seaflowpy/cli/
+-rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-6.2.1/src/seaflowpy/cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.591244 seaflowpy-6.2.1/src/seaflowpy/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/dayofyear_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2020-07-19 21:48:09.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/db_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2022-10-28 22:17:48.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/evt_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/filter_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/opp_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/sds2sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/version_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-6.2.1/src/seaflowpy/cloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.592244 seaflowpy-6.2.1/src/seaflowpy/data/
+-rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-6.2.1/src/seaflowpy/data/popcycle.sql
+-rw-r--r--   0 root         (0) root         (0)    11780 2022-02-18 01:01:04.000000 seaflowpy-6.2.1/src/seaflowpy/db.py
+-rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-6.2.1/src/seaflowpy/errors.py
+-rw-r--r--   0 root         (0) root         (0)    13696 2022-08-22 23:54:55.000000 seaflowpy-6.2.1/src/seaflowpy/fileio.py
+-rw-r--r--   0 root         (0) root         (0)    13776 2022-04-21 21:40:19.000000 seaflowpy-6.2.1/src/seaflowpy/filterevt.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/geo.py
+-rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-6.2.1/src/seaflowpy/particleops.py
+-rw-r--r--   0 root         (0) root         (0)    10280 2022-10-31 23:12:46.000000 seaflowpy-6.2.1/src/seaflowpy/sample.py
+-rw-r--r--   0 root         (0) root         (0)     9411 2022-08-18 22:28:13.000000 seaflowpy-6.2.1/src/seaflowpy/seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-6.2.1/src/seaflowpy/sfl.py
+-rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-6.2.1/src/seaflowpy/time.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-6.2.1/src/seaflowpy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.588244 seaflowpy-6.2.1/src/seaflowpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.596244 seaflowpy-6.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-6.2.1/tests/file_dates.parquet
+-rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-6.2.1/tests/sfl.parquet
+-rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-6.2.1/tests/test_evtopp.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-6.2.1/tests/test_geo.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-6.2.1/tests/test_sample.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2022-02-18 18:39:19.000000 seaflowpy-6.2.1/tests/test_seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-6.2.1/tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.580244 seaflowpy-6.2.1/tests/testcruise_evt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.604244 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.580244 seaflowpy-6.2.1/tests/testcruise_evt_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.612244 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-6.2.1/tests/testcruise_full_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-6.2.1/tests/testcruise_full_plan.db
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.613244 seaflowpy-6.2.1/tests/testcruise_opp_one_param/
+-rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.613244 seaflowpy-6.2.1/tests/testcruise_opp_plan/
+-rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-6.2.1/tests/testcruise_paramsonly_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-6.2.1/tests/testcruise_paramsonly_plan.db
+-rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-6.2.1/versioneer.py
```

### Comparing `seaflowpy-6.2.0/LICENSE` & `seaflowpy-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/PKG-INFO` & `seaflowpy-6.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 6.2.0
+Version: 6.2.1
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Seaflowpy
 
@@ -246,9 +244,7 @@
 ```
 
 Leave the virtual environment
 
 ```sh
 deactivate
 ```
-
-
```

### Comparing `seaflowpy-6.2.0/README.md` & `seaflowpy-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/setup.py` & `seaflowpy-6.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/cli.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/dayofyear_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/dayofyear_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/db_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/db_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/evt_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/evt_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/filter_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/filter_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/opp_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/opp_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/sds2sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cli/commands/sfl_cmd.py` & `seaflowpy-6.2.1/src/seaflowpy/cli/commands/sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/cloud.py` & `seaflowpy-6.2.1/src/seaflowpy/cloud.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/data/popcycle.sql` & `seaflowpy-6.2.1/src/seaflowpy/data/popcycle.sql`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/db.py` & `seaflowpy-6.2.1/src/seaflowpy/db.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/fileio.py` & `seaflowpy-6.2.1/src/seaflowpy/fileio.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/filterevt.py` & `seaflowpy-6.2.1/src/seaflowpy/filterevt.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/geo.py` & `seaflowpy-6.2.1/src/seaflowpy/geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/particleops.py` & `seaflowpy-6.2.1/src/seaflowpy/particleops.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     if len(set(list(df)).intersection(set(["D1", "D2", "fsc_small"]))) < 3:
         raise ValueError("Can't apply noise filter without D1, D2, and fsc_small")
 
     # Mark noise events in new column "noise"
     return ~((df["fsc_small"].values > 1) | (df["D1"].values > 1) | (df["D2"].values > 1))
 
 
-def mark_saturated(df, cols=["D1", "D2"]):
+def mark_saturated(df, cols=None):
     """
     Mark data that saturates D1 or D2.
 
     This function returns a boolean Series marking events where
     D1 == max(D1) or D2 == max(D2).
 
     Parameters
@@ -163,14 +163,16 @@
         Columns to test for saturation.
 
     Returns
     -------
     numpy.ndarray
         Boolean array of saturated events.
     """
+    if cols is None:
+        cols = ["D1", "D2"]
     if len(set(list(df)).intersection(set(cols))) < len(cols):
         raise ValueError("Some columns requested are not present in df")
     if len(df.index) == 0:
         return np.full(len(df.index), False)
     else:
         idx = False
         for col in cols:
```

### Comparing `seaflowpy-6.2.0/src/seaflowpy/sample.py` & `seaflowpy-6.2.1/src/seaflowpy/sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/seaflowfile.py` & `seaflowpy-6.2.1/src/seaflowpy/seaflowfile.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/sfl.py` & `seaflowpy-6.2.1/src/seaflowpy/sfl.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         errors.append(create_error(df, "date", msg="date column is missing"))
     else:
         # All dates must match RFC 3339 with no fractional seconds
         # only integer seconds.
         date_flags = df["date"].map(check_date_string)
         if len(date_flags) > 0:
             # select rows that failed date check
-            for i, v in df[~date_flags]["date"].iteritems():
+            for i, v in df[~date_flags]["date"].items():
                 errors.append(create_error(df, "date", msg="Invalid date format", row=i, val=v))
     return errors
 
 
 def check_date_string(date):
     """Confirm value is an RFC3339 string with UTC timezone as [+-]00:00"""
     passed = False
@@ -139,34 +139,34 @@
             if s.path_dayofyear:
                 return True
             return False
 
         good_files_selector = df["file"].map(parse_filename)
         good_files = df[good_files_selector]
         bad_files = df[~good_files_selector]
-        for i, v in bad_files["file"].iteritems():
+        for i, v in bad_files["file"].items():
             errors.append(create_error(bad_files, "file", msg="Invalid file name", row=i, val=v))
 
         # Files must be unique
         dup_files = df.loc[df["file"].duplicated(keep=False), "file"]
-        for i, v in dup_files.iteritems():
+        for i, v in dup_files.items():
             errors.append(create_error(dup_files, "file", msg="Duplicate file", row=i, val=v))
 
         # Files should be in order
         # Only consider files that are parseable by seaflowfile.SeaFlowFile
         inorder = seaflowfile.sorted_files(good_files["file"])
         files_equal = good_files["file"] == inorder
         if not files_equal.all():
             i = int(good_files[~files_equal].index[0])
             v = "First out of order file {}".format(good_files.loc[i, "file"])
             errors.append(create_error(good_files, "file", msg="Files out of order", row=i, val=v))
 
         # Files should match date in same row
         if "date" in df.columns:
-            for i, v in good_files["file"].iteritems():
+            for i, v in good_files["file"].items():
                 s = seaflowfile.SeaFlowFile(v)
                 d = good_files.loc[i, "date"]
                 if s.is_new_style and s.rfc3339 != d:
                     errors.append(create_error(good_files, "file/date", msg="File and date don't match", row=i, val=f"{v} {d}"))
 
     return errors
 
@@ -213,31 +213,31 @@
         if minval is not None:
             good_selector = good_selector & (numbers >= minval)
         if maxval is not None:
             good_selector = good_selector & (numbers <= maxval)
         # Catch values outside correct range
         # Catch non-numeric values (NAs created during to_numeric())
         bad_numbers = notnas.loc[~good_selector, colname]
-        for i, v in bad_numbers.iteritems():
+        for i, v in bad_numbers.items():
             errors.append(create_error(df, colname, msg=f"Invalid {colname}", row=i, val=v, level="error"))
 
         nas = df.loc[df[colname].isna(), colname]
         if len(nas) == len(df):
             # No data in column
             if require_all or require_some:
                 errors.append(create_error(df, colname, msg=f"{colname} column has no data", level="error"))
             else:
                 errors.append(create_error(df, colname, msg=f"{colname} column has no data", level="warning"))
         elif len(nas) > 0:
             # Some missing
             if require_all:
-                for i, v in nas.iteritems():
+                for i, v in nas.items():
                     errors.append(create_error(df, colname, msg="Missing required data", row=i, val=v, level="error"))
             elif warn_missing:
-                for i, v in nas.iteritems():
+                for i, v in nas.items():
                     errors.append(create_error(df, colname, msg="Missing data", row=i, val=v, level="warning"))
 
     return errors
 
 
 def convert_gga2dd(df):
     """Return a copy of df with coordinates converted from GGA to decimal degrees."""
```

### Comparing `seaflowpy-6.2.0/src/seaflowpy/time.py` & `seaflowpy-6.2.1/src/seaflowpy/time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy/util.py` & `seaflowpy-6.2.1/src/seaflowpy/util.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/src/seaflowpy.egg-info/PKG-INFO` & `seaflowpy-6.2.1/src/seaflowpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 6.2.0
+Version: 6.2.1
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Seaflowpy
 
@@ -246,9 +244,7 @@
 ```
 
 Leave the virtual environment
 
 ```sh
 deactivate
 ```
-
-
```

### Comparing `seaflowpy-6.2.0/src/seaflowpy.egg-info/SOURCES.txt` & `seaflowpy-6.2.1/src/seaflowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/file_dates.parquet` & `seaflowpy-6.2.1/tests/file_dates.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/sfl.parquet` & `seaflowpy-6.2.1/tests/sfl.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/test_evtopp.py` & `seaflowpy-6.2.1/tests/test_evtopp.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/test_geo.py` & `seaflowpy-6.2.1/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/test_sample.py` & `seaflowpy-6.2.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/test_seaflowfile.py` & `seaflowpy-6.2.1/tests/test_seaflowfile.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/test_time.py` & `seaflowpy-6.2.1/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_full_one_param.db` & `seaflowpy-6.2.1/tests/testcruise_full_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_full_plan.db` & `seaflowpy-6.2.1/tests/testcruise_full_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_paramsonly_one_param.db` & `seaflowpy-6.2.1/tests/testcruise_paramsonly_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/tests/testcruise_paramsonly_plan.db` & `seaflowpy-6.2.1/tests/testcruise_paramsonly_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.0/versioneer.py` & `seaflowpy-6.2.1/versioneer.py`

 * *Files identical despite different names*

