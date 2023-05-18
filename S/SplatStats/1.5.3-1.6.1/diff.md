# Comparing `tmp/SplatStats-1.5.3.tar.gz` & `tmp/SplatStats-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-1.5.3.tar", last modified: Tue May  9 17:06:45 2023, max compression
+gzip compressed data, was "SplatStats-1.6.1.tar", last modified: Thu May 18 17:58:01 2023, max compression
```

## Comparing `SplatStats-1.5.3.tar` & `SplatStats-1.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-09 17:06:45.269565 SplatStats-1.5.3/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-09-17 20:12:28.000000 SplatStats-1.5.3/LICENSE
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-09 17:06:45.265565 SplatStats-1.5.3/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6368 2023-01-25 04:16:56.000000 SplatStats-1.5.3/README.md
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-09 17:06:45.265565 SplatStats-1.5.3/SplatStats/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10828 2023-03-14 03:30:29.000000 SplatStats-1.5.3/SplatStats/Battle.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10398 2023-05-09 04:00:59.000000 SplatStats-1.5.3/SplatStats/Player.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     3058 2023-05-08 04:02:05.000000 SplatStats-1.5.3/SplatStats/StatInk.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     2477 2022-11-01 00:29:50.000000 SplatStats-1.5.3/SplatStats/Team.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      896 2023-03-19 21:08:44.000000 SplatStats-1.5.3/SplatStats/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       21 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6148 2022-12-04 18:34:39.000000 SplatStats-1.5.3/SplatStats/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13947 2023-05-08 00:35:21.000000 SplatStats-1.5.3/SplatStats/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     5393 2023-05-09 16:49:18.000000 SplatStats-1.5.3/SplatStats/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4137 2023-03-14 03:19:39.000000 SplatStats-1.5.3/SplatStats/files.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8663 2023-02-17 22:36:56.000000 SplatStats-1.5.3/SplatStats/parsers.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    56269 2023-05-09 05:39:51.000000 SplatStats-1.5.3/SplatStats/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1428 2022-09-29 02:14:29.000000 SplatStats-1.5.3/SplatStats/plotsAux.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1709 2022-11-14 00:32:41.000000 SplatStats-1.5.3/SplatStats/plotsTeam.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10176 2023-04-06 04:24:33.000000 SplatStats-1.5.3/SplatStats/statInkConstants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    10543 2023-04-28 00:57:38.000000 SplatStats-1.5.3/SplatStats/statInkPlots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     8511 2023-04-06 03:09:35.000000 SplatStats-1.5.3/SplatStats/statInkStats.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    13991 2023-05-09 04:12:42.000000 SplatStats-1.5.3/SplatStats/stats.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-05-09 17:06:45.265565 SplatStats-1.5.3/SplatStats.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6748 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      607 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      159 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       11 2023-05-09 17:06:45.000000 SplatStats-1.5.3/SplatStats.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-05-09 17:06:45.269565 SplatStats-1.5.3/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1251 2023-02-19 19:16:43.000000 SplatStats-1.5.3/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 17:58:01.681049 SplatStats-1.6.1/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-1.6.1/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-18 17:58:01.680919 SplatStats-1.6.1/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6368 2023-05-11 17:29:12.000000 SplatStats-1.6.1/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 17:58:01.680097 SplatStats-1.6.1/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13947 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-1.6.1/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10543 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13991 2023-05-11 17:29:12.000000 SplatStats-1.6.1/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-05-18 17:58:01.680734 SplatStats-1.6.1/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6748 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-05-18 17:58:01.000000 SplatStats-1.6.1/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-05-18 17:58:01.681095 SplatStats-1.6.1/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-1.6.1/setup.py
```

### Comparing `SplatStats-1.5.3/LICENSE` & `SplatStats-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/PKG-INFO` & `SplatStats-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.5.3
+Version: 1.6.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.5.3/README.md` & `SplatStats-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/Battle.py` & `SplatStats-1.6.1/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/Player.py` & `SplatStats-1.6.1/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/StatInk.py` & `SplatStats-1.6.1/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/Team.py` & `SplatStats-1.6.1/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/__init__.py` & `SplatStats-1.6.1/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/auxiliary.py` & `SplatStats-1.6.1/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/colors.py` & `SplatStats-1.6.1/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/constants.py` & `SplatStats-1.6.1/SplatStats/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,19 +70,21 @@
     False: ','
 }
 CLR_FEST = {
     True: clr.PINK_V_GREEN_S1 [0],
     False: clr.LMODEL_V_PMODEL_S2[-1]
 }
 CLR_STAGE = {
+    'Barnacle & Dime': clr.GHERKOUT_V_GHERKIN_S2[1],
     'Brinewater Springs': clr.GRAPE_V_TURQUOISE_S2[0], 
     'Eeltail Alley': clr.PINK_V_ORANGE_S1[1],
     'Flounder Heights': clr.SWEATER_V_SOCKS_S2[0],
     'Hagglefish Market': clr.LPINK_V_BLUE_S2[1],
     'Hammerhead Bridge': clr.MAYO_V_KETCHUP_S2[1],
+    'Humpback Pump Track': clr.CALLIE_V_MARIE_S1[1],
     'Inkblot Art Academy': clr.LPINK_V_BLUE_S2[0],
     'Mahi-Mahi Resort': clr.CHAOS_V_ORDER_S2[1],
     'MakoMart': clr.PINK_V_GREEN_S1[2],
     'Mincemeat Metalworks': clr.TSUBUAN_V_KOSHIAN_S2[1],
     "Museum d'Alfonsino": clr.SALTY_V_SWEET_S2[0],
     'Scorch Gorge': clr.UNICORN_V_NARWHAL_S2[0],
     'Sturgeon Shipyard': clr.VAMPIRE_V_WEREWOLF_S2[2],
```

### Comparing `SplatStats-1.5.3/SplatStats/files.py` & `SplatStats-1.6.1/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/parsers.py` & `SplatStats-1.6.1/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/plots.py` & `SplatStats-1.6.1/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/plotsAux.py` & `SplatStats-1.6.1/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/plotsTeam.py` & `SplatStats-1.6.1/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/statInkConstants.py` & `SplatStats-1.6.1/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/statInkPlots.py` & `SplatStats-1.6.1/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/statInkStats.py` & `SplatStats-1.6.1/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats/stats.py` & `SplatStats-1.6.1/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/SplatStats.egg-info/PKG-INFO` & `SplatStats-1.6.1/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 1.5.3
+Version: 1.6.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-1.5.3/SplatStats.egg-info/SOURCES.txt` & `SplatStats-1.6.1/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-1.5.3/setup.py` & `SplatStats-1.6.1/setup.py`

 * *Files identical despite different names*

