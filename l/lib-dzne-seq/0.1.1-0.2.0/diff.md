# Comparing `tmp/lib-dzne-seq-0.1.1.tar.gz` & `tmp/lib-dzne-seq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-seq-0.1.1.tar", last modified: Tue Feb 28 21:18:20 2023, max compression
+gzip compressed data, was "lib-dzne-seq-0.2.0.tar", last modified: Thu May 18 18:14:56 2023, max compression
```

## Comparing `lib-dzne-seq-0.1.1.tar` & `lib-dzne-seq-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-28 21:18:20.737318 lib-dzne-seq-0.1.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-seq-0.1.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-02-28 21:18:20.737318 lib-dzne-seq-0.1.1/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      556 2023-02-28 21:17:36.000000 lib-dzne-seq-0.1.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-02-28 21:18:20.737318 lib-dzne-seq-0.1.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-28 21:18:20.737318 lib-dzne-seq-0.1.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-28 21:18:20.737318 lib-dzne-seq-0.1.1/src/lib_dzne_seq/
--rw-r--r--   0 base      (1001) base      (1001)     2346 2023-02-28 21:14:49.000000 lib-dzne-seq-0.1.1/src/lib_dzne_seq/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-28 21:18:20.737318 lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-02-28 21:18:20.000000 lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      260 2023-02-28 21:18:20.000000 lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-02-28 21:18:20.000000 lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       32 2023-02-28 21:18:20.000000 lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       13 2023-02-28 21:18:20.000000 lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-seq-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      556 2023-05-18 17:21:53.000000 lib-dzne-seq-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/src/lib_dzne_seq/
+-rw-rw-r--   0 base      (1001) base      (1001)     4030 2023-05-18 18:09:49.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      260 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       32 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       13 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/top_level.txt
```

### Comparing `lib-dzne-seq-0.1.1/LICENSE` & `lib-dzne-seq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-seq-0.1.1/PKG-INFO` & `lib-dzne-seq-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-seq
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for handling genetic sequences. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-seq-0.1.1/pyproject.toml` & `lib-dzne-seq-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-seq"
-version = "0.1.1"
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
     'Bio>=1.5.3',
-    'lib_dzne_data>=0.1.0',
+    'lib-dzne-data>=0.1.2',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-seq-0.1.1/src/lib_dzne_seq.egg-info/PKG-INFO` & `lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-seq
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for handling genetic sequences. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

