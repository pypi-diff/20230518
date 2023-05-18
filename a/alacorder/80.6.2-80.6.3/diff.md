# Comparing `tmp/alacorder-80.6.2.tar.gz` & `tmp/alacorder-80.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.2.tar", max compression
+gzip compressed data, was "alacorder-80.6.3.tar", max compression
```

## Comparing `alacorder-80.6.2.tar` & `alacorder-80.6.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.2/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.2/README.md
--rw-r--r--   0        0        0      746 2023-05-18 16:26:19.428735 alacorder-80.6.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-18 16:26:13.972097 alacorder-80.6.2/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234128 2023-05-18 16:25:56.123146 alacorder-80.6.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234128 2023-05-18 16:25:50.985997 alacorder-80.6.2/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.3/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.3/README.md
+-rw-r--r--   0        0        0      746 2023-05-18 16:59:39.102314 alacorder-80.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-18 16:59:38.772596 alacorder-80.6.3/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234215 2023-05-18 16:59:13.235012 alacorder-80.6.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234215 2023-05-18 16:59:09.146003 alacorder-80.6.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.3/PKG-INFO
```

### Comparing `alacorder-80.6.2/LICENSE` & `alacorder-80.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.2/README.md` & `alacorder-80.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.2/pyproject.toml` & `alacorder-80.6.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.2"
+version = "80.6.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.2/src/alacorder/.DS_Store` & `alacorder-80.6.3/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.2/src/alacorder/__main__.py` & `alacorder-80.6.3/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.2"
+version = "80.6.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2588,18 +2588,18 @@
         ]
     )
     images = images.select(
         [
             pl.col("CaseNumber"),
             pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
             pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).str.to_time('%-H %M %S %p', strict=False).alias("Time"),
-            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').alias("Doc#"),
+            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').cast(pl.Int64, strict=False).alias("Doc#"),
             pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
             pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
-            pl.col("Images").str.extract(r'^(\d)\s').alias("Pages")
+            pl.col("Images").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("Pages")
         ])
     images = images.fill_null('')
     return images
 
 
 def _explode_case_action_summary(df, debug=False):
     cas = df.select(
@@ -2736,15 +2736,15 @@
             .alias("Settings"),
         ]
     )
     settings = settings.drop_nulls()
     settings = settings.select(
         [
             pl.col("CaseNumber"),
-            pl.col("Settings").str.extract(r'^(\d)\s').alias("#"),
+            pl.col("Settings").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("#"),
             pl.col("Settings").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
             pl.col("Settings").str.extract(r'\s(\d\d\d)\s').alias("Que"),
             pl.col("Settings").str.extract(r'(\d\d \d\d [A|P]M)').str.to_time(r'%H %M %p', strict=False).alias("Time"),
             pl.col("Settings").str.extract(r'[A|P]M (.+)').str.strip().alias("Description")
         ])
     return settings
```

### Comparing `alacorder-80.6.2/src/alacorder/alac.py` & `alacorder-80.6.3/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.2"
+version = "80.6.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2588,18 +2588,18 @@
         ]
     )
     images = images.select(
         [
             pl.col("CaseNumber"),
             pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
             pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).str.to_time('%-H %M %S %p', strict=False).alias("Time"),
-            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').alias("Doc#"),
+            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').cast(pl.Int64, strict=False).alias("Doc#"),
             pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
             pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
-            pl.col("Images").str.extract(r'^(\d)\s').alias("Pages")
+            pl.col("Images").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("Pages")
         ])
     images = images.fill_null('')
     return images
 
 
 def _explode_case_action_summary(df, debug=False):
     cas = df.select(
@@ -2736,15 +2736,15 @@
             .alias("Settings"),
         ]
     )
     settings = settings.drop_nulls()
     settings = settings.select(
         [
             pl.col("CaseNumber"),
-            pl.col("Settings").str.extract(r'^(\d)\s').alias("#"),
+            pl.col("Settings").str.extract(r'^(\d)\s').cast(pl.Int64, strict=False).alias("#"),
             pl.col("Settings").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
             pl.col("Settings").str.extract(r'\s(\d\d\d)\s').alias("Que"),
             pl.col("Settings").str.extract(r'(\d\d \d\d [A|P]M)').str.to_time(r'%H %M %p', strict=False).alias("Time"),
             pl.col("Settings").str.extract(r'[A|P]M (.+)').str.strip().alias("Description")
         ])
     return settings
```

### Comparing `alacorder-80.6.2/PKG-INFO` & `alacorder-80.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.2
+Version: 80.6.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

