# Comparing `tmp/alacorder-80.6.3.tar.gz` & `tmp/alacorder-80.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.3.tar", max compression
+gzip compressed data, was "alacorder-80.6.4.tar", max compression
```

## Comparing `alacorder-80.6.3.tar` & `alacorder-80.6.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.3/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.3/README.md
--rw-r--r--   0        0        0      746 2023-05-18 16:59:39.102314 alacorder-80.6.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-18 16:59:38.772596 alacorder-80.6.3/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.3/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234215 2023-05-18 16:59:13.235012 alacorder-80.6.3/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234215 2023-05-18 16:59:09.146003 alacorder-80.6.3/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.4/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.4/README.md
+-rw-r--r--   0        0        0      746 2023-05-18 17:49:14.768333 alacorder-80.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-18 17:49:24.483501 alacorder-80.6.4/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.4/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234228 2023-05-18 17:48:17.428661 alacorder-80.6.4/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234228 2023-05-18 17:48:12.889832 alacorder-80.6.4/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.4/PKG-INFO
```

### Comparing `alacorder-80.6.3/LICENSE` & `alacorder-80.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.3/README.md` & `alacorder-80.6.4/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.3/pyproject.toml` & `alacorder-80.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.3"
+version = "80.6.4"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.3/src/alacorder/.DS_Store` & `alacorder-80.6.4/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.3/src/alacorder/__main__.py` & `alacorder-80.6.4/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.3"
+version = "80.6.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2247,15 +2247,15 @@
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
             pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)")
+            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
                 r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
@@ -2379,15 +2379,15 @@
             .then("020-002-143(A)")
             .otherwise(pl.col("Cite"))
             .alias("Cite")
         ]
     )
     charges = charges.with_columns(
         [
-            pl.col("Charges").str.extract(r'\s(A|S|C)\s').alias("ID"),
+            pl.col("Charges").str.extract(r'\s(A|S|C|P)\s').alias("ID"),
             pl.concat_str(
                 [
                     pl.col("CaseNumber"),
                     pl.lit(" - "),
                     pl.col("Num"),
                     pl.lit(" "),
                     pl.col("Cite"),
```

### Comparing `alacorder-80.6.3/src/alacorder/alac.py` & `alacorder-80.6.4/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.3"
+version = "80.6.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2247,15 +2247,15 @@
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
             pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)")
+            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
                 r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
@@ -2379,15 +2379,15 @@
             .then("020-002-143(A)")
             .otherwise(pl.col("Cite"))
             .alias("Cite")
         ]
     )
     charges = charges.with_columns(
         [
-            pl.col("Charges").str.extract(r'\s(A|S|C)\s').alias("ID"),
+            pl.col("Charges").str.extract(r'\s(A|S|C|P)\s').alias("ID"),
             pl.concat_str(
                 [
                     pl.col("CaseNumber"),
                     pl.lit(" - "),
                     pl.col("Num"),
                     pl.lit(" "),
                     pl.col("Cite"),
```

### Comparing `alacorder-80.6.3/PKG-INFO` & `alacorder-80.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.3
+Version: 80.6.4
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

