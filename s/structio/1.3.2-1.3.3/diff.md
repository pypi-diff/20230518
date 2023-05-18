# Comparing `tmp/structio-1.3.2.tar.gz` & `tmp/structio-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.3.2.tar", last modified: Thu May 18 02:01:57 2023, max compression
+gzip compressed data, was "structio-1.3.3.tar", last modified: Thu May 18 02:05:00 2023, max compression
```

## Comparing `structio-1.3.2.tar` & `structio-1.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:57.825066 structio-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-18 02:01:57.825066 structio-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 02:01:40.000000 structio-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-18 02:01:40.000000 structio-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:01:57.825066 structio-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:01:57.825066 structio-1.3.2/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-18 02:01:57.000000 structio-1.3.2/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 02:01:57.000000 structio-1.3.2/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:01:57.000000 structio-1.3.2/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 02:01:57.000000 structio-1.3.2/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-18 02:01:40.000000 structio-1.3.2/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:05:00.852738 structio-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-18 02:05:00.852738 structio-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 02:04:43.000000 structio-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-18 02:04:43.000000 structio-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:05:00.852738 structio-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:05:00.852738 structio-1.3.3/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-18 02:04:43.000000 structio-1.3.3/structio.py
```

### Comparing `structio-1.3.2/PKG-INFO` & `structio-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -56,16 +56,14 @@
 
 ### Struct
 
 Contains methods for unpacking and packing various data types.
 
 ### Attributes
 
-**buffer**: the current content of the object.
-
 **endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
 
 **encoding**: specifies the default encoding used by string methods.
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
@@ -142,14 +140,16 @@
 
 ### StructIO
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
+**buffer**: the current content of the object.
+
 **endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
 
 **encoding**: specifies the default encoding used by string methods.
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
```

### Comparing `structio-1.3.2/README.md` & `structio-1.3.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,14 @@
 
 ### Struct
 
 Contains methods for unpacking and packing various data types.
 
 ### Attributes
 
-**buffer**: the current content of the object.
-
 **endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
 
 **encoding**: specifies the default encoding used by string methods.
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
@@ -134,14 +132,16 @@
 
 ### StructIO
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
+**buffer**: the current content of the object.
+
 **endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
 
 **encoding**: specifies the default encoding used by string methods.
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
```

### Comparing `structio-1.3.2/structio.egg-info/PKG-INFO` & `structio-1.3.3/structio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -56,16 +56,14 @@
 
 ### Struct
 
 Contains methods for unpacking and packing various data types.
 
 ### Attributes
 
-**buffer**: the current content of the object.
-
 **endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
 
 **encoding**: specifies the default encoding used by string methods.
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
@@ -142,14 +140,16 @@
 
 ### StructIO
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
+**buffer**: the current content of the object.
+
 **endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
 
 **encoding**: specifies the default encoding used by string methods.
 
 **errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
 
 ### Methods
```

### Comparing `structio-1.3.2/structio.py` & `structio-1.3.3/structio.py`

 * *Files identical despite different names*

