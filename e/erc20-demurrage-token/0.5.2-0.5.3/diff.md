# Comparing `tmp/erc20-demurrage-token-0.5.2.tar.gz` & `tmp/erc20-demurrage-token-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erc20-demurrage-token-0.5.2.tar", last modified: Sun Mar 26 07:25:21 2023, max compression
+gzip compressed data, was "erc20-demurrage-token-0.5.3.tar", last modified: Thu May 18 05:45:10 2023, max compression
```

## Comparing `erc20-demurrage-token-0.5.2.tar` & `erc20-demurrage-token-0.5.3.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-03-22 12:57:15.000000 erc20-demurrage-token-0.5.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-08-24 19:49:18.000000 erc20-demurrage-token-0.5.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      754 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token/
--rw-r--r--   0 lash      (1000) lash      (1000)      198 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/.chainlib
--rw-r--r--   0 lash      (1000) lash      (1000)    52656 2023-03-26 07:25:08.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/DemurrageTokenSingleNocap.bin
--rw-r--r--   0 lash      (1000) lash      (1000)    17193 2023-03-26 07:25:08.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/DemurrageTokenSingleNocap.json
--rw-r--r--   0 lash      (1000) lash      (1000)    18252 2023-03-26 07:25:08.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/DemurrageTokenSingleNocap.metadata.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-03-22 09:00:20.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-12-21 10:17:58.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/config/eth.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2021-12-21 10:17:58.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/config/session.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      142 2021-12-21 10:17:58.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/config/token.ini
--rw-r--r--   0 lash      (1000) lash      (1000)     2738 2023-03-22 08:00:10.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/demurrage.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1046 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/expiry.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     6028 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/runnable/publish.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1825 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/seal.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token/sim/
--rw-r--r--   0 lash      (1000) lash      (1000)       78 2021-06-06 07:35:49.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/sim/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)       47 2021-06-06 07:35:49.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/sim/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)    11875 2021-10-24 14:29:58.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/sim/sim.py
--rw-r--r--   0 lash      (1000) lash      (1000)    23772 2023-03-22 08:59:54.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/token.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-10 09:14:53.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5227 2023-03-22 10:12:31.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4854 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token/unittest/newbase.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      754 2023-03-26 07:25:21.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1444 2023-03-26 07:25:21.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-26 07:25:21.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       94 2023-03-26 07:25:21.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       85 2023-03-26 07:25:21.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2023-03-26 07:25:21.000000 erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       85 2023-03-22 10:23:09.000000 erc20-demurrage-token-0.5.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1121 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      620 2021-05-06 08:36:15.000000 erc20-demurrage-token-0.5.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-08-24 19:49:18.000000 erc20-demurrage-token-0.5.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:25:21.443322 erc20-demurrage-token-0.5.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     5408 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_amounts.py
--rw-r--r--   0 lash      (1000) lash      (1000)    13691 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)    12440 2023-03-22 10:16:21.000000 erc20-demurrage-token-0.5.2/tests/test_burn.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2041 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_cap.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3190 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_expiry.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1864 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_growth.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2527 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_mint.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9148 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_period.py
--rw-r--r--   0 lash      (1000) lash      (1000)     8189 2023-03-22 08:42:19.000000 erc20-demurrage-token-0.5.2/tests/test_redistribution_single.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7895 2023-03-22 08:43:12.000000 erc20-demurrage-token-0.5.2/tests/test_redistribution_unit.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6518 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_seal.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3644 2023-03-22 08:00:42.000000 erc20-demurrage-token-0.5.2/tests/test_single.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.923105 erc20-demurrage-token-0.5.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      109 2023-05-18 05:43:28.000000 erc20-demurrage-token-0.5.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      754 2023-05-18 05:45:10.923105 erc20-demurrage-token-0.5.3/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token/
+-rw-r--r--   0 lash      (1000) lash      (1000)      198 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/.chainlib
+-rw-r--r--   0 lash      (1000) lash      (1000)    52656 2023-04-03 06:52:15.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/DemurrageTokenSingleNocap.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)    17193 2023-04-03 06:51:46.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/DemurrageTokenSingleNocap.json
+-rw-r--r--   0 lash      (1000) lash      (1000)    18252 2023-04-03 06:52:15.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/DemurrageTokenSingleNocap.metadata.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2023-03-22 09:00:20.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-12-21 10:17:58.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/config/eth.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2021-12-21 10:17:58.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/config/session.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      142 2021-12-21 10:17:58.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/config/token.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)     2738 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/demurrage.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1046 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/expiry.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     6028 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/runnable/publish.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1825 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/seal.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token/sim/
+-rw-r--r--   0 lash      (1000) lash      (1000)       78 2021-06-06 07:35:49.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/sim/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       47 2021-06-06 07:35:49.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/sim/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    11875 2021-10-24 14:29:58.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/sim/sim.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    23772 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/token.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-10 09:14:53.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5227 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4854 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token/unittest/newbase.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      754 2023-05-18 05:45:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1486 2023-05-18 05:45:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-18 05:45:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       94 2023-05-18 05:45:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       85 2023-05-18 05:45:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2023-05-18 05:45:10.000000 erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.919772 erc20-demurrage-token-0.5.3/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     8025 2023-05-18 05:43:28.000000 erc20-demurrage-token-0.5.3/man/build/erc20-demurrage-token-publish.1
+-rw-r--r--   0 lash      (1000) lash      (1000)       85 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1121 2023-05-18 05:45:10.923105 erc20-demurrage-token-0.5.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      792 2023-05-18 05:43:28.000000 erc20-demurrage-token-0.5.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-08-24 19:49:18.000000 erc20-demurrage-token-0.5.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-18 05:45:10.923105 erc20-demurrage-token-0.5.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5408 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_amounts.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    13691 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    12440 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_burn.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2041 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_cap.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3190 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_expiry.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1864 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_growth.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2527 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_mint.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9148 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_period.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     8189 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_redistribution_single.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7895 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_redistribution_unit.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6518 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_seal.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3644 2023-04-03 06:50:10.000000 erc20-demurrage-token-0.5.3/tests/test_single.py
```

### Comparing `erc20-demurrage-token-0.5.2/LICENSE` & `erc20-demurrage-token-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/PKG-INFO` & `erc20-demurrage-token-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-demurrage-token
-Version: 0.5.2
+Version: 0.5.3
 Summary: ERC20 token with redistributed continual demurrage
 Home-page: https://holbrook.no/src/erc20-demurrage-token/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum,blockchain,cryptocurrency,erc20
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/DemurrageTokenSingleNocap.bin` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/DemurrageTokenSingleNocap.bin`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/DemurrageTokenSingleNocap.json` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/DemurrageTokenSingleNocap.json`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/data/DemurrageTokenSingleNocap.metadata.json` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/data/DemurrageTokenSingleNocap.metadata.json`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/demurrage.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/demurrage.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/expiry.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/expiry.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/runnable/publish.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/seal.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/seal.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/sim/sim.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/sim/sim.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/token.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/token.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/unittest/base.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/unittest/base.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token/unittest/newbase.py` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token/unittest/newbase.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/PKG-INFO` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erc20-demurrage-token
-Version: 0.5.2
+Version: 0.5.3
 Summary: ERC20 token with redistributed continual demurrage
 Home-page: https://holbrook.no/src/erc20-demurrage-token/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: ethereum,blockchain,cryptocurrency,erc20
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erc20-demurrage-token-0.5.2/erc20_demurrage_token.egg-info/SOURCES.txt` & `erc20-demurrage-token-0.5.3/erc20_demurrage_token.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 erc20_demurrage_token/runnable/publish.py
 erc20_demurrage_token/sim/__init__.py
 erc20_demurrage_token/sim/error.py
 erc20_demurrage_token/sim/sim.py
 erc20_demurrage_token/unittest/__init__.py
 erc20_demurrage_token/unittest/base.py
 erc20_demurrage_token/unittest/newbase.py
+man/build/erc20-demurrage-token-publish.1
 tests/test_amounts.py
 tests/test_basic.py
 tests/test_burn.py
 tests/test_cap.py
 tests/test_expiry.py
 tests/test_growth.py
 tests/test_mint.py
```

### Comparing `erc20-demurrage-token-0.5.2/setup.cfg` & `erc20-demurrage-token-0.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erc20-demurrage-token
-version = 0.5.2
+version = 0.5.3
 description = ERC20 token with redistributed continual demurrage
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/erc20-demurrage-token/log.html
 keywords = 
 	ethereum
 	blockchain
```

### Comparing `erc20-demurrage-token-0.5.2/tests/test_amounts.py` & `erc20-demurrage-token-0.5.3/tests/test_amounts.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_basic.py` & `erc20-demurrage-token-0.5.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_burn.py` & `erc20-demurrage-token-0.5.3/tests/test_burn.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_cap.py` & `erc20-demurrage-token-0.5.3/tests/test_cap.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_expiry.py` & `erc20-demurrage-token-0.5.3/tests/test_expiry.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_growth.py` & `erc20-demurrage-token-0.5.3/tests/test_growth.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_mint.py` & `erc20-demurrage-token-0.5.3/tests/test_mint.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_period.py` & `erc20-demurrage-token-0.5.3/tests/test_period.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_redistribution_single.py` & `erc20-demurrage-token-0.5.3/tests/test_redistribution_single.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_redistribution_unit.py` & `erc20-demurrage-token-0.5.3/tests/test_redistribution_unit.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_seal.py` & `erc20-demurrage-token-0.5.3/tests/test_seal.py`

 * *Files identical despite different names*

### Comparing `erc20-demurrage-token-0.5.2/tests/test_single.py` & `erc20-demurrage-token-0.5.3/tests/test_single.py`

 * *Files identical despite different names*

