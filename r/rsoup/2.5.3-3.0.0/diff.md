# Comparing `tmp/rsoup-2.5.3-cp39-none-win_amd64.whl.zip` & `tmp/rsoup-3.0.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 829488 bytes, number of entries: 14
--rw-r--r--  4.6 unx      893 b- defN 23-Mar-24 01:03 rsoup-2.5.3.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Mar-24 01:03 rsoup-2.5.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     1085 b- defN 23-Mar-24 01:03 rsoup-2.5.3.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      604 b- defN 23-Mar-24 01:03 rsoup/exceptions.py
--rw-r--r--  4.6 unx      583 b- defN 23-Mar-24 01:03 rsoup/fetch_tables.py
--rw-r--r--  4.6 unx    15633 b- defN 23-Mar-24 01:03 rsoup/python/context_extractor.py
--rw-r--r--  4.6 unx     3201 b- defN 23-Mar-24 01:03 rsoup/python/models/context.py
--rw-r--r--  4.6 unx    10137 b- defN 23-Mar-24 01:03 rsoup/python/models/html_table.py
--rw-r--r--  4.6 unx        0 b- defN 23-Mar-24 01:03 rsoup/python/models/__init__.py
--rw-r--r--  4.6 unx    11447 b- defN 23-Mar-24 01:03 rsoup/python/table_extractor.py
--rw-r--r--  4.6 unx     4374 b- defN 23-Mar-24 01:03 rsoup/rsoup.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Mar-24 01:03 rsoup/__init__.py
--rwxr-xr-x  4.6 unx  2161664 b- defN 23-Mar-24 01:03 rsoup/rsoup.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx     1127 b- defN 23-Mar-24 01:03 rsoup-2.5.3.dist-info/RECORD
-14 files, 2210844 bytes uncompressed, 827626 bytes compressed:  62.6%
+Zip file size: 833733 bytes, number of entries: 14
+-rw-r--r--  4.6 unx      893 b- defN 23-May-17 01:57 rsoup-3.0.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-May-17 01:57 rsoup-3.0.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1085 b- defN 23-May-17 01:57 rsoup-3.0.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     4374 b- defN 23-May-17 01:57 rsoup/core.pyi
+-rw-r--r--  4.6 unx      604 b- defN 23-May-17 01:57 rsoup/exceptions.py
+-rw-r--r--  4.6 unx      583 b- defN 23-May-17 01:57 rsoup/fetch_tables.py
+-rw-r--r--  4.6 unx    15633 b- defN 23-May-17 01:57 rsoup/python/context_extractor.py
+-rw-r--r--  4.6 unx     3201 b- defN 23-May-17 01:57 rsoup/python/models/context.py
+-rw-r--r--  4.6 unx    10137 b- defN 23-May-17 01:57 rsoup/python/models/html_table.py
+-rw-r--r--  4.6 unx        0 b- defN 23-May-17 01:57 rsoup/python/models/__init__.py
+-rw-r--r--  4.6 unx    11447 b- defN 23-May-17 01:57 rsoup/python/table_extractor.py
+-rw-r--r--  4.6 unx        0 b- defN 23-May-17 01:57 rsoup/__init__.py
+-rwxr-xr-x  4.6 unx  2175488 b- defN 23-May-17 01:57 rsoup/core.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx     1125 b- defN 23-May-17 01:57 rsoup-3.0.0.dist-info/RECORD
+14 files, 2224666 bytes uncompressed, 831875 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,14 +1,17 @@
-Filename: rsoup-2.5.3.dist-info/METADATA
+Filename: rsoup-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: rsoup-2.5.3.dist-info/WHEEL
+Filename: rsoup-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: rsoup-2.5.3.dist-info/license_files/LICENSE
+Filename: rsoup-3.0.0.dist-info/license_files/LICENSE
+Comment: 
+
+Filename: rsoup/core.pyi
 Comment: 
 
 Filename: rsoup/exceptions.py
 Comment: 
 
 Filename: rsoup/fetch_tables.py
 Comment: 
@@ -24,20 +27,17 @@
 
 Filename: rsoup/python/models/__init__.py
 Comment: 
 
 Filename: rsoup/python/table_extractor.py
 Comment: 
 
-Filename: rsoup/rsoup.pyi
-Comment: 
-
 Filename: rsoup/__init__.py
 Comment: 
 
-Filename: rsoup/rsoup.cp39-win_amd64.pyd
+Filename: rsoup/core.cp39-win_amd64.pyd
 Comment: 
 
-Filename: rsoup-2.5.3.dist-info/RECORD
+Filename: rsoup-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rsoup-2.5.3.dist-info/METADATA` & `rsoup-3.0.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsoup
-Version: 2.5.3
+Version: 3.0.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: beautifulsoup4 >= 4.9.3, < 5.0.0
 Requires-Dist: html5lib >= 1.1.0, < 2.0.0
 Requires-Dist: requests >= 2.28.0, < 3.0.0
 Requires-Dist: tabulate >= 0.8.10
 Requires-Dist: pytest >= 7.1.3, < 8.0.0; extra == 'dev'
```

## Comparing `rsoup-2.5.3.dist-info/license_files/LICENSE` & `rsoup-3.0.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `rsoup/rsoup.pyi` & `rsoup/core.pyi`

 * *Files identical despite different names*

## Comparing `rsoup-2.5.3.dist-info/RECORD` & `rsoup-3.0.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-rsoup-2.5.3.dist-info/METADATA,sha256=cO7XRfMuHJ1MCXIrReyeSf6vgrhanNeW_MzU6ghT14Y,893
-rsoup-2.5.3.dist-info/WHEEL,sha256=FJL2ou7K5V0ITYVnNpdqdDvfSZSOqe03YPiBtWkAJ5k,96
-rsoup-2.5.3.dist-info/license_files/LICENSE,sha256=takhlO4EcEdY_bLxK8ZY-StVLn9i5hlTi95OQ6LhRB8,1085
+rsoup-3.0.0.dist-info/METADATA,sha256=vFOlgEPmKvkQSOKrEhYBtoQDdG9sgi79y0D_TvBWp0I,893
+rsoup-3.0.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+rsoup-3.0.0.dist-info/license_files/LICENSE,sha256=takhlO4EcEdY_bLxK8ZY-StVLn9i5hlTi95OQ6LhRB8,1085
+rsoup/core.pyi,sha256=t199efSN-DHMOknlHQ8f7IaBSDlaGhDuEbReXewdtIw,4374
 rsoup/exceptions.py,sha256=v0__zf9lYzxZJdXlboOGDxdEgEUZvLc-IN8OEOwKU5k,604
 rsoup/fetch_tables.py,sha256=C3CPDxck3cnAWjJhxOIzrHv-0pxLWB7sJgmuXgAP4O8,583
 rsoup/python/context_extractor.py,sha256=S7PY704ZeAt69z08swAx3yFaac4rCf87Uw_4SgKj0IY,15633
 rsoup/python/models/context.py,sha256=OIVv9Vw70Ocop_ICe0AoYCrM-cCBEPMbEm8MSBB-6PA,3201
 rsoup/python/models/html_table.py,sha256=P0orxGQ8grmx1_-kUsajHc1iCFJpaJYKX4IHfbru25g,10137
 rsoup/python/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rsoup/python/table_extractor.py,sha256=B0sPRqAwC5Xg2dVq1dbbZ4xgq5P_7p9rNz3Djhjq-gw,11447
-rsoup/rsoup.pyi,sha256=t199efSN-DHMOknlHQ8f7IaBSDlaGhDuEbReXewdtIw,4374
 rsoup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rsoup/rsoup.cp39-win_amd64.pyd,sha256=PriE-Axg0qMVghqQnY1filynYt2AFOp3AsKro8Y3nic,2161664
-rsoup-2.5.3.dist-info/RECORD,,
+rsoup/core.cp39-win_amd64.pyd,sha256=jvN4CLol8aC6XRgYk7LKdZ3iQqnne7oj-HDFQ5GWIS4,2175488
+rsoup-3.0.0.dist-info/RECORD,,
```

