# Comparing `tmp/alacorder-80.6.0.1.tar.gz` & `tmp/alacorder-80.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.0.1.tar", max compression
+gzip compressed data, was "alacorder-80.6.1.tar", max compression
```

## Comparing `alacorder-80.6.0.1.tar` & `alacorder-80.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.0.1/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.0.1/README.md
--rw-r--r--   0        0        0      748 2023-05-17 18:01:35.060602 alacorder-80.6.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-17 17:59:02.346002 alacorder-80.6.0.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.0.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234285 2023-05-17 17:54:48.794246 alacorder-80.6.0.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234285 2023-05-17 17:54:52.738672 alacorder-80.6.0.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 alacorder-80.6.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.1/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.1/README.md
+-rw-r--r--   0        0        0      746 2023-05-18 14:21:45.241305 alacorder-80.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-18 14:22:01.526053 alacorder-80.6.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   233835 2023-05-18 14:21:34.032202 alacorder-80.6.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   233835 2023-05-18 14:21:30.079990 alacorder-80.6.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.1/PKG-INFO
```

### Comparing `alacorder-80.6.0.1/LICENSE` & `alacorder-80.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0.1/README.md` & `alacorder-80.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0.1/pyproject.toml` & `alacorder-80.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.0.1"
+version = "80.6.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.0.1/src/alacorder/.DS_Store` & `alacorder-80.6.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.0.1/src/alacorder/__main__.py` & `alacorder-80.6.1/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.0"
+version = "80.6.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2484,57 +2484,49 @@
             .alias("FEE_SEP"),
         ]
     )
     dlog(df.columns, df.shape, cf=debug)
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
-            pl.col("SPACE_SEP").arr.get(0).alias("AdminFee1"),
-            pl.col("SPACE_SEP").arr.get(1).alias("FeeStatus1"),
+            pl.col("SPACE_SEP").arr.get(0).alias("FeeStatus1"),
             pl.col("FEE_SEP").arr.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
             pl.col("FEE_SEP")
             .arr.get(1)
             .str.replace(r"\$", "")
             .alias("AmtPaid"),  # good
             pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
             pl.col("SPACE_SEP").arr.get(5).alias("FeeCode"),
             pl.col("Fees").str.extract(r"(\w00\d)").alias("Payor"),
             pl.col("Fees").str.extract(r"\s(\d\d\d)\s").alias("Payee"),
         ]
     )
     out = df.with_columns(
         [
             pl.col("CaseNumber"),
-            pl.when(pl.col("AdminFee1") != "ACTIVE")
+            pl.when(pl.col("FeeStatus1") != "ACTIVE")
             .then(True)
             .otherwise(False)
             .alias("TOT"),
-            pl.when(pl.col("AdminFee1") == "Total")
-            .then(pl.lit(None))
-            .otherwise(pl.col("FeeStatus1"))
-            .alias("FeeStatus2"),
             pl.when(pl.col("Balance1").is_in(["L", pl.Null]))
             .then("$0.00")
             .otherwise(pl.col("Balance1").str.replace_all(r"[A-Z]|\$", ""))
             .alias("AmtHold2"),
         ]
     )
     out = out.with_columns(
+        pl.col("Fees").str.extract(r'\s(Y|N)\s').alias("AdminFee"),
         pl.when(pl.col("TOT") == True)
         .then(pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", ""))
         .otherwise(pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", ""))
         .alias("AmtHold"),
         pl.when(pl.col("TOT") == False)
         .then(pl.col("SPACE_SEP").arr.get(0))
         .otherwise(pl.lit(""))
         .alias("FeeStatus"),
-        pl.when(pl.col("TOT") == False)
-        .then(pl.col("SPACE_SEP").arr.get(1))
-        .otherwise(pl.lit(""))
-        .alias("AdminFee"),
         pl.when(pl.col("TOT") == True)
         .then(pl.lit("Total:"))
         .otherwise(pl.lit(""))
         .alias("Total"),
     )
     dlog(out.columns, out.shape, cf=debug)
     out = out.with_columns(
@@ -2689,18 +2681,15 @@
             .str.replace(r"SJIS Witness List", "")
             .str.replace("Date Issued", "")
             .str.replace("Subpoena", "")
             .str.replace("List", "")
             .str.replace("Requesting Party Name Witness", "")
             .str.replace("Date: Time Code Comments", "")
             .str.replace(r"© Alacourt.com \d\d?/\d\d?/\d\d\d\d", "")
-            .str.replace(
-                r"Requesting Party Name Witness # Date Served Service Type Attorney Issued Type   Date Issued   Subpoena",
-                "",
-            )
+            .str.replace(r'\#','')
             .str.replace_all(r"[A-Z][a-z]+", " ")
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip()
             .alias("Witnesses"),
         ]
     )
     return wit.drop_nulls()
```

### Comparing `alacorder-80.6.0.1/src/alacorder/alac.py` & `alacorder-80.6.1/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.0"
+version = "80.6.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2484,57 +2484,49 @@
             .alias("FEE_SEP"),
         ]
     )
     dlog(df.columns, df.shape, cf=debug)
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
-            pl.col("SPACE_SEP").arr.get(0).alias("AdminFee1"),
-            pl.col("SPACE_SEP").arr.get(1).alias("FeeStatus1"),
+            pl.col("SPACE_SEP").arr.get(0).alias("FeeStatus1"),
             pl.col("FEE_SEP").arr.get(0).str.replace(r"\$", "").alias("AmtDue"),  # good
             pl.col("FEE_SEP")
             .arr.get(1)
             .str.replace(r"\$", "")
             .alias("AmtPaid"),  # good
             pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", "").alias("Balance1"),
             pl.col("SPACE_SEP").arr.get(5).alias("FeeCode"),
             pl.col("Fees").str.extract(r"(\w00\d)").alias("Payor"),
             pl.col("Fees").str.extract(r"\s(\d\d\d)\s").alias("Payee"),
         ]
     )
     out = df.with_columns(
         [
             pl.col("CaseNumber"),
-            pl.when(pl.col("AdminFee1") != "ACTIVE")
+            pl.when(pl.col("FeeStatus1") != "ACTIVE")
             .then(True)
             .otherwise(False)
             .alias("TOT"),
-            pl.when(pl.col("AdminFee1") == "Total")
-            .then(pl.lit(None))
-            .otherwise(pl.col("FeeStatus1"))
-            .alias("FeeStatus2"),
             pl.when(pl.col("Balance1").is_in(["L", pl.Null]))
             .then("$0.00")
             .otherwise(pl.col("Balance1").str.replace_all(r"[A-Z]|\$", ""))
             .alias("AmtHold2"),
         ]
     )
     out = out.with_columns(
+        pl.col("Fees").str.extract(r'\s(Y|N)\s').alias("AdminFee"),
         pl.when(pl.col("TOT") == True)
         .then(pl.col("FEE_SEP").arr.get(-1).str.replace(r"\$", ""))
         .otherwise(pl.col("FEE_SEP").arr.get(2).str.replace(r"\$", ""))
         .alias("AmtHold"),
         pl.when(pl.col("TOT") == False)
         .then(pl.col("SPACE_SEP").arr.get(0))
         .otherwise(pl.lit(""))
         .alias("FeeStatus"),
-        pl.when(pl.col("TOT") == False)
-        .then(pl.col("SPACE_SEP").arr.get(1))
-        .otherwise(pl.lit(""))
-        .alias("AdminFee"),
         pl.when(pl.col("TOT") == True)
         .then(pl.lit("Total:"))
         .otherwise(pl.lit(""))
         .alias("Total"),
     )
     dlog(out.columns, out.shape, cf=debug)
     out = out.with_columns(
@@ -2689,18 +2681,15 @@
             .str.replace(r"SJIS Witness List", "")
             .str.replace("Date Issued", "")
             .str.replace("Subpoena", "")
             .str.replace("List", "")
             .str.replace("Requesting Party Name Witness", "")
             .str.replace("Date: Time Code Comments", "")
             .str.replace(r"© Alacourt.com \d\d?/\d\d?/\d\d\d\d", "")
-            .str.replace(
-                r"Requesting Party Name Witness # Date Served Service Type Attorney Issued Type   Date Issued   Subpoena",
-                "",
-            )
+            .str.replace(r'\#','')
             .str.replace_all(r"[A-Z][a-z]+", " ")
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip()
             .alias("Witnesses"),
         ]
     )
     return wit.drop_nulls()
```

### Comparing `alacorder-80.6.0.1/PKG-INFO` & `alacorder-80.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.0.1
+Version: 80.6.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

