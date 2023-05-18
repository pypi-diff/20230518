# Comparing `tmp/anyon-3.2.2-cp311-cp311-win_amd64.whl.zip` & `tmp/anyon-3.2.3-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 366291 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-15 06:28 anyon-3.2.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1191 b- defN 23-May-15 06:28 anyon-3.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-15 06:28 anyon-3.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-15 06:28 anyon-3.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      376 b- defN 23-May-15 06:28 anyon-3.2.2.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-May-15 06:28 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    76288 b- defN 23-May-15 06:28 anyon/loader.pyd
--rw-rw-rw-  2.0 fat    99840 b- defN 23-May-15 06:28 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   179712 b- defN 23-May-15 06:28 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-May-15 06:28 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    92672 b- defN 23-May-15 06:28 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   134144 b- defN 23-May-15 06:28 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    61952 b- defN 23-May-15 06:28 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   114176 b- defN 23-May-15 06:28 anyon/stage/device.pyd
-14 files, 803006 bytes uncompressed, 364529 bytes compressed:  54.6%
+Zip file size: 363935 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-18 13:24 anyon-3.2.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-May-18 13:24 anyon-3.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-18 13:24 anyon-3.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-18 13:24 anyon-3.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      376 b- defN 23-May-18 13:24 anyon-3.2.3.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    20480 b- defN 23-May-18 13:24 anyon/__init__.pyd
+-rw-rw-rw-  2.0 fat    75776 b- defN 23-May-18 13:24 anyon/loader.pyd
+-rw-rw-rw-  2.0 fat    99328 b- defN 23-May-18 13:24 anyon/remote.pyd
+-rw-rw-rw-  2.0 fat   176640 b- defN 23-May-18 13:24 anyon/server.pyd
+-rw-rw-rw-  2.0 fat    20992 b- defN 23-May-18 13:24 anyon/stage/__init__.pyd
+-rw-rw-rw-  2.0 fat    94208 b- defN 23-May-18 13:24 anyon/stage/calculator.pyd
+-rw-rw-rw-  2.0 fat   133632 b- defN 23-May-18 13:24 anyon/stage/compiler.pyd
+-rw-rw-rw-  2.0 fat    62976 b- defN 23-May-18 13:24 anyon/stage/demodulator.pyd
+-rw-rw-rw-  2.0 fat   114176 b- defN 23-May-18 13:24 anyon/stage/device.pyd
+14 files, 800958 bytes uncompressed, 362173 bytes compressed:  54.8%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: anyon-3.2.2.dist-info/LICENSE
+Filename: anyon-3.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.2.2.dist-info/METADATA
+Filename: anyon-3.2.3.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.2.2.dist-info/WHEEL
+Filename: anyon-3.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.2.2.dist-info/top_level.txt
+Filename: anyon-3.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.2.2.dist-info/RECORD
+Filename: anyon-3.2.3.dist-info/RECORD
 Comment: 
 
 Filename: anyon/__init__.pyd
 Comment: 
 
 Filename: anyon/loader.pyd
 Comment:
```

## Comparing `anyon-3.2.2.dist-info/LICENSE` & `anyon-3.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anyon-3.2.2.dist-info/METADATA` & `anyon-3.2.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyon
-Version: 3.2.2
+Version: 3.2.3
 Summary: Dream It Possible!
 Home-page: https://gitee.com/
 Author: YL Feng
 Author-email: fengyulong@pku.edu.cn
 License: MIT
 Project-URL: source, https://gitee.com
 Keywords: Hello,World!
@@ -19,15 +19,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: axion (>=3.3.1)
+Requires-Dist: axion (>=3.3.3)
 Requires-Dist: srpc (>=4.2.8)
 Requires-Dist: zee (>=0.0.2)
 Requires-Dist: requests (>=2.28.0)
 
 #### 介绍
```

