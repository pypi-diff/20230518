# Comparing `tmp/hftbacktest-1.5.5.tar.gz` & `tmp/hftbacktest-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.5.5.tar", last modified: Wed May 10 15:04:42 2023, max compression
+gzip compressed data, was "hftbacktest-1.6.0.tar", last modified: Thu May 18 14:43:53 2023, max compression
```

## Comparing `hftbacktest-1.5.5.tar` & `hftbacktest-1.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.5.5/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11501 2023-05-10 14:57:27.000000 hftbacktest-1.5.5/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14547 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.5.5/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.5.5/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.5.5/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.5.5/hftbacktest/data/validation.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/experimental/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14453 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/experimental/live/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/binancefutures.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/custom_strategy.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/ordermanager.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/settings.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6821 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/multiassetinit.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.5.5/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4139 2023-05-10 12:56:12.000000 hftbacktest-1.5.5/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5866 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14794 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    22145 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.5.5/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.5.5/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1252 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.5/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.6.0/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.085622 hftbacktest-1.6.0/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11523 2023-05-18 13:06:32.000000 hftbacktest-1.6.0/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    15671 2023-05-17 15:15:26.000000 hftbacktest-1.6.0/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.085622 hftbacktest-1.6.0/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.6.0/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.6.0/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.6.0/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.6.0/hftbacktest/data/validation.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/experimental/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14543 2023-05-11 12:00:41.000000 hftbacktest-1.6.0/hftbacktest/experimental/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/experimental/live/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/binancefutures.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/custom_strategy.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/ordermanager.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.6.0/hftbacktest/experimental/live/settings.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6817 2023-05-11 11:48:17.000000 hftbacktest-1.6.0/hftbacktest/experimental/multiasset.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.6.0/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4150 2023-05-17 14:22:00.000000 hftbacktest-1.6.0/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6538 2023-05-18 14:26:22.000000 hftbacktest-1.6.0/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.6.0/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    29420 2023-05-18 13:41:42.000000 hftbacktest-1.6.0/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.6.0/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.6.0/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.6.0/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.6.0/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-18 14:43:53.085622 hftbacktest-1.6.0/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1248 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.6.0/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-05-18 14:43:53.000000 hftbacktest-1.6.0/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-05-18 14:43:53.086622 hftbacktest-1.6.0/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.6.0/setup.py
```

### Comparing `hftbacktest-1.5.5/LICENSE` & `hftbacktest-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/PKG-INFO` & `hftbacktest-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.5
+Version: 1.6.0
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.5.5/README.rst` & `hftbacktest-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/__init__.py` & `hftbacktest-1.6.0/hftbacktest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 )
 from .models.queue import (
     RiskAverseQueueModel as RiskAverseQueueModel_,
     LogProbQueueModel as LogProbQueueModel_,
     IdentityProbQueueModel as IdentityProbQueueModel_,
     SquareProbQueueModel as SquareProbQueueModel_
 )
-from .order import BUY, SELL, NONE, NEW, EXPIRED, FILLED, CANCELED, GTC, GTX, Order, OrderBus
+from .order import BUY, SELL, NONE, NEW, EXPIRED, FILLED, CANCELED, MODIFY, GTC, GTX, Order, OrderBus
 from .proc.local import Local
 from .proc.nopartialfillexchange import NoPartialFillExchange
 from .proc.partialfillexchange import PartialFillExchange
 from .reader import (
     COL_EVENT,
     COL_EXCH_TIMESTAMP,
     COL_LOCAL_TIMESTAMP,
@@ -83,14 +83,15 @@
 
     # Order status
     'NONE',
     'NEW',
     'EXPIRED',
     'FILLED',
     'CANCELED',
+    'MODIFY',
 
     # Time-In-Force
     'GTC',
     'GTX',
 
     # Exchange models
     'NoPartialFillExchange',
@@ -123,15 +124,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.5.5'
+__version__ = '1.6.0'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.5.5/hftbacktest/assettype.py` & `hftbacktest-1.6.0/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/backtest.py` & `hftbacktest-1.6.0/hftbacktest/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,39 @@
         """
         self.local.submit_order(order_id, SELL, price, qty, order_type, time_in_force, self.current_timestamp)
 
         if wait:
             return self.goto(UNTIL_END_OF_DATA, wait_order_response=order_id)
         return True
 
+    def modify(self, order_id: int64, price: float64, qty: float64, wait: boolean = False):
+        r"""
+        Modify the specified order.
+
+        - If the adjusted total quantity(leaves_qty + executed_qty) is less than or equal to
+          the quantity already executed, the order will be considered expired. Be aware that this adjustment doesn't
+          affect the remaining quantity in the market, it only changes the total quantity.
+        - Modified orders will be reordered in the match queue.
+
+        Args:
+            order_id: Order ID to modify.
+            price: Order price.
+            qty: Quantity to sell.
+            wait: If ``True``, wait until the order placement response is received.
+
+        Returns:
+            ``True`` if the method reaches the specified timestamp within the data. If the end of the data is reached
+            before the specified timestamp, it returns ``False``.
+        """
+        self.local.modify_order(order_id, price, qty, self.current_timestamp)
+
+        if wait:
+            return self.goto(UNTIL_END_OF_DATA, wait_order_response=order_id)
+        return True
+
     def cancel(self, order_id: int64, wait: boolean = False):
         r"""
         Cancel the specified order.
 
         Args:
             order_id: Order ID to cancel.
             wait: If ``True``, wait until the order placement response is received.
```

### Comparing `hftbacktest-1.5.5/hftbacktest/data/__init__.py` & `hftbacktest-1.6.0/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.6.0/hftbacktest/data/utils/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.6.0/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.6.0/hftbacktest/data/utils/tardis.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/data/validation.py` & `hftbacktest-1.6.0/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/experimental/backtest.py` & `hftbacktest-1.6.0/hftbacktest/experimental/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,17 @@
     def __init__(self, locals, exchs):
         self.locals = locals
         self.exchs = exchs
 
         #: Whether a backtest has finished.
         self.run = True
 
-        timestamp = self.locals[0].next_data[0, COL_LOCAL_TIMESTAMP]
-        if len(self.locals) > 1:
-            for local in self.locals[1:]:
-                timestamp = min(timestamp, local.next_data[0, COL_LOCAL_TIMESTAMP])
+        timestamp = UNTIL_END_OF_DATA
+        for local in self.locals:
+            timestamp = min(timestamp, local.next_data[0, COL_LOCAL_TIMESTAMP])
 
         #: Current timestamp
         self.current_timestamp = timestamp
 
     def position(self, asset: int64):
         """
         Current position.
@@ -342,15 +341,15 @@
             before the specified timestamp, it returns ``False``.
         """
         return self.goto(self.current_timestamp + duration)
 
     def goto(
             self,
             timestamp: float64,
-            asset: Optional[int64] = None,
+            # asset: Optional[int64] = None,
             wait_order_response: int64 = WAIT_ORDER_RESPONSE_NONE
     ):
         r"""
         Goes to a specified timestamp.
 
         This method moves to the specified timestamp, updating the backtesting state to match the corresponding time. If
         ``wait_order_response`` is provided, the method will stop and return when it receives the response for the
@@ -367,49 +366,51 @@
             ``True`` if the method reaches the specified timestamp within the data. If the end of the data is reached
             before the specified timestamp, it returns ``False``.
         """
         found_order_resp_timestamp = False
         while True:
             # Select which side will be processed next.
             next_local_timestamp = -1
-            next_local_proc = None
+            next_local_proc = self.locals[0] # to type assign
             for local in self.locals:
                 timestamp = local.next_timestamp()
                 if timestamp >= 0 or next_local_timestamp == -1:
                     if timestamp < next_local_timestamp:
                         next_local_timestamp = timestamp
                         next_local_proc = local
 
             next_exch_timestamp = -1
-            next_exch_proc = None
-            for exch in self.exchs:
+            next_exch_proc = self.exchs[0] # to type assign
+            next_exch_index = -1
+            for i, exch in enumerate(self.exchs):
                 timestamp = exch.next_timestamp()
                 if timestamp > 0 or next_exch_timestamp == -1:
                     if timestamp < next_exch_timestamp:
                         next_exch_timestamp = timestamp
                         next_exch_proc = exch
+                        next_exch_index = i
 
             # Local will be processed.
             if (0 < next_local_timestamp < next_exch_timestamp) \
                     or (next_local_timestamp > 0 >= next_exch_timestamp):
                 if next_local_timestamp > timestamp:
                     break
                 resp_timestamp = next_local_proc.process(WAIT_ORDER_RESPONSE_NONE)
 
             # Exchange will be processed.
             elif (0 < next_exch_timestamp <= next_local_timestamp) \
                     or (next_exch_timestamp > 0 >= next_local_timestamp):
                 if next_exch_timestamp > timestamp:
                     break
-                if next_exch_proc is asset:  # fixme
-                    resp_timestamp = next_exch_proc(
-                        wait_order_response if not found_order_resp_timestamp else WAIT_ORDER_RESPONSE_NONE
-                    )
-                else:
-                    resp_timestamp = next_exch_proc(WAIT_ORDER_RESPONSE_NONE)
+                # if asset is not None and next_exch_index == asset:
+                #     resp_timestamp = next_exch_proc(
+                #         wait_order_response if not found_order_resp_timestamp else WAIT_ORDER_RESPONSE_NONE
+                #     )
+                # else:
+                resp_timestamp = next_exch_proc(WAIT_ORDER_RESPONSE_NONE)
 
             # No more data or orders to be processed.
             else:
                 self.run = False
                 break
 
             if resp_timestamp > 0:
```

### Comparing `hftbacktest-1.5.5/hftbacktest/experimental/live/binancefutures.py` & `hftbacktest-1.6.0/hftbacktest/experimental/live/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/experimental/live/ordermanager.py` & `hftbacktest-1.6.0/hftbacktest/experimental/live/ordermanager.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/experimental/live/settings.py` & `hftbacktest-1.6.0/hftbacktest/experimental/live/settings.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/experimental/multiassetinit.py` & `hftbacktest-1.6.0/hftbacktest/experimental/multiasset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,35 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Callable
 
 import numpy as np
 import pandas as pd
-from numba import boolean, int64, typeof, ListType
+from numba import boolean, int64, typeof
 from numba.experimental import jitclass
+from numba.typed import List
 
-from .assettype import (
-    LinearAsset as LinearAsset_,
-    InverseAsset as InverseAsset_,
-)
-from .backtest import SingleAssetHftBacktest as SingleAssetHftBacktest_
-from .data import (
-    merge_on_local_timestamp,
-    validate_data,
-    correct_local_timestamp,
-    correct_exch_timestamp,
-    correct_exch_timestamp_adjust,
-    correct,
-)
-from .marketdepth import MarketDepth
-from .models.latencies import (
-    FeedLatency as FeedLatency_,
-    ConstantLatency as ConstantLatency_,
-    ForwardFeedLatency as ForwardFeedLatency_,
-    BackwardFeedLatency as BackwardFeedLatency_,
-    IntpOrderLatency as IntpOrderLatency_
-)
-from .models.queue import (
-    RiskAverseQueueModel as RiskAverseQueueModel_,
-    LogProbQueueModel as LogProbQueueModel_,
-    IdentityProbQueueModel as IdentityProbQueueModel_,
-    SquareProbQueueModel as SquareProbQueueModel_
-)
-from .order import BUY, SELL, NONE, NEW, EXPIRED, FILLED, CANCELED, GTC, GTX, Order, OrderBus
-from .proc.local import Local
-from .proc.nopartialfillexchange import NoPartialFillExchange
-from .proc.partialfillexchange import PartialFillExchange
-from .reader import (
-    COL_EVENT,
-    COL_EXCH_TIMESTAMP,
-    COL_LOCAL_TIMESTAMP,
-    COL_SIDE,
-    COL_PRICE,
-    COL_QTY,
-    DEPTH_EVENT,
-    DEPTH_CLEAR_EVENT,
-    DEPTH_SNAPSHOT_EVENT,
-    TRADE_EVENT,
+from .backtest import MultiAssetHftBacktest as MultiAssetHftBacktest_
+from .. import __load_data, RiskAverseQueueModel
+from ..marketdepth import MarketDepth
+from ..order import OrderBus
+from ..proc.local import LocalInit
+from ..proc.nopartialfillexchange import NoPartialFillExchange, NoPartialFillExchangeInit
+from ..reader import (
     DataReader,
     Cache
 )
-from .stat import Stat
-from .state import State
-from .typing import (
+from ..state import StateInit
+from ..typing import (
     Data,
     ExchangeModelInitiator,
     AssetType,
     OrderLatencyModel,
-    QueueModel,
-    DataCollection,
-    HftBacktestType
+    DataCollection, QueueModel
 )
 
 
-# JIT'ed latency models
-ConstantLatency = jitclass()(ConstantLatency_)
-FeedLatency = jitclass()(FeedLatency_)
-ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
-BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
-IntpOrderLatency = jitclass()(IntpOrderLatency_)
-
-# JIT'ed queue models
-RiskAverseQueueModel = jitclass()(RiskAverseQueueModel_)
-LogProbQueueModel = jitclass()(LogProbQueueModel_)
-IdentityProbQueueModel = jitclass()(IdentityProbQueueModel_)
-SquareProbQueueModel = jitclass()(SquareProbQueueModel_)
-
-# JIT'ed asset types
-LinearAsset = jitclass()(LinearAsset_)
-InverseAsset = jitclass()(InverseAsset_)
-
-Linear = LinearAsset()
-Inverse = InverseAsset()
-
 # JIT'ed HftBacktest
 def MultiAssetHftBacktest(locals, exchs):
     jitted = jitclass(spec=[
         ('run', boolean),
         ('current_timestamp', int64),
         ('locals', typeof(locals)),
         ('exchs', typeof(exchs)),
@@ -96,27 +39,46 @@
 
 class Asset:
     data: DataCollection
     tick_size: float
     lot_size: float
     maker_fee: float
     taker_fee: float
+    snapshot: Optional[Data]
+    start_position: float
+    start_balance: float
+    start_fee: float
+
+    def __init__(
+            self,
+            data: DataCollection,
+            tick_size: float,
+            lot_size: float,
+            maker_fee: float,
+            taker_fee: float,
+            snapshot: Optional[Data]
+    ):
+        self.data = data
+        self.tick_size = tick_size
+        self.lot_size = lot_size
+        self.maker_fee = maker_fee
+        self.taker_fee = taker_fee
+        self.snapshot = snapshot
+        self.start_position = 0
+        self.start_balance = 0
+        self.start_fee = 0
 
 
 def HftBacktest(
-        asset: List[Asset],
-        order_latency: OrderLatencyModel,
-        asset_type: AssetType,
-        queue_model: Optional[QueueModel] = None,
-        snapshot: Optional[Data] = None,
-        start_position: float = 0,
-        start_balance: float = 0,
-        start_fee: float = 0,
+        assets: List[Asset],
+        order_latency: Callable[[], OrderLatencyModel],
+        asset_type: Callable[[], AssetType],
+        queue_model: Optional[Callable[[], QueueModel]] = None,
         trade_list_size: int = 0,
-        exchange_model: ExchangeModelInitiator = None
+        exchange_model: Optional[ExchangeModelInitiator] = None
 ):
     r"""
     Create a HftBacktest instance.
 
     Args:
         data: Data to be fed.
         tick_size: Minimum price increment for the given asset.
@@ -133,91 +95,118 @@
         trade_list_size: Buffer size for storing market trades; the default value of ``0`` indicates that market trades
                          will not be stored in the buffer.
         exchange_model: Exchange model with default set as ``NoPartialFillExchange``.
 
     Returns:
          JIT'ed :class:`.SingleAssetHftBacktest`
     """
-
-    cache = Cache()
-
-    if isinstance(data, list):
-        local_reader = DataReader(cache)
-        exch_reader = DataReader(cache)
-        for item in data:
-            if isinstance(item, str):
-                local_reader.add_file(item)
-                exch_reader.add_file(item)
-            elif isinstance(item, pd.DataFrame) or isinstance(item, np.ndarray):
-                local_reader.add_data(item)
-                exch_reader.add_data(item)
-            else:
-                raise ValueError('Unsupported data type')
-    elif isinstance(data, str):
-        local_reader = DataReader(cache)
-        local_reader.add_file(data)
-
-        exch_reader = DataReader(cache)
-        exch_reader.add_file(data)
-    else:
-        data = __load_data(data)
-        local_reader = DataReader(cache)
-        local_reader.add_data(data)
-
-        exch_reader = DataReader(cache)
-        exch_reader.add_data(data)
-
     if queue_model is None:
-        queue_model = RiskAverseQueueModel()
-
-    local_market_depth = MarketDepth(tick_size, lot_size)
-    exch_market_depth = MarketDepth(tick_size, lot_size)
-
-    if snapshot is not None:
-        snapshot = __load_data(snapshot)
-        local_market_depth.apply_snapshot(snapshot)
-        exch_market_depth.apply_snapshot(snapshot)
-
-    local_state = State(
-        start_position,
-        start_balance,
-        start_fee,
-        maker_fee,
-        taker_fee,
-        asset_type
-    )
-    exch_state = State(
-        start_position,
-        start_balance,
-        start_fee,
-        maker_fee,
-        taker_fee,
-        asset_type
-    )
-
-    exch_to_local_orders = OrderBus()
-    local_to_exch_orders = OrderBus()
-
-    local = Local(
-        local_reader,
-        local_to_exch_orders,
-        exch_to_local_orders,
-        local_market_depth,
-        local_state,
-        order_latency,
-        trade_list_size
-    )
+        queue_model = RiskAverseQueueModel
 
     if exchange_model is None:
         exchange_model = NoPartialFillExchange
 
-    exch = exchange_model(
-        exch_reader,
-        exch_to_local_orders,
-        local_to_exch_orders,
-        exch_market_depth,
-        exch_state,
-        order_latency,
-        queue_model
-    )
+    locals = None
+    exchs = None
+
+    local_reader = DataReader(Cache())
+    state_init = StateInit(asset_type())
+    sample_state = state_init(
+            0,
+            0,
+            0,
+            0,
+            0,
+            asset_type()
+        )
+    local_init = LocalInit(local_reader, sample_state, order_latency())
+    exch_init = NoPartialFillExchangeInit(
+            local_reader,
+            sample_state,
+            order_latency(),
+            queue_model()
+        )
+
+    for asset in assets:
+        cache = Cache()
+
+        if isinstance(asset.data, list):
+            local_reader = DataReader(cache)
+            exch_reader = DataReader(cache)
+            for item in asset.data:
+                if isinstance(item, str):
+                    local_reader.add_file(item)
+                    exch_reader.add_file(item)
+                elif isinstance(item, pd.DataFrame) or isinstance(item, np.ndarray):
+                    local_reader.add_data(item)
+                    exch_reader.add_data(item)
+                else:
+                    raise ValueError('Unsupported data type')
+        elif isinstance(asset.data, str):
+            local_reader = DataReader(cache)
+            local_reader.add_file(asset.data)
+
+            exch_reader = DataReader(cache)
+            exch_reader.add_file(asset.data)
+        else:
+            data = __load_data(asset.data)
+            local_reader = DataReader(cache)
+            local_reader.add_data(data)
+
+            exch_reader = DataReader(cache)
+            exch_reader.add_data(data)
+
+        local_market_depth = MarketDepth(asset.tick_size, asset.lot_size)
+        exch_market_depth = MarketDepth(asset.tick_size, asset.lot_size)
+
+        if asset.snapshot is not None:
+            snapshot = __load_data(asset.snapshot)
+            local_market_depth.apply_snapshot(snapshot)
+            exch_market_depth.apply_snapshot(snapshot)
+
+        local_state = state_init(
+            asset.start_position,
+            asset.start_balance,
+            asset.start_fee,
+            asset.maker_fee,
+            asset.taker_fee,
+            asset_type()
+        )
+        exch_state = state_init(
+            asset.start_position,
+            asset.start_balance,
+            asset.start_fee,
+            asset.maker_fee,
+            asset.taker_fee,
+            asset_type()
+        )
+
+        exch_to_local_orders = OrderBus()
+        local_to_exch_orders = OrderBus()
+
+        local = local_init(
+            local_reader,
+            local_to_exch_orders,
+            exch_to_local_orders,
+            local_market_depth,
+            local_state,
+            order_latency(),
+            trade_list_size
+        )
+        if locals is None:
+            locals = List.empty_list(typeof(local))
+        locals.append(local)
+
+        exch = exch_init(
+            exch_reader,
+            exch_to_local_orders,
+            local_to_exch_orders,
+            exch_market_depth,
+            exch_state,
+            order_latency(),
+            queue_model()
+        )
+        if exchs is None:
+            exchs = List.empty_list(typeof(exch))
+        exchs.append(exch)
 
     return MultiAssetHftBacktest(locals, exchs)
```

### Comparing `hftbacktest-1.5.5/hftbacktest/marketdepth.py` & `hftbacktest-1.6.0/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/models/latencies.py` & `hftbacktest-1.6.0/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/models/queue.py` & `hftbacktest-1.6.0/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/order.py` & `hftbacktest-1.6.0/hftbacktest/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 NONE = 0
 NEW = 1
 EXPIRED = 2
 FILLED = 3
 CANCELED = 4
 PARTIALLY_FILLED = 5
+MODIFY = 6
 
 GTC = 0  # Good 'till cancel
 GTX = 1  # Post only
 FOK = 2  # Fill or kill
 IOC = 3  # Immediate or cancel
 
 LIMIT = 0
```

### Comparing `hftbacktest-1.5.5/hftbacktest/proc/local.py` & `hftbacktest-1.6.0/hftbacktest/proc/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from numba import int64, float64
 from numba.experimental import jitclass
 
 from .proc import Proc, proc_spec
-from ..order import BUY, NEW, CANCELED, FILLED, EXPIRED, NONE, Order
+from ..order import BUY, NEW, CANCELED, FILLED, EXPIRED, NONE, MODIFY, Order
 from ..reader import (
     COL_EVENT,
     COL_LOCAL_TIMESTAMP,
     COL_SIDE,
     COL_PRICE,
     COL_QTY,
     DEPTH_CLEAR_EVENT,
@@ -125,21 +125,38 @@
         order = Order(order_id, price_tick, self.depth.tick_size, qty, side, time_in_force, order_type)
         order.req = NEW
         exch_recv_timestamp = current_timestamp + self.order_latency.entry(current_timestamp, order, self)
 
         self.orders[order.order_id] = order
         self.orders_to.append(order.copy(), exch_recv_timestamp)
 
+    def modify_order(self, order_id, price, qty, current_timestamp):
+        order = self.orders.get(order_id)
+
+        if order is None:
+            raise KeyError('the given order_id does not exist.')
+        if order.req != NONE:
+            raise ValueError('the given order cannot be modified because there is a ongoing request.')
+
+        order.req = MODIFY
+
+        order = order.copy()
+        order.price_tick = round(price / self.depth.tick_size)
+        order.qty = qty
+        exch_recv_timestamp = current_timestamp + self.order_latency.entry(current_timestamp, order, self)
+
+        self.orders_to.append(order, exch_recv_timestamp)
+
     def cancel(self, order_id, current_timestamp):
         order = self.orders.get(order_id)
 
         if order is None:
             raise KeyError('the given order_id does not exist.')
         if order.req != NONE:
-            raise ValueError('the given order cannot be cancelled because there is a ongoing request.')
+            raise ValueError('the given order cannot be canceled because there is a ongoing request.')
 
         order.req = CANCELED
         exch_recv_timestamp = current_timestamp + self.order_latency.entry(current_timestamp, order, self)
 
         self.orders_to.append(order.copy(), exch_recv_timestamp)
 
     def clear_inactive_orders(self):
```

### Comparing `hftbacktest-1.5.5/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.6.0/hftbacktest/proc/nopartialfillexchange.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from numba import typeof, int64
 from numba.experimental import jitclass
 from numba.typed.typeddict import Dict
 from numba.types import DictType
 
 from .proc import Proc, proc_spec
 from ..marketdepth import INVALID_MAX, INVALID_MIN
-from ..order import BUY, SELL, NEW, CANCELED, FILLED, EXPIRED, GTX, NONE, order_ladder_ty
+from ..order import BUY, SELL, NEW, CANCELED, FILLED, EXPIRED, GTX, NONE, MODIFY, order_ladder_ty
 from ..reader import (
     COL_EVENT,
     COL_EXCH_TIMESTAMP,
     COL_SIDE,
     COL_PRICE,
     COL_QTY,
     DEPTH_CLEAR_EVENT,
@@ -72,14 +72,19 @@
 
     def _process_recv_order(self, order, recv_timestamp, wait_resp, next_timestamp):
         # Process a new order.
         if order.req == NEW:
             order.req = NONE
             resp_timestamp = self.__ack_new(order, recv_timestamp)
 
+        # Process a modify order.
+        elif order.req == MODIFY:
+            order.req = NONE
+            resp_timestamp = self.__ack_modify(order, recv_timestamp)
+
         # Process a cancel order.
         elif order.req == CANCELED:
             order.req = NONE
             resp_timestamp = self.__ack_cancel(order, recv_timestamp)
 
         else:
             raise ValueError('req')
@@ -293,14 +298,100 @@
                 self.queue_model.new(order, self)
                 order.status = NEW
         order.exch_timestamp = timestamp
         local_recv_timestamp = timestamp + self.order_latency.response(timestamp, order, self)
         self.orders_to.append(order.copy(), local_recv_timestamp)
         return local_recv_timestamp
 
+    def __ack_modify(self, order, timestamp):
+        exch_order = self.orders.get(order.order_id)
+
+        # The order can be already deleted due to fill or expiration.
+        if exch_order is None:
+            order.status = EXPIRED
+            order.exch_timestamp = timestamp
+            local_recv_timestamp = timestamp + self.order_latency.response(timestamp, order, self)
+            # It can overwrite another existing order on the local side if order_id is the same. So, commented out.
+            # self.orders_to.append(order.copy(), local_recv_timestamp)
+            return local_recv_timestamp
+
+        prev_price_tick = exch_order.price_tick
+        exch_order.price_tick = order.price_tick
+        # No partial fill occurs.
+        exch_order.qty = order.qty
+        # The initialization of the order queue position may not occur when the modified quantity is smaller than
+        # the previous quantity, depending on the exchanges. It may need to implement exchange-specific
+        # specialization.
+        init_q_pos = True
+
+        if exch_order.side == BUY:
+            # Check if the buy order price is greater than or equal to the current best ask.
+            if exch_order.price_tick >= self.depth.best_ask_tick:
+                del self.buy_orders[prev_price_tick][exch_order.order_id]
+                del self.orders[exch_order.order_id]
+
+                if exch_order.time_in_force == GTX:
+                    exch_order.status = EXPIRED
+                else:
+                    # Take the market.
+                    return self.__fill(
+                        exch_order,
+                        timestamp,
+                        False,
+                        exec_price_tick=self.depth.best_ask_tick,
+                        delete_order=False
+                    )
+            else:
+                # The exchange accepts this order.
+                if prev_price_tick != exch_order.price_tick:
+                    del self.buy_orders[prev_price_tick][exch_order.order_id]
+                    o = self.buy_orders.setdefault(
+                        exch_order.price_tick,
+                        Dict.empty(int64, order_ladder_ty)
+                    )
+                    o[exch_order.order_id] = exch_order
+                if init_q_pos or prev_price_tick != exch_order.price_tick:
+                    # Initialize the order's queue position.
+                    self.queue_model.new(exch_order, self)
+                exch_order.status = NEW
+        else:
+            # Check if the sell order price is less than or equal to the current best bid.
+            if exch_order.price_tick <= self.depth.best_bid_tick:
+                del self.sell_orders[prev_price_tick][exch_order.order_id]
+                del self.orders[exch_order.order_id]
+
+                if exch_order.time_in_force == GTX:
+                    exch_order.status = EXPIRED
+                else:
+                    # Take the market.
+                    return self.__fill(
+                        exch_order,
+                        timestamp,
+                        False,
+                        exec_price_tick=self.depth.best_bid_tick,
+                        delete_order=False
+                    )
+            else:
+                # The exchange accepts this order.
+                if prev_price_tick != exch_order.price_tick:
+                    del self.sell_orders[prev_price_tick][exch_order.order_id]
+                    o = self.sell_orders.setdefault(
+                        exch_order.price_tick,
+                        Dict.empty(int64, order_ladder_ty)
+                    )
+                    o[exch_order.order_id] = exch_order
+                if init_q_pos or prev_price_tick != exch_order.price_tick:
+                    # Initialize the order's queue position.
+                    self.queue_model.new(exch_order, self)
+                exch_order.status = NEW
+        exch_order.exch_timestamp = timestamp
+        local_recv_timestamp = timestamp + self.order_latency.response(timestamp, exch_order, self)
+        self.orders_to.append(exch_order.copy(), local_recv_timestamp)
+        return local_recv_timestamp
+
     def __ack_cancel(self, order, timestamp):
         exch_order = self.orders.get(order.order_id)
 
         # The order can be already deleted due to fill or expiration.
         if exch_order is None:
             order.status = EXPIRED
             order.exch_timestamp = timestamp
```

### Comparing `hftbacktest-1.5.5/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.6.0/hftbacktest/proc/partialfillexchange.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     BUY,
     SELL,
     NEW,
     CANCELED,
     FILLED,
     EXPIRED,
     PARTIALLY_FILLED,
+    MODIFY,
     GTX,
+    GTC,
     FOK,
     IOC,
     NONE,
     order_ladder_ty
 )
 from ..reader import (
     COL_EVENT,
@@ -87,14 +89,19 @@
 
     def _process_recv_order(self, order, recv_timestamp, wait_resp, next_timestamp):
         # Process a new order.
         if order.req == NEW:
             order.req = NONE
             resp_timestamp = self.__ack_new(order, recv_timestamp)
 
+        # Process a modify order.
+        elif order.req == MODIFY:
+            order.req = NONE
+            resp_timestamp = self.__ack_modify(order, recv_timestamp)
+
         # Process a cancel order.
         elif order.req == CANCELED:
             order.req = NONE
             resp_timestamp = self.__ack_cancel(order, recv_timestamp)
 
         else:
             raise ValueError('req')
@@ -468,14 +475,144 @@
                 self.queue_model.new(order, self)
                 order.status = NEW
         order.exch_timestamp = timestamp
         local_recv_timestamp = timestamp + self.order_latency.response(timestamp, order, self)
         self.orders_to.append(order.copy(), local_recv_timestamp)
         return local_recv_timestamp
 
+    def __ack_modify(self, order, timestamp):
+        exch_order = self.orders.get(order.order_id)
+
+        # The order can be already deleted due to fill or expiration.
+        if exch_order is None:
+            order.status = EXPIRED
+            order.exch_timestamp = timestamp
+            local_recv_timestamp = timestamp + self.order_latency.response(timestamp, order, self)
+            # It can overwrite another existing order on the local side if order_id is the same. So, commented out.
+            # self.orders_to.append(order.copy(), local_recv_timestamp)
+            return local_recv_timestamp
+
+        prev_price_tick = exch_order.price_tick
+        exch_order.price_tick = order.price_tick
+
+        # See https://binance-docs.github.io/apidocs/futures/en/#modify-order-trade
+        # It's not sure if this is a general behavior across exchanges.
+        executed_qty = exch_order.qty - exch_order.leaves_qty
+        if exch_order.status == PARTIALLY_FILLED and order.qty <= executed_qty:
+            exch_order.status = EXPIRED
+
+            if exch_order.side == BUY:
+                del self.buy_orders[prev_price_tick][exch_order.order_id]
+            else:
+                del self.sell_orders[prev_price_tick][exch_order.order_id]
+            del self.orders[exch_order.order_id]
+        else:
+            # The initialization of the order queue position may not occur when the modified quantity is smaller than
+            # the previous quantity, depending on the exchanges. It may need to implement exchange-specific
+            # specialization.
+            init_q_pos = True
+            exch_order.qty = order.qty
+
+            if exch_order.side == BUY:
+                # Check if the buy order price is greater than or equal to the current best ask.
+                if exch_order.price_tick >= self.depth.best_ask_tick:
+                    del self.buy_orders[prev_price_tick][exch_order.order_id]
+                    del self.orders[exch_order.order_id]
+
+                    if exch_order.time_in_force == GTX:
+                        exch_order.status = EXPIRED
+                    elif exch_order.time_in_force == GTC:
+                        # Take the market.
+                        for t in range(self.depth.best_ask_tick, exch_order.price_tick):
+                            exec_qty = min(self.depth.ask_depth[t], exch_order.qty)
+                            local_recv_timestamp = self.__fill(
+                                exch_order,
+                                exec_qty,
+                                timestamp,
+                                False,
+                                exec_price_tick=t,
+                                delete_order=False
+                            )
+                            if exch_order.status == FILLED:
+                                return local_recv_timestamp
+                        # The buy order cannot remain in the ask book, as it cannot affect the market depth during
+                        # backtesting based on market-data replay. So, even though it simulates partial fill, if the order
+                        # size is not small enough, it introduces unreality.
+                        return self.__fill(
+                            exch_order,
+                            exch_order.leaves_qty,
+                            timestamp,
+                            False,
+                            exec_price_tick=exch_order.price_tick,
+                            delete_order=False
+                        )
+                else:
+                    # The exchange accepts this order.
+                    if prev_price_tick != exch_order.price_tick:
+                        del self.buy_orders[prev_price_tick][exch_order.order_id]
+                        o = self.buy_orders.setdefault(
+                            exch_order.price_tick,
+                            Dict.empty(int64, order_ladder_ty)
+                        )
+                        o[exch_order.order_id] = exch_order
+                    if init_q_pos or prev_price_tick != exch_order.price_tick:
+                        # Initialize the order's queue position.
+                        self.queue_model.new(exch_order, self)
+                    exch_order.status = NEW
+            else:
+                # Check if the sell order price is less than or equal to the current best bid.
+                if exch_order.price_tick <= self.depth.best_bid_tick:
+                    del self.sell_orders[prev_price_tick][exch_order.order_id]
+                    del self.orders[exch_order.order_id]
+
+                    if exch_order.time_in_force == GTX:
+                        exch_order.status = EXPIRED
+                    elif exch_order.time_in_force == GTC:
+                        # Take the market.
+                        for t in range(self.depth.best_bid_tick, exch_order.price_tick, -1):
+                            exec_qty = min(self.depth.bid_depth[t], exch_order.qty)
+                            local_recv_timestamp = self.__fill(
+                                exch_order,
+                                exec_qty,
+                                timestamp,
+                                False,
+                                exec_price_tick=t,
+                                delete_order=False
+                            )
+                            if exch_order.status == FILLED:
+                                return local_recv_timestamp
+                        # The sell order cannot remain in the bid book, as it cannot affect the market depth during
+                        # backtesting based on market-data replay. So, even though it simulates partial fill, if the order
+                        # size is not small enough, it introduces unreality.
+                        return self.__fill(
+                            exch_order,
+                            exch_order.leaves_qty,
+                            timestamp,
+                            False,
+                            exec_price_tick=exch_order.price_tick,
+                            delete_order=False
+                        )
+                else:
+                    # The exchange accepts this order.
+                    if prev_price_tick != exch_order.price_tick:
+                        del self.sell_orders[prev_price_tick][exch_order.order_id]
+                        o = self.sell_orders.setdefault(
+                            exch_order.price_tick,
+                            Dict.empty(int64, order_ladder_ty)
+                        )
+                        o[exch_order.order_id] = exch_order
+                    if init_q_pos or prev_price_tick != exch_order.price_tick:
+                        # Initialize the order's queue position.
+                        self.queue_model.new(exch_order, self)
+                    exch_order.status = NEW
+        exch_order.exch_timestamp = timestamp
+        local_recv_timestamp = timestamp + self.order_latency.response(timestamp, exch_order, self)
+        self.orders_to.append(exch_order.copy(), local_recv_timestamp)
+        return local_recv_timestamp
+
     def __ack_cancel(self, order, timestamp):
         exch_order = self.orders.get(order.order_id)
 
         # The order can be already deleted due to fill or expiration.
         if exch_order is None:
             order.status = EXPIRED
             order.exch_timestamp = timestamp
```

### Comparing `hftbacktest-1.5.5/hftbacktest/proc/proc.py` & `hftbacktest-1.6.0/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/reader.py` & `hftbacktest-1.6.0/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/stat.py` & `hftbacktest-1.6.0/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/state.py` & `hftbacktest-1.6.0/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest/typing.py` & `hftbacktest-1.6.0/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.5/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.6.0/hftbacktest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.5
+Version: 1.6.0
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.5.5/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.6.0/hftbacktest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 hftbacktest/data/validation.py
 hftbacktest/data/utils/__init__.py
 hftbacktest/data/utils/binancefutures.py
 hftbacktest/data/utils/snapshot.py
 hftbacktest/data/utils/tardis.py
 hftbacktest/experimental/__init__.py
 hftbacktest/experimental/backtest.py
-hftbacktest/experimental/multiassetinit.py
+hftbacktest/experimental/multiasset.py
 hftbacktest/experimental/live/__init__.py
 hftbacktest/experimental/live/binancefutures.py
 hftbacktest/experimental/live/custom_strategy.py
 hftbacktest/experimental/live/ordermanager.py
 hftbacktest/experimental/live/settings.py
 hftbacktest/models/__init__.py
 hftbacktest/models/latencies.py
```

### Comparing `hftbacktest-1.5.5/setup.cfg` & `hftbacktest-1.6.0/setup.cfg`

 * *Files identical despite different names*

