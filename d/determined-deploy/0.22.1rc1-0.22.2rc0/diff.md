# Comparing `tmp/determined_deploy-0.22.1rc1-py3-none-any.whl.zip` & `tmp/determined_deploy-0.22.2rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1815 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-May-17 18:35 determined_deploy/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-May-17 18:35 determined_deploy/__version__.py
--rw-r--r--  2.0 unx      417 b- defN 23-May-17 18:35 determined_deploy-0.22.1rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 18:35 determined_deploy-0.22.1rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-17 18:35 determined_deploy-0.22.1rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-May-17 18:35 determined_deploy-0.22.1rc1.dist-info/RECORD
-6 files, 1314 bytes uncompressed, 847 bytes compressed:  35.5%
+Zip file size: 1813 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      235 b- defN 23-May-17 23:33 determined_deploy/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-May-17 23:33 determined_deploy/__version__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-May-17 23:33 determined_deploy-0.22.2rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 23:33 determined_deploy-0.22.2rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-17 23:33 determined_deploy-0.22.2rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-May-17 23:33 determined_deploy-0.22.2rc0.dist-info/RECORD
+6 files, 1314 bytes uncompressed, 845 bytes compressed:  35.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_deploy/__init__.py
 Comment: 
 
 Filename: determined_deploy/__version__.py
 Comment: 
 
-Filename: determined_deploy-0.22.1rc1.dist-info/METADATA
+Filename: determined_deploy-0.22.2rc0.dist-info/METADATA
 Comment: 
 
-Filename: determined_deploy-0.22.1rc1.dist-info/WHEEL
+Filename: determined_deploy-0.22.2rc0.dist-info/WHEEL
 Comment: 
 
-Filename: determined_deploy-0.22.1rc1.dist-info/top_level.txt
+Filename: determined_deploy-0.22.2rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_deploy-0.22.1rc1.dist-info/RECORD
+Filename: determined_deploy-0.22.2rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_deploy/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.22.1-rc1"
+__version__ = "0.22.2-rc0"
```

