# Comparing `tmp/gs_engine-0.22.0a20230515-py2.py3-none-macosx_12_0_arm64.whl.zip` & `tmp/gs_engine-0.22.0a20230516-py2.py3-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11911 bytes, number of entries: 9
--rw-r--r--  2.0 unx      694 b- defN 23-May-15 08:41 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      840 b- defN 23-May-15 02:20 gs_engine-0.22.0a20230515.dist-info/RECORD
--rw-r--r--  2.0 unx      138 b- defN 23-May-15 09:16 gs_engine-0.22.0a20230515.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-15 09:16 gs_engine-0.22.0a20230515.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21664 b- defN 23-May-15 09:16 gs_engine-0.22.0a20230515.dist-info/METADATA
--rw-r--r--  2.0 unx     1573 b- defN 23-May-15 08:41 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-May-15 08:41 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-May-15 08:41 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-May-15 08:41 graphscope.runtime/conf/log4rs.yml
-9 files, 26034 bytes uncompressed, 10449 bytes compressed:  59.9%
+Zip file size: 11910 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      840 b- defN 23-May-16 21:10 gs_engine-0.22.0a20230516.dist-info/RECORD
+-rw-r--r--  2.0 unx      140 b- defN 23-May-16 20:58 gs_engine-0.22.0a20230516.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-16 20:58 gs_engine-0.22.0a20230516.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    21664 b- defN 23-May-16 20:58 gs_engine-0.22.0a20230516.dist-info/METADATA
+-rw-r--r--  2.0 unx      694 b- defN 23-May-16 19:05 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx     1573 b- defN 23-May-16 19:05 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      398 b- defN 23-May-16 19:05 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      504 b- defN 23-May-16 19:05 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx      204 b- defN 23-May-16 19:05 graphscope.runtime/conf/log4rs.yml
+9 files, 26036 bytes uncompressed, 10448 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: graphscope_runtime/__init__.py
+Filename: gs_engine-0.22.0a20230516.dist-info/RECORD
 Comment: 
 
-Filename: gs_engine-0.22.0a20230515.dist-info/RECORD
+Filename: gs_engine-0.22.0a20230516.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.22.0a20230515.dist-info/WHEEL
+Filename: gs_engine-0.22.0a20230516.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.22.0a20230515.dist-info/top_level.txt
+Filename: gs_engine-0.22.0a20230516.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.22.0a20230515.dist-info/METADATA
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
 Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
 Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment:
```

## Comparing `gs_engine-0.22.0a20230515.dist-info/METADATA` & `gs_engine-0.22.0a20230516.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.22.0a20230515
+Version: 0.22.0a20230516
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

