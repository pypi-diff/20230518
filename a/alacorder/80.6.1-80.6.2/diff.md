# Comparing `tmp/alacorder-80.6.1.tar.gz` & `tmp/alacorder-80.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.1.tar", max compression
+gzip compressed data, was "alacorder-80.6.2.tar", max compression
```

## Comparing `alacorder-80.6.1.tar` & `alacorder-80.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.1/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.1/README.md
--rw-r--r--   0        0        0      746 2023-05-18 14:21:45.241305 alacorder-80.6.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-18 14:22:01.526053 alacorder-80.6.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   233835 2023-05-18 14:21:34.032202 alacorder-80.6.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   233835 2023-05-18 14:21:30.079990 alacorder-80.6.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.2/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.2/README.md
+-rw-r--r--   0        0        0      746 2023-05-18 16:26:19.428735 alacorder-80.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-18 16:26:13.972097 alacorder-80.6.2/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234128 2023-05-18 16:25:56.123146 alacorder-80.6.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234128 2023-05-18 16:25:50.985997 alacorder-80.6.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.2/PKG-INFO
```

### Comparing `alacorder-80.6.1/LICENSE` & `alacorder-80.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.1/README.md` & `alacorder-80.6.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.1/pyproject.toml` & `alacorder-80.6.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.1"
+version = "80.6.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.1/src/alacorder/.DS_Store` & `alacorder-80.6.2/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.1/src/alacorder/__main__.py` & `alacorder-80.6.2/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.1"
+version = "80.6.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -174,18 +174,20 @@
     print("Parsing witnesses...", cf=cf)
     wit = _explode_witnesses(df)
     print("Parsing attorneys...", cf=cf)
     att = _explode_attorneys(df)
     print("Parsing images...", cf=cf)
     img = _explode_images(df)
     dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
-    ch_filing = ch.filter(pl.col("Filing") == True).select(
-        pl.exclude("CourtAction", "CourtActionDate")
+    ch_filing = ch.filter(pl.col("Filing")).select(
+        pl.exclude("CourtAction", "CourtActionDate", "PaymentToRestore", "TotalBalance", "Filing", "Disposition", "CERVDisqConviction", "PardonDisqConviction", "PermanentDisqConviction", "Conviction")
+    )
+    ch_disposition = ch.filter(pl.col("Disposition")).select(
+        pl.exclude("Filing", "Disposition")
     )
-    ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             [ca, ch_filing, ch_disposition, fs, fh, sent, settings, cas, wit, att, img],
             sheet_names=[
                 "cases",
                 "filing-charges",
@@ -1584,23 +1586,14 @@
             .str.strip()
             .alias("ALInstitutionalServiceNum"),
             pl.col("AllPagesText")
             .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("Retrieved"),
             pl.col("AllPagesText")
-            .str.extract(
-                r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)"
-            )
-            .alias("CourtAction"),
-            pl.col("AllPagesText")
-            .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("CourtActionDate"),
-            pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
             .cast(pl.Categorical)
             .alias("JuryDemand"),
             pl.col("AllPagesText")
             .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
             .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
@@ -2012,33 +2005,31 @@
 
     cases = cases.fill_null("")
 
     cases = cases.select(
         "Retrieved",
         "CaseNumber",
         "Name",
+        "Alias",
         "DOB",
         "Race",
         "Sex",
-        "CourtAction",
-        "CourtActionDate",
         "TotalAmtDue",
         "TotalAmtPaid",
         "TotalBalance",
         "TotalAmtHold",
         "D999",
         "BondAmt",
         "Phone",
         "StreetAddress",
         "City",
         "State",
         "ZipCode",
         "County",
         "Country",
-        "Alias",
         "SSN",
         "Weight",
         "Eyes",
         "Hair",
         "FilingDate",
         "CaseInitiationDate",
         "ArrestDate",
@@ -2592,14 +2583,25 @@
             pl.col("CaseNumber"),
             pl.col("Images")
             .str.replace_all(r"[A-Z][a-z]+", " ")
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip(),
         ]
     )
+    images = images.select(
+        [
+            pl.col("CaseNumber"),
+            pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
+            pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).str.to_time('%-H %M %S %p', strict=False).alias("Time"),
+            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').alias("Doc#"),
+            pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
+            pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
+            pl.col("Images").str.extract(r'^(\d)\s').alias("Pages")
+        ])
+    images = images.fill_null('')
     return images
 
 
 def _explode_case_action_summary(df, debug=False):
     cas = df.select(
         [
             pl.concat_str(
@@ -2730,16 +2732,25 @@
             pl.col("SET1")
             .str.replace_all(r"[A-Z][a-z]+", " ")
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip()
             .alias("Settings"),
         ]
     )
-    return settings.drop_nulls()
-
+    settings = settings.drop_nulls()
+    settings = settings.select(
+        [
+            pl.col("CaseNumber"),
+            pl.col("Settings").str.extract(r'^(\d)\s').alias("#"),
+            pl.col("Settings").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
+            pl.col("Settings").str.extract(r'\s(\d\d\d)\s').alias("Que"),
+            pl.col("Settings").str.extract(r'(\d\d \d\d [A|P]M)').str.to_time(r'%H %M %p', strict=False).alias("Time"),
+            pl.col("Settings").str.extract(r'[A|P]M (.+)').str.strip().alias("Description")
+        ])
+    return settings
 
 def _explode_split_sentences(df, debug=False):
     sent = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
@@ -2908,28 +2919,14 @@
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
             pl.col("Sentence")
-            .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
-            .str.replace("© Alacourt.com", "", literal=True)
-            .str.replace(r"Split.+", "")
-            .str.replace(r"Confinement.+", "")
-            .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
-            .str.replace(r"\$|Recipient", "")
-            .str.replace(r'PrelimHearing\:X?','')
-            .str.replace(r'SX10\:X?','')
-            .str.replace(r'DemandReductionHearing\:\d+\.\d\d','')
-            .str.replace(r'Subpoena\:X?','')
-            .str.replace(r'AttorneyFees\:','')
-            .str.replace_all(r"\s+", "")
-            .alias("AttorneyFees"),
-            pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(
                 r"Total Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
```

### Comparing `alacorder-80.6.1/src/alacorder/alac.py` & `alacorder-80.6.2/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.1"
+version = "80.6.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -174,18 +174,20 @@
     print("Parsing witnesses...", cf=cf)
     wit = _explode_witnesses(df)
     print("Parsing attorneys...", cf=cf)
     att = _explode_attorneys(df)
     print("Parsing images...", cf=cf)
     img = _explode_images(df)
     dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
-    ch_filing = ch.filter(pl.col("Filing") == True).select(
-        pl.exclude("CourtAction", "CourtActionDate")
+    ch_filing = ch.filter(pl.col("Filing")).select(
+        pl.exclude("CourtAction", "CourtActionDate", "PaymentToRestore", "TotalBalance", "Filing", "Disposition", "CERVDisqConviction", "PardonDisqConviction", "PermanentDisqConviction", "Conviction")
+    )
+    ch_disposition = ch.filter(pl.col("Disposition")).select(
+        pl.exclude("Filing", "Disposition")
     )
-    ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             [ca, ch_filing, ch_disposition, fs, fh, sent, settings, cas, wit, att, img],
             sheet_names=[
                 "cases",
                 "filing-charges",
@@ -1584,23 +1586,14 @@
             .str.strip()
             .alias("ALInstitutionalServiceNum"),
             pl.col("AllPagesText")
             .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("Retrieved"),
             pl.col("AllPagesText")
-            .str.extract(
-                r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)"
-            )
-            .alias("CourtAction"),
-            pl.col("AllPagesText")
-            .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date("%m/%d/%Y", strict=False)
-            .alias("CourtActionDate"),
-            pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
             .cast(pl.Categorical)
             .alias("JuryDemand"),
             pl.col("AllPagesText")
             .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
             .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
@@ -2012,33 +2005,31 @@
 
     cases = cases.fill_null("")
 
     cases = cases.select(
         "Retrieved",
         "CaseNumber",
         "Name",
+        "Alias",
         "DOB",
         "Race",
         "Sex",
-        "CourtAction",
-        "CourtActionDate",
         "TotalAmtDue",
         "TotalAmtPaid",
         "TotalBalance",
         "TotalAmtHold",
         "D999",
         "BondAmt",
         "Phone",
         "StreetAddress",
         "City",
         "State",
         "ZipCode",
         "County",
         "Country",
-        "Alias",
         "SSN",
         "Weight",
         "Eyes",
         "Hair",
         "FilingDate",
         "CaseInitiationDate",
         "ArrestDate",
@@ -2592,14 +2583,25 @@
             pl.col("CaseNumber"),
             pl.col("Images")
             .str.replace_all(r"[A-Z][a-z]+", " ")
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip(),
         ]
     )
+    images = images.select(
+        [
+            pl.col("CaseNumber"),
+            pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=1).str.to_date('%-m/%-d/%Y', strict=False).alias("Date"),
+            pl.col("Images").str.extract(r'(\d\d?/\d\d?/\d\d\d\d) (\d\d? \d\d? \d\d? [A|P]M)', group_index=2).str.to_time('%-H %M %S %p', strict=False).alias("Time"),
+            pl.col("Images").str.extract(r'^\d\s.+?\s(\d)').alias("Doc#"),
+            pl.col("Images").str.extract(r'^\d\s(.+?)\s\d').alias("Title"),
+            pl.col("Images").str.extract(r'^\d\s.+?\s\d\s(.+?)\s\d\d?/\d\d?/\d\d\d\d').alias("Description"),
+            pl.col("Images").str.extract(r'^(\d)\s').alias("Pages")
+        ])
+    images = images.fill_null('')
     return images
 
 
 def _explode_case_action_summary(df, debug=False):
     cas = df.select(
         [
             pl.concat_str(
@@ -2730,16 +2732,25 @@
             pl.col("SET1")
             .str.replace_all(r"[A-Z][a-z]+", " ")
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip()
             .alias("Settings"),
         ]
     )
-    return settings.drop_nulls()
-
+    settings = settings.drop_nulls()
+    settings = settings.select(
+        [
+            pl.col("CaseNumber"),
+            pl.col("Settings").str.extract(r'^(\d)\s').alias("#"),
+            pl.col("Settings").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Date"),
+            pl.col("Settings").str.extract(r'\s(\d\d\d)\s').alias("Que"),
+            pl.col("Settings").str.extract(r'(\d\d \d\d [A|P]M)').str.to_time(r'%H %M %p', strict=False).alias("Time"),
+            pl.col("Settings").str.extract(r'[A|P]M (.+)').str.strip().alias("Description")
+        ])
+    return settings
 
 def _explode_split_sentences(df, debug=False):
     sent = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
@@ -2908,28 +2919,14 @@
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
             pl.col("Sentence")
-            .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
-            .str.replace("© Alacourt.com", "", literal=True)
-            .str.replace(r"Split.+", "")
-            .str.replace(r"Confinement.+", "")
-            .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
-            .str.replace(r"\$|Recipient", "")
-            .str.replace(r'PrelimHearing\:X?','')
-            .str.replace(r'SX10\:X?','')
-            .str.replace(r'DemandReductionHearing\:\d+\.\d\d','')
-            .str.replace(r'Subpoena\:X?','')
-            .str.replace(r'AttorneyFees\:','')
-            .str.replace_all(r"\s+", "")
-            .alias("AttorneyFees"),
-            pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(
                 r"Total Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
```

### Comparing `alacorder-80.6.1/PKG-INFO` & `alacorder-80.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.1
+Version: 80.6.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

