# Comparing `tmp/usearch-0.3.0-cp39-cp39-win_amd64.whl.zip` & `tmp/usearch-0.4.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 132686 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-17 22:28 usearch/__init__.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-17 22:28 usearch/client.py
--rw-rw-rw-  2.0 fat   273408 b- defN 23-May-17 22:40 usearch/index.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2298 b- defN 23-May-17 22:28 usearch/io.py
--rw-rw-rw-  2.0 fat     1203 b- defN 23-May-17 22:28 usearch/server.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    19489 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      770 b- defN 23-May-17 22:40 usearch-0.3.0.dist-info/RECORD
-10 files, 309885 bytes uncompressed, 131390 bytes compressed:  57.6%
+Zip file size: 134062 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-17 23:01 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-May-17 23:01 usearch/client.py
+-rw-rw-rw-  2.0 fat   275968 b- defN 23-May-17 23:09 usearch/index.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2298 b- defN 23-May-17 23:01 usearch/io.py
+-rw-rw-rw-  2.0 fat     1203 b- defN 23-May-17 23:01 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    19489 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      770 b- defN 23-May-17 23:09 usearch-0.4.0.dist-info/RECORD
+10 files, 312445 bytes uncompressed, 132766 bytes compressed:  57.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: usearch/io.py
 Comment: 
 
 Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-0.3.0.dist-info/LICENSE
+Filename: usearch-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-0.3.0.dist-info/METADATA
+Filename: usearch-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.3.0.dist-info/WHEEL
+Filename: usearch-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-0.3.0.dist-info/top_level.txt
+Filename: usearch-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch-0.3.0.dist-info/RECORD
+Filename: usearch-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `usearch-0.3.0.dist-info/LICENSE` & `usearch-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `usearch-0.3.0.dist-info/METADATA` & `usearch-0.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usearch
-Version: 0.3.0
+Version: 0.4.0
 Summary: Smaller & Faster Single-File Vector Search Engine from Unum
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usearch Version: 0.3.0 Summary: Smaller & Faster
+Metadata-Version: 2.1 Name: usearch Version: 0.4.0 Summary: Smaller & Faster
 Single-File Vector Search Engine from Unum License: Apache-2.0 Classifier:
 Development Status :: 4 - Beta Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: C++ Classifier: Operating System :: MacOS Classifier:
```

## Comparing `usearch-0.3.0.dist-info/RECORD` & `usearch-0.4.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 usearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 usearch/client.py,sha256=0QBbWSF-4qBm94f0sHVt1CmuL9Xi3b7tCnNSqt3Da9Q,1051
-usearch/index.cp39-win_amd64.pyd,sha256=-wK5k0ouTB9tk2s1cRJuV2HTIhwybiQRJEMMMXqNueE,273408
+usearch/index.cp39-win_amd64.pyd,sha256=eYC32ADxqEcBiOQsSQ7cp4MpG6ni7vA76rjdMoLmStg,275968
 usearch/io.py,sha256=xbieZtFNHPaG_1xFsoqQQdtuT_7s7DowdXK2BEphtzk,2298
 usearch/server.py,sha256=UmP2jabcTKeUVGU0Z-PMvEnjU9tkJDx-qstigg6Y0E4,1203
-usearch-0.3.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-usearch-0.3.0.dist-info/METADATA,sha256=mZBbyrPv2ryXFSZ0Z2i6Cn0eVLEU9f5K-viz_zd0Gww,19489
-usearch-0.3.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-usearch-0.3.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
-usearch-0.3.0.dist-info/RECORD,,
+usearch-0.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+usearch-0.4.0.dist-info/METADATA,sha256=HIvAiyybAOkzMeB-vZPhzoTxNzO9uars7tWUtT_oxJc,19489
+usearch-0.4.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+usearch-0.4.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
+usearch-0.4.0.dist-info/RECORD,,
```

