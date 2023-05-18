# Comparing `tmp/pyspeaker-1.1.win-amd64.zip` & `tmp/pyspeaker-1.2.win-amd64.zip`

## zipinfo {}

```diff
@@ -1,16 +1,13 @@
-Zip file size: 4375 bytes, number of entries: 14
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/Python/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/Python/Python311/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/Python/Python311/Lib/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/__pycache__/
--rw-rw-rw-  2.0 fat      776 b- defN 23-May-18 17:15 Programs/Python/Python311/Lib/site-packages/Audio.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat      212 b- defN 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       28 b- defN 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/requires.txt
--rw-rw-rw-  2.0 fat      203 b- defN 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat     1961 b- defN 23-May-18 18:26 Programs/Python/Python311/Lib/site-packages/__pycache__/Audio.cpython-311.pyc
-14 files, 3187 bytes uncompressed, 1653 bytes compressed:  48.1%
+Zip file size: 2428 bytes, number of entries: 11
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:38 Programs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:38 Programs/Python/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:38 Programs/Python/Python311/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:38 Programs/Python/Python311/Lib/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat      212 b- defN 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat       28 b- defN 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat      194 b- defN 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-18 18:38 Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/top_level.txt
+11 files, 436 bytes uncompressed, 304 bytes compressed:  30.3%
```

## zipnote {}

```diff
@@ -9,35 +9,26 @@
 
 Filename: Programs/Python/Python311/Lib/
 Comment: 
 
 Filename: Programs/Python/Python311/Lib/site-packages/
 Comment: 
 
-Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/
+Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/
 Comment: 
 
-Filename: Programs/Python/Python311/Lib/site-packages/__pycache__/
+Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/dependency_links.txt
 Comment: 
 
-Filename: Programs/Python/Python311/Lib/site-packages/Audio.py
+Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/PKG-INFO
 Comment: 
 
-Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/dependency_links.txt
+Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/requires.txt
 Comment: 
 
-Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/PKG-INFO
+Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/SOURCES.txt
 Comment: 
 
-Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/requires.txt
-Comment: 
-
-Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/SOURCES.txt
-Comment: 
-
-Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.1-py3.11.egg-info/top_level.txt
-Comment: 
-
-Filename: Programs/Python/Python311/Lib/site-packages/__pycache__/Audio.cpython-311.pyc
+Filename: Programs/Python/Python311/Lib/site-packages/pyspeaker-1.2-py3.11.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

