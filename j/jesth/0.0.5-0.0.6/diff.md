# Comparing `tmp/jesth-0.0.5.tar.gz` & `tmp/jesth-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jesth-0.0.5.tar", last modified: Thu Sep 15 22:04:35 2022, max compression
+gzip compressed data, was "dist/jesth-0.0.6.tar", last modified: Sat Feb 25 01:39:20 2023, max compression
```

## Comparing `jesth-0.0.5.tar` & `jesth-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.922397 jesth-0.0.5/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1076 2022-05-20 19:25:11.000000 jesth-0.0.5/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       67 2022-05-20 19:23:56.000000 jesth-0.0.5/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)     6898 2022-09-15 22:04:35.922397 jesth-0.0.5/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)     6309 2022-09-08 11:27:40.000000 jesth-0.0.5/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2022-09-08 11:28:14.000000 jesth-0.0.5/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.814478 jesth-0.0.5/jesth/
--rw-rw-r--   0 alex      (1002) alex      (1003)      231 2022-06-22 20:31:27.000000 jesth-0.0.5/jesth/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      140 2022-05-21 09:50:04.000000 jesth-0.0.5/jesth/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.862442 jesth-0.0.5/jesth/error/
--rw-rw-r--   0 alex      (1002) alex      (1003)       96 2022-06-22 20:31:27.000000 jesth-0.0.5/jesth/error/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.862442 jesth-0.0.5/jesth/parser/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-21 09:50:15.000000 jesth-0.0.5/jesth/parser/.private
--rw-rw-r--   0 alex      (1002) alex      (1003)     3634 2022-09-05 15:25:00.000000 jesth-0.0.5/jesth/parser/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.882427 jesth-0.0.5/jesth/renderer/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-21 09:50:15.000000 jesth-0.0.5/jesth/renderer/.private
--rw-rw-r--   0 alex      (1002) alex      (1003)     1984 2022-09-05 15:25:00.000000 jesth-0.0.5/jesth/renderer/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.906409 jesth-0.0.5/jesth/util/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-21 09:50:15.000000 jesth-0.0.5/jesth/util/.private
--rw-rw-r--   0 alex      (1002) alex      (1003)      864 2022-06-21 07:01:00.000000 jesth-0.0.5/jesth/util/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.858445 jesth-0.0.5/jesth.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)     6898 2022-09-15 22:04:35.000000 jesth-0.0.5/jesth.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      466 2022-09-15 22:04:35.000000 jesth-0.0.5/jesth.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-09-15 22:04:35.000000 jesth-0.0.5/jesth.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       47 2022-09-15 22:04:35.000000 jesth-0.0.5/jesth.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-05-20 19:25:34.000000 jesth-0.0.5/jesth.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       12 2022-09-15 22:04:35.000000 jesth-0.0.5/jesth.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.5/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      765 2022-09-15 22:04:35.926394 jesth-0.0.5/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.5/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-09-15 22:04:35.922397 jesth-0.0.5/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-20 19:23:56.000000 jesth-0.0.5/tests/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.240203 jesth-0.0.6/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:42:40.000000 jesth-0.0.6/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       67 2022-05-20 19:23:56.000000 jesth-0.0.6/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)     6898 2023-02-25 01:39:20.240203 jesth-0.0.6/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)     6309 2022-09-08 11:27:40.000000 jesth-0.0.6/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2022-09-15 22:04:36.000000 jesth-0.0.6/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.088263 jesth-0.0.6/jesth/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      231 2022-06-22 20:31:27.000000 jesth-0.0.6/jesth/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      140 2022-05-21 09:50:04.000000 jesth-0.0.6/jesth/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.164233 jesth-0.0.6/jesth/error/
+-rw-rw-r--   0 alex      (1002) alex      (1003)       96 2022-06-22 20:31:27.000000 jesth-0.0.6/jesth/error/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.200219 jesth-0.0.6/jesth/parser/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-21 09:50:15.000000 jesth-0.0.6/jesth/parser/.private
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3639 2023-02-12 19:03:12.000000 jesth-0.0.6/jesth/parser/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.200219 jesth-0.0.6/jesth/renderer/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-21 09:50:15.000000 jesth-0.0.6/jesth/renderer/.private
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2025 2023-02-21 09:28:14.000000 jesth-0.0.6/jesth/renderer/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.204217 jesth-0.0.6/jesth/util/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-21 09:50:15.000000 jesth-0.0.6/jesth/util/.private
+-rw-rw-r--   0 alex      (1002) alex      (1003)      864 2022-06-21 07:01:00.000000 jesth-0.0.6/jesth/util/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.164233 jesth-0.0.6/jesth.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     6898 2023-02-25 01:39:19.000000 jesth-0.0.6/jesth.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      466 2023-02-25 01:39:20.000000 jesth-0.0.6/jesth.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-02-25 01:39:19.000000 jesth-0.0.6/jesth.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       47 2023-02-25 01:39:19.000000 jesth-0.0.6/jesth.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-05-20 19:25:34.000000 jesth-0.0.6/jesth.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       12 2023-02-25 01:39:19.000000 jesth-0.0.6/jesth.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.6/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      765 2023-02-25 01:39:20.244201 jesth-0.0.6/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:23:56.000000 jesth-0.0.6/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 01:39:20.240203 jesth-0.0.6/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-05-20 19:23:56.000000 jesth-0.0.6/tests/__init__.py
```

### Comparing `jesth-0.0.5/LICENSE` & `jesth-0.0.6/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Pyrustic Evangelist
+Copyright (c) 2022, 2023 Pyrustic Evangelist
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jesth-0.0.5/PKG-INFO` & `jesth-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jesth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Just Extract Sections Then Hack
 Home-page: https://github.com/pyrustic/jesth
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
```

### Comparing `jesth-0.0.5/README.md` & `jesth-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jesth-0.0.5/jesth/parser/__init__.py` & `jesth-0.0.6/jesth/parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     [return]
     Returns a Jesth structure. A Jesth structure is a dict.
     Each key represents a section title.
     The value of a key is the body of the section.
     The body is a list of string, each string represents a line of text without the newline at end.
     """
     if isinstance(source, pathlib.Path):
-        source = source.resolve()
+        source = str(source.resolve())
     if not os.path.isfile(source):
         return OrderedDict()
     parser = Parser(compact=compact, split_body=split_body)
     with open(source, "r") as file:
         while True:
             line = file.readline()
             if not line:
```

### Comparing `jesth-0.0.5/jesth/renderer/__init__.py` & `jesth-0.0.6/jesth/renderer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     except Exception as e:
         raise error.StructureError from None
     return data
 
 
 def write(structure, destination):
     """
-    Convert a Jesth structure into plain text then save it in a file
+    Convert a Jesth structure into plain text then save it in a file (the parent directory should exist)
 
     [parameters]
     - structure: dict, Jesth structure. Each key represents a section title.
     The value of a key is the body of the section.
     The body is either a string (with newlines or none), or a list of strings
     - destination: str, the path (or a pathlib.Path instance) to a file in which
      the rendered Jesth text can be saved.
@@ -39,15 +39,15 @@
     - jesth.error.StructureError: raised if the structure isn't valid
 
     [return]
     Return the rendered plain text
     """
     data = render(structure)
     if isinstance(destination, pathlib.Path):
-        destination = destination.resolve()
+        destination = str(destination.resolve())
     with open(destination, "w") as file:
         file.write(data)
     return data
 
 
 def _render(structure):
     text = []
```

### Comparing `jesth-0.0.5/jesth/util/__init__.py` & `jesth-0.0.6/jesth/util/__init__.py`

 * *Files identical despite different names*

### Comparing `jesth-0.0.5/jesth.egg-info/PKG-INFO` & `jesth-0.0.6/jesth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jesth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Just Extract Sections Then Hack
 Home-page: https://github.com/pyrustic/jesth
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
```

### Comparing `jesth-0.0.5/setup.cfg` & `jesth-0.0.6/setup.cfg`

 * *Files identical despite different names*

