# Comparing `tmp/Orange3-Tools-0.0.1.tar.gz` & `tmp/Orange3-Tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Tools-0.0.1.tar", last modified: Sun Apr 16 18:37:46 2023, max compression
+gzip compressed data, was "Orange3-Tools-0.0.2.tar", last modified: Thu May 18 17:02:12 2023, max compression
```

## Comparing `Orange3-Tools-0.0.1.tar` & `Orange3-Tools-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-04-16 18:37:46.614386 Orange3-Tools-0.0.1/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.1/LICENSE
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-04-16 18:37:46.610343 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-04-16 18:37:46.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/PKG-INFO
--rw-r--r--   0 julioj.melero   (501) staff       (20)      920 2023-04-16 18:37:46.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-04-16 18:37:46.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-04-16 18:37:46.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/entry_points.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-04-16 15:00:15.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/not-zip-safe
--rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-04-16 18:37:46.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/requires.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-04-16 18:37:46.000000 Orange3-Tools-0.0.1/Orange3_Tools.egg-info/top_level.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-04-16 18:37:46.614126 Orange3-Tools-0.0.1/PKG-INFO
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.1/README.md
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-04-16 18:37:46.610482 Orange3-Tools-0.0.1/orangecontrib/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.1/orangecontrib/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-04-16 18:37:46.610719 Orange3-Tools-0.0.1/orangecontrib/tools/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.1/orangecontrib/tools/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-04-16 18:37:46.612391 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/
--rw-r--r--   0 julioj.melero   (501) staff       (20)     6970 2023-04-16 09:51:53.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Barplot.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     6982 2023-04-16 09:52:23.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Linesplot.py
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/MySqlOrange.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Pairsplot.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Scatterplot.py
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-04-16 18:37:46.613801 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/
--rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/Barchart.svg
--rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/Pairs.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/category.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/mysql-orange.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/sscater.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.1/orangecontrib/tools/widgets/utils.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-04-16 18:37:46.614429 Orange3-Tools-0.0.1/setup.cfg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-04-16 18:37:45.000000 Orange3-Tools-0.0.1/setup.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.829624 Orange3-Tools-0.0.2/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.2/LICENSE
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.820266 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     1126 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/not-zip-safe
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/requires.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/top_level.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-18 17:02:12.829293 Orange3-Tools-0.0.2/PKG-INFO
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.2/README.md
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.820695 Orange3-Tools-0.0.2/orangecontrib/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.2/orangecontrib/__init__.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.2/orangecontrib/functions.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.821158 Orange3-Tools-0.0.2/orangecontrib/tools/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.2/orangecontrib/tools/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.825831 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     6970 2023-04-16 09:51:53.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Barplot.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     6982 2023-04-16 09:52:23.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Linesplot.py
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/MySqlOrange.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Pairsplot.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Scatterplot.py
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.828957 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/ARIMA.svg
+-rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Barchart.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Correlogram.svg
+-rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Pairs.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/category.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/mysql-orange.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/sscater.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     5175 2023-05-18 08:35:35.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/owcorrelogram.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    30247 2023-05-18 16:46:54.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/owsarima.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/utils.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-18 17:02:12.829673 Orange3-Tools-0.0.2/setup.cfg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-18 08:27:14.000000 Orange3-Tools-0.0.2/setup.py
```

### Comparing `Orange3-Tools-0.0.1/LICENSE` & `Orange3-Tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/Orange3_Tools.egg-info/SOURCES.txt` & `Orange3-Tools-0.0.2/Orange3_Tools.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 Orange3_Tools.egg-info/SOURCES.txt
 Orange3_Tools.egg-info/dependency_links.txt
 Orange3_Tools.egg-info/entry_points.txt
 Orange3_Tools.egg-info/not-zip-safe
 Orange3_Tools.egg-info/requires.txt
 Orange3_Tools.egg-info/top_level.txt
 orangecontrib/__init__.py
+orangecontrib/functions.py
 orangecontrib/tools/__init__.py
 orangecontrib/tools/widgets/Barplot.py
 orangecontrib/tools/widgets/Linesplot.py
 orangecontrib/tools/widgets/MySqlOrange.py
 orangecontrib/tools/widgets/Pairsplot.py
 orangecontrib/tools/widgets/Scatterplot.py
 orangecontrib/tools/widgets/__init__.py
+orangecontrib/tools/widgets/owcorrelogram.py
+orangecontrib/tools/widgets/owsarima.py
 orangecontrib/tools/widgets/utils.py
+orangecontrib/tools/widgets/icons/ARIMA.svg
 orangecontrib/tools/widgets/icons/Barchart.svg
+orangecontrib/tools/widgets/icons/Correlogram.svg
 orangecontrib/tools/widgets/icons/Pairs.svg
 orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
 orangecontrib/tools/widgets/icons/category.svg
 orangecontrib/tools/widgets/icons/mysql-orange.svg
 orangecontrib/tools/widgets/icons/sscater.svg
```

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/__init__.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Barplot.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Barplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Linesplot.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Linesplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/MySqlOrange.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/MySqlOrange.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Pairsplot.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Pairsplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/Scatterplot.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Scatterplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/__init__.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/Barchart.svg` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Barchart.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/Pairs.svg` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Pairs.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/category.svg` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/mysql-orange.svg` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/mysql-orange.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/icons/sscater.svg` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/sscater.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/orangecontrib/tools/widgets/utils.py` & `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.1/setup.py` & `Orange3-Tools-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os import path, walk
 from setuptools import setup, find_packages
 from setuptools.dist import Distribution
 
 NAME = "Orange3-Tools"
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 DESCRIPTION = "Tools para Asignatura Big Data Master EERR"
 LONG_DESCRIPTION = ""
 
 LICENSE = "GPL-3.0"
 
 KEYWORDS = (
```

