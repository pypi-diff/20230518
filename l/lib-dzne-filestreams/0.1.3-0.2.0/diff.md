# Comparing `tmp/lib-dzne-filestreams-0.1.3.tar.gz` & `tmp/lib-dzne-filestreams-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filestreams-0.1.3.tar", last modified: Sat Mar 18 08:59:24 2023, max compression
+gzip compressed data, was "lib-dzne-filestreams-0.2.0.tar", last modified: Thu May 18 18:19:16 2023, max compression
```

## Comparing `lib-dzne-filestreams-0.1.3.tar` & `lib-dzne-filestreams-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-18 08:59:24.401590 lib-dzne-filestreams-0.1.3/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1489 2023-03-18 08:59:24.401590 lib-dzne-filestreams-0.1.3/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      644 2023-03-18 08:56:25.000000 lib-dzne-filestreams-0.1.3/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-03-18 08:59:24.401590 lib-dzne-filestreams-0.1.3/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-18 08:59:24.401590 lib-dzne-filestreams-0.1.3/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-18 08:59:24.401590 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/
--rw-r--r--   0 base      (1001) base      (1001)      805 2023-03-18 08:27:17.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/BASEStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      763 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/ResourceStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      950 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/SeqreadInStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      652 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/SeqreadOutStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      458 2023-03-01 21:41:51.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/TOMLStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      894 2023-03-18 08:43:57.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/TabStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      757 2023-03-18 08:49:25.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/TextStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      505 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/WorkbookStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      352 2023-03-18 08:46:43.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/_CharsStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)     1678 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/_SeqreadStreamType.py
--rw-r--r--   0 base      (1001) base      (1001)     2331 2023-03-01 21:44:12.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/_StreamType.py
--rw-r--r--   0 base      (1001) base      (1001)      832 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-18 08:59:24.401590 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1489 2023-03-18 08:59:24.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      802 2023-03-18 08:59:24.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-03-18 08:59:24.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       91 2023-03-18 08:59:24.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       21 2023-03-18 08:59:24.000000 lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:19:16.704007 lib-dzne-filestreams-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filestreams-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1489 2023-05-18 18:19:16.704007 lib-dzne-filestreams-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      653 2023-05-18 17:22:13.000000 lib-dzne-filestreams-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-18 18:19:16.704007 lib-dzne-filestreams-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:19:16.704007 lib-dzne-filestreams-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:19:16.704007 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams/
+-rw-r--r--   0 base      (1001) base      (1001)     5327 2023-05-18 18:08:33.000000 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:19:16.704007 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1489 2023-05-18 18:19:16.000000 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      308 2023-05-18 18:19:16.000000 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-18 18:19:16.000000 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)      100 2023-05-18 18:19:16.000000 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       21 2023-05-18 18:19:16.000000 lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/top_level.txt
```

### Comparing `lib-dzne-filestreams-0.1.3/LICENSE` & `lib-dzne-filestreams-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filestreams-0.1.3/PKG-INFO` & `lib-dzne-filestreams-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filestreams
-Version: 0.1.3
+Version: 0.2.0
 Summary: Libary for handling genetic sequences. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filestreams-0.1.3/pyproject.toml` & `lib-dzne-filestreams-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filestreams"
-version = "0.1.3"
+version = "0.2.0"
 description = "Libary for handling genetic sequences. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
-    'Bio>=1.5.3',
     'tomli_w',
     'lib-dzne-basetables>=0.1.2',
     'lib-dzne-tsv>=0.1.4',
     'lib-dzne-workbook>=0.1.3',
+    'lib-dzne-seq>=0.2.0',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-filestreams-0.1.3/src/lib_dzne_filestreams.egg-info/PKG-INFO` & `lib-dzne-filestreams-0.2.0/src/lib_dzne_filestreams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filestreams
-Version: 0.1.3
+Version: 0.2.0
 Summary: Libary for handling genetic sequences. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

