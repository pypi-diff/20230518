# Comparing `tmp/imessagedb-1.2.6.tar.gz` & `tmp/imessagedb-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.2.6.tar", max compression
+gzip compressed data, was "imessagedb-1.2.7.tar", max compression
```

## Comparing `imessagedb-1.2.6.tar` & `imessagedb-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1070 2023-05-18 01:55:28.519982 imessagedb-1.2.6/LICENSE
--rw-r--r--   0        0        0     8458 2023-05-18 01:55:28.519982 imessagedb-1.2.6/README.md
--rw-r--r--   0        0        0     1309 2023-05-18 01:56:15.252258 imessagedb-1.2.6/pyproject.toml
--rw-r--r--   0        0        0    10222 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8456 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3049 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2510 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23073 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/html.py
--rw-r--r--   0        0        0     5138 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/message.py
--rw-r--r--   0        0        0     5359 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-18 01:55:28.527982 imessagedb-1.2.6/src/imessagedb/text.py
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-18 02:04:41.005016 imessagedb-1.2.7/LICENSE
+-rw-r--r--   0        0        0     8458 2023-05-18 02:04:41.005016 imessagedb-1.2.7/README.md
+-rw-r--r--   0        0        0     1309 2023-05-18 02:05:16.137377 imessagedb-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     9342 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8456 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3049 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2133 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     2510 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3301 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/default.ini
+-rw-r--r--   0        0        0      985 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     1640 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    23073 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5138 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/message.py
+-rw-r--r--   0        0        0     5359 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     4182 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/text.py
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.7/PKG-INFO
```

### Comparing `imessagedb-1.2.6/LICENSE` & `imessagedb-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/README.md` & `imessagedb-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/pyproject.toml` & `imessagedb-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.2.6"
+version = "1.2.7"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.2.6/src/imessagedb/__init__.py` & `imessagedb-1.2.7/src/imessagedb/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -96,36 +96,18 @@
 
 [CONTACTS]
 
 # A person that you text with can have multiple numbers, and you may not always want to specify the full specific
 #  number as stored in the handle database, so you can do the mapping here, providing the name of a person,
 #  and a comma separated list of numbers
 
-Ashley: +18484676050, ashleywilliams_@live.com, sparkette325@yahoo.com, +17325722108,
-   williaa2@kean.edu
+Samantha: +18434676040, samanthasmilt@gmail.com, 
+   s12ddd2@colt.edu
 Abe: +16103499696
-Alisha: +15082088327
-Emily: +12672803303
-Hermosa: +17329103453
-Kanani: +17325351530
-Randi: +16093394399
-Rose: fhecla@gmail.com, +16109602522
-Marta: +19172974204
-Maxine: mlee99@optonline.net, panda9966@gmail.com, +19084725929, +17323816580
-Monika: +19176678993, mnowak2@binghamton.edu, Xplsumnerx@gmail.com
-Michele: +12153917169
-Marissa: +14016490739
-Lily: lilyyalexb@gmail.com, njlibrn@yahoo.com, +17327887245
-Daniel: daniel@gittler.com, +17326460220, dsg1002@gmail.com, gittlerd@gmail.com, dgittler@berklee.edu
-Kandela: +17324849684
-Tiffany: Wickedblueglow@gmail.com, Tlgreenberg80@gmail.com, +17327105145
-Jessica: jessica.marozine@icloud.com, jessica.marozine@gmail.com, +17326923688
-Becky: rebecca@schore.org, +17329838356
-Lynda: lylasmith559@yahoo.com, lylalombardi@icloud.com, +17323001586
-Stefanie: stefanie.thomas2@gmail.com, thostefa@kean.edu, +17326101065
+Marissa: +14029490739
 '''
 
 
 def _create_default_configuration(filename: str) -> None:
     """Generates a default configuration if one is not passed in
 
     """
```

### Comparing `imessagedb-1.2.6/src/imessagedb/attachment.py` & `imessagedb-1.2.7/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/attachments.py` & `imessagedb-1.2.7/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/chat.py` & `imessagedb-1.2.7/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/chats.py` & `imessagedb-1.2.7/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/db.py` & `imessagedb-1.2.7/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/default.ini` & `imessagedb-1.2.7/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/handle.py` & `imessagedb-1.2.7/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/handles.py` & `imessagedb-1.2.7/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/html.py` & `imessagedb-1.2.7/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/message.py` & `imessagedb-1.2.7/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/messages.py` & `imessagedb-1.2.7/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/src/imessagedb/text.py` & `imessagedb-1.2.7/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.6/PKG-INFO` & `imessagedb-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.2.6
+Version: 1.2.7
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

