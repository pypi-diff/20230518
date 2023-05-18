# Comparing `tmp/berlin-0.3.3-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/berlin-0.3.4-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8961654 bytes, number of entries: 7
--rw-r--r--  4.6 unx     5280 b- defN 23-May-04 22:45 berlin-0.3.3.dist-info/METADATA
--rw-r--r--  4.6 unx      141 b- defN 23-May-04 22:45 berlin-0.3.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     2434 b- defN 23-May-04 22:45 berlin-0.3.3.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx      307 b- defN 23-May-04 22:45 berlin/_utils.py
--rw-r--r--  4.6 unx       41 b- defN 23-May-04 22:45 berlin/__init__.py
--rwxr-xr-x  4.6 unx 42792264 b- defN 23-May-04 22:45 berlin/berlin.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      559 b- defN 23-May-04 22:45 berlin-0.3.3.dist-info/RECORD
-7 files, 42801026 bytes uncompressed, 8960672 bytes compressed:  79.1%
+Zip file size: 8961683 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     5280 b- defN 23-May-18 08:20 berlin-0.3.4.dist-info/METADATA
+-rw-r--r--  4.6 unx      135 b- defN 23-May-18 08:20 berlin-0.3.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2434 b- defN 23-May-18 08:20 berlin-0.3.4.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx      307 b- defN 23-May-18 08:20 berlin/_utils.py
+-rw-r--r--  4.6 unx       64 b- defN 23-May-18 08:20 berlin/__init__.py
+-rwxr-xr-x  4.6 unx 42792264 b- defN 23-May-18 08:20 berlin/berlin.pypy39-pp73-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      559 b- defN 23-May-18 08:20 berlin-0.3.4.dist-info/RECORD
+7 files, 42801043 bytes uncompressed, 8960701 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: berlin-0.3.3.dist-info/METADATA
+Filename: berlin-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: berlin-0.3.3.dist-info/WHEEL
+Filename: berlin-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: berlin-0.3.3.dist-info/license_files/LICENSE.md
+Filename: berlin-0.3.4.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: berlin/_utils.py
 Comment: 
 
 Filename: berlin/__init__.py
 Comment: 
 
 Filename: berlin/berlin.pypy39-pp73-x86_64-linux-gnu.so
 Comment: 
 
-Filename: berlin-0.3.3.dist-info/RECORD
+Filename: berlin-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## berlin/__init__.py

```diff
@@ -1 +1,3 @@
 from .berlin import load, load_from_json
+
+__version__ = "0.3.4"
```

## Comparing `berlin-0.3.3.dist-info/METADATA` & `berlin-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin
-Version: 0.3.3
+Version: 0.3.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Summary: Identify locations and tag them with UN-LOCODEs and ISO-3166-2 subdivisions.
 Keywords: geospatial,nlp,search
 Author-email: Metin Akat <metin.akat@flaxandteal.co.uk>, Phil Weir <phil.weir@flaxandteal.co.uk>
```

## Comparing `berlin-0.3.3.dist-info/license_files/LICENSE.md` & `berlin-0.3.4.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `berlin-0.3.3.dist-info/RECORD` & `berlin-0.3.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-berlin-0.3.3.dist-info/METADATA,sha256=_7T_Ep7zq64Qr7HqQY7JJnNCguoMVa4WifdxLQfnWmA,5280
-berlin-0.3.3.dist-info/WHEEL,sha256=9IAI9PX3s07tPjzHDDtrj8814ohxpbgN8qwu0vXhmAQ,141
-berlin-0.3.3.dist-info/license_files/LICENSE.md,sha256=O9qRokRsn17u3gf-vcikAvva7Mf52cJlnTTwqFD6ikk,2434
+berlin-0.3.4.dist-info/METADATA,sha256=ZhcBkXTQBvnwUxp0Vk6bZZEHJExoWwUeFwYSWU8Z7WU,5280
+berlin-0.3.4.dist-info/WHEEL,sha256=7nzcOH2DCNqGWfOERaPgA7pT5OZfgVIAA60cBfq1Is0,135
+berlin-0.3.4.dist-info/license_files/LICENSE.md,sha256=O9qRokRsn17u3gf-vcikAvva7Mf52cJlnTTwqFD6ikk,2434
 berlin/_utils.py,sha256=7udQN_hRB3QaMre_pp85dafHJgC4k7FLXlyWZxCDMto,307
-berlin/__init__.py,sha256=T4d3ssJBbZA6zuc4v93Rl9GcL8_Bv9jxASYBwdjS16s,41
+berlin/__init__.py,sha256=jS40CeWnkcc6KdU_cAqRqhPNmYhkkt5VbfGnts-RD-E,64
 berlin/berlin.pypy39-pp73-x86_64-linux-gnu.so,sha256=Br_6L3D5GgmJe583bu-sfw-Qbwjplk-XgrPlUOyQQR4,42792264
-berlin-0.3.3.dist-info/RECORD,,
+berlin-0.3.4.dist-info/RECORD,,
```

