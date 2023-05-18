# Comparing `tmp/sdmaster-1.0.7.tar.gz` & `tmp/sdmaster-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmaster-1.0.7.tar", last modified: Sun Aug 21 02:31:11 2022, max compression
+gzip compressed data, was "sdmaster-1.0.8.tar", last modified: Thu May 18 02:42:44 2023, max compression
```

## Comparing `sdmaster-1.0.7.tar` & `sdmaster-1.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.690118 sdmaster-1.0.7/
--rw-r--r--   0 mikewang   (501) staff       (20)     1070 2022-03-01 03:40:49.000000 sdmaster-1.0.7/LICENSE
--rw-r--r--   0 mikewang   (501) staff       (20)    10022 2022-08-21 02:31:11.689906 sdmaster-1.0.7/PKG-INFO
--rw-r--r--   0 mikewang   (501) staff       (20)     9568 2022-02-28 05:06:12.000000 sdmaster-1.0.7/README.md
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.683467 sdmaster-1.0.7/sdm/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/__init__.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.684312 sdmaster-1.0.7/sdm/api/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/api/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     5077 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/api/api.py
--rw-r--r--   0 mikewang   (501) staff       (20)     5229 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/api/fmp.py
--rw-r--r--   0 mikewang   (501) staff       (20)     7647 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/api/iex_cloud.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.684781 sdmaster-1.0.7/sdm/candlestick/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/candlestick/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     8452 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/candlestick/evaluate.py
--rw-r--r--   0 mikewang   (501) staff       (20)     2832 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/candlestick/parameters.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.685909 sdmaster-1.0.7/sdm/candlestick/pattern/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/candlestick/pattern/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     4334 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/candlestick/pattern/advanced_shapes.py
--rw-r--r--   0 mikewang   (501) staff       (20)     5020 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/candlestick/pattern/basic_shapes.py
--rw-r--r--   0 mikewang   (501) staff       (20)     3186 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/candlestick/pattern/trend.py
--rw-r--r--   0 mikewang   (501) staff       (20)     4498 2022-02-28 04:51:06.000000 sdmaster-1.0.7/sdm/constants.py
--rw-r--r--   0 mikewang   (501) staff       (20)     2982 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/master.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.686156 sdmaster-1.0.7/sdm/operation/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/operation/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     5011 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/operation/validation.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.686852 sdmaster-1.0.7/sdm/persistence/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/persistence/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     5848 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/persistence/csv_operator.py
--rw-r--r--   0 mikewang   (501) staff       (20)      505 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/persistence/file_operator.py
--rw-r--r--   0 mikewang   (501) staff       (20)     6908 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/persistence/sql_operator.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.687870 sdmaster-1.0.7/sdm/simulation/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.7/sdm/simulation/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     5349 2022-08-15 19:26:27.000000 sdmaster-1.0.7/sdm/simulation/market.py
--rw-r--r--   0 mikewang   (501) staff       (20)     7095 2022-08-21 02:29:54.000000 sdmaster-1.0.7/sdm/simulation/performance.py
--rw-r--r--   0 mikewang   (501) staff       (20)    10709 2022-08-15 19:26:19.000000 sdmaster-1.0.7/sdm/simulation/trader.py
--rw-r--r--   0 mikewang   (501) staff       (20)     1752 2022-08-15 19:10:23.000000 sdmaster-1.0.7/sdm/simulation/transaction.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.689104 sdmaster-1.0.7/sdm/util/
--rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/util/__init__.py
--rw-r--r--   0 mikewang   (501) staff       (20)     1028 2022-02-28 04:49:37.000000 sdmaster-1.0.7/sdm/util/date_utils.py
--rw-r--r--   0 mikewang   (501) staff       (20)      961 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/util/io_utils.py
--rw-r--r--   0 mikewang   (501) staff       (20)     3913 2022-07-18 02:16:53.000000 sdmaster-1.0.7/sdm/util/market_utils.py
--rw-r--r--   0 mikewang   (501) staff       (20)     1730 2022-02-21 02:44:55.000000 sdmaster-1.0.7/sdm/util/misc_utils.py
-drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2022-08-21 02:31:11.689705 sdmaster-1.0.7/sdmaster.egg-info/
--rw-r--r--   0 mikewang   (501) staff       (20)    10022 2022-08-21 02:31:11.000000 sdmaster-1.0.7/sdmaster.egg-info/PKG-INFO
--rw-r--r--   0 mikewang   (501) staff       (20)      970 2022-08-21 02:31:11.000000 sdmaster-1.0.7/sdmaster.egg-info/SOURCES.txt
--rw-r--r--   0 mikewang   (501) staff       (20)        1 2022-08-21 02:31:11.000000 sdmaster-1.0.7/sdmaster.egg-info/dependency_links.txt
--rw-r--r--   0 mikewang   (501) staff       (20)       36 2022-08-21 02:31:11.000000 sdmaster-1.0.7/sdmaster.egg-info/requires.txt
--rw-r--r--   0 mikewang   (501) staff       (20)        4 2022-08-21 02:31:11.000000 sdmaster-1.0.7/sdmaster.egg-info/top_level.txt
--rw-r--r--   0 mikewang   (501) staff       (20)       38 2022-08-21 02:31:11.690165 sdmaster-1.0.7/setup.cfg
--rw-r--r--   0 mikewang   (501) staff       (20)      765 2022-08-21 02:30:29.000000 sdmaster-1.0.7/setup.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.016806 sdmaster-1.0.8/
+-rw-r--r--   0 mikewang   (501) staff       (20)     1070 2022-03-01 03:40:49.000000 sdmaster-1.0.8/LICENSE
+-rw-r--r--   0 mikewang   (501) staff       (20)    10022 2023-05-18 02:42:44.016597 sdmaster-1.0.8/PKG-INFO
+-rw-r--r--   0 mikewang   (501) staff       (20)     9568 2022-02-28 05:06:12.000000 sdmaster-1.0.8/README.md
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.009462 sdmaster-1.0.8/sdm/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/__init__.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.010703 sdmaster-1.0.8/sdm/api/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/api/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     5077 2022-11-22 05:31:57.000000 sdmaster-1.0.8/sdm/api/api.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     5279 2022-12-30 22:02:42.000000 sdmaster-1.0.8/sdm/api/fmp.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     7647 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/api/iex_cloud.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.011290 sdmaster-1.0.8/sdm/candlestick/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/candlestick/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     8452 2023-05-18 02:38:13.000000 sdmaster-1.0.8/sdm/candlestick/evaluate.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     2832 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/candlestick/parameters.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.012420 sdmaster-1.0.8/sdm/candlestick/pattern/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/candlestick/pattern/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     4334 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/candlestick/pattern/advanced_shapes.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     5020 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/candlestick/pattern/basic_shapes.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     3186 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/candlestick/pattern/trend.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     4498 2022-02-28 04:51:06.000000 sdmaster-1.0.8/sdm/constants.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     2982 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/master.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.012714 sdmaster-1.0.8/sdm/operation/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/operation/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     5011 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/operation/validation.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.013467 sdmaster-1.0.8/sdm/persistence/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/persistence/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     5848 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/persistence/csv_operator.py
+-rw-r--r--   0 mikewang   (501) staff       (20)      505 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/persistence/file_operator.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     6908 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/persistence/sql_operator.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.014533 sdmaster-1.0.8/sdm/simulation/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-19 03:01:58.000000 sdmaster-1.0.8/sdm/simulation/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     5349 2022-08-15 19:26:27.000000 sdmaster-1.0.8/sdm/simulation/market.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     7095 2022-08-21 02:29:54.000000 sdmaster-1.0.8/sdm/simulation/performance.py
+-rw-r--r--   0 mikewang   (501) staff       (20)    10709 2023-05-09 03:08:15.000000 sdmaster-1.0.8/sdm/simulation/trader.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     1752 2022-08-15 19:10:23.000000 sdmaster-1.0.8/sdm/simulation/transaction.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.015747 sdmaster-1.0.8/sdm/util/
+-rw-r--r--   0 mikewang   (501) staff       (20)        0 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/util/__init__.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     1028 2022-02-28 04:49:37.000000 sdmaster-1.0.8/sdm/util/date_utils.py
+-rw-r--r--   0 mikewang   (501) staff       (20)      961 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/util/io_utils.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     3913 2022-07-18 02:16:53.000000 sdmaster-1.0.8/sdm/util/market_utils.py
+-rw-r--r--   0 mikewang   (501) staff       (20)     1730 2022-02-21 02:44:55.000000 sdmaster-1.0.8/sdm/util/misc_utils.py
+drwxr-xr-x   0 mikewang   (501) staff       (20)        0 2023-05-18 02:42:44.016420 sdmaster-1.0.8/sdmaster.egg-info/
+-rw-r--r--   0 mikewang   (501) staff       (20)    10022 2023-05-18 02:42:43.000000 sdmaster-1.0.8/sdmaster.egg-info/PKG-INFO
+-rw-r--r--   0 mikewang   (501) staff       (20)      970 2023-05-18 02:42:43.000000 sdmaster-1.0.8/sdmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 mikewang   (501) staff       (20)        1 2023-05-18 02:42:43.000000 sdmaster-1.0.8/sdmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 mikewang   (501) staff       (20)       36 2023-05-18 02:42:43.000000 sdmaster-1.0.8/sdmaster.egg-info/requires.txt
+-rw-r--r--   0 mikewang   (501) staff       (20)        4 2023-05-18 02:42:43.000000 sdmaster-1.0.8/sdmaster.egg-info/top_level.txt
+-rw-r--r--   0 mikewang   (501) staff       (20)       38 2023-05-18 02:42:44.016851 sdmaster-1.0.8/setup.cfg
+-rw-r--r--   0 mikewang   (501) staff       (20)      765 2023-05-18 02:42:30.000000 sdmaster-1.0.8/setup.py
```

### Comparing `sdmaster-1.0.7/LICENSE` & `sdmaster-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/PKG-INFO` & `sdmaster-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmaster
-Version: 1.0.7
+Version: 1.0.8
 Summary: Stock Data Master
 Home-page: https://github.com/RedrumSherlock/stockdatamaster
 Author: Mike Wang
 Author-email: wml816@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdmaster-1.0.7/README.md` & `sdmaster-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/api/api.py` & `sdmaster-1.0.8/sdm/api/api.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/api/fmp.py` & `sdmaster-1.0.8/sdm/api/fmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         suffix = "quotes/" + self._market + "?apikey=" + self._token
         raw_response = super()._call_url(suffix)
         logging.info("Successfully loaded all {} realtime quotes for market {}".format(len(raw_response), self._market))
         result = {}
         for quote in raw_response:
             if self._symbol_key in quote:
                 symbol_quote = dict(quote)
-                if self._timestamp_key in symbol_quote:
+                if self._timestamp_key in symbol_quote and symbol_quote[self._timestamp_key] is not None:
                     symbol_quote[c.DATETIME_KEY] = timestamp_to_datetime(symbol_quote[self._timestamp_key])
                     del symbol_quote[self._timestamp_key]
                 del symbol_quote[self._symbol_key]
                 result[quote[self._symbol_key]] = symbol_quote
         return result
 
     def convert_historical_response(self, data, start_date=c.EARLIEST_DATE, end_date=c.LATEST_DATE):
```

### Comparing `sdmaster-1.0.7/sdm/api/iex_cloud.py` & `sdmaster-1.0.8/sdm/api/iex_cloud.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/candlestick/evaluate.py` & `sdmaster-1.0.8/sdm/candlestick/evaluate.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/candlestick/parameters.py` & `sdmaster-1.0.8/sdm/candlestick/parameters.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/candlestick/pattern/advanced_shapes.py` & `sdmaster-1.0.8/sdm/candlestick/pattern/advanced_shapes.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/candlestick/pattern/basic_shapes.py` & `sdmaster-1.0.8/sdm/candlestick/pattern/basic_shapes.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/candlestick/pattern/trend.py` & `sdmaster-1.0.8/sdm/candlestick/pattern/trend.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/constants.py` & `sdmaster-1.0.8/sdm/constants.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/master.py` & `sdmaster-1.0.8/sdm/master.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/operation/validation.py` & `sdmaster-1.0.8/sdm/operation/validation.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/persistence/csv_operator.py` & `sdmaster-1.0.8/sdm/persistence/csv_operator.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/persistence/sql_operator.py` & `sdmaster-1.0.8/sdm/persistence/sql_operator.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/simulation/market.py` & `sdmaster-1.0.8/sdm/simulation/market.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/simulation/performance.py` & `sdmaster-1.0.8/sdm/simulation/performance.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/simulation/trader.py` & `sdmaster-1.0.8/sdm/simulation/trader.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/simulation/transaction.py` & `sdmaster-1.0.8/sdm/simulation/transaction.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/util/date_utils.py` & `sdmaster-1.0.8/sdm/util/date_utils.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/util/io_utils.py` & `sdmaster-1.0.8/sdm/util/io_utils.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/util/market_utils.py` & `sdmaster-1.0.8/sdm/util/market_utils.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdm/util/misc_utils.py` & `sdmaster-1.0.8/sdm/util/misc_utils.py`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/sdmaster.egg-info/PKG-INFO` & `sdmaster-1.0.8/sdmaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmaster
-Version: 1.0.7
+Version: 1.0.8
 Summary: Stock Data Master
 Home-page: https://github.com/RedrumSherlock/stockdatamaster
 Author: Mike Wang
 Author-email: wml816@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdmaster-1.0.7/sdmaster.egg-info/SOURCES.txt` & `sdmaster-1.0.8/sdmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdmaster-1.0.7/setup.py` & `sdmaster-1.0.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='sdmaster',
-    version='1.0.7',
+    version='1.0.8',
     packages=setuptools.find_packages(),
     url='https://github.com/RedrumSherlock/stockdatamaster',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

