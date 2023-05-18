# Comparing `tmp/imessagedb-1.2.4.tar.gz` & `tmp/imessagedb-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.2.4.tar", max compression
+gzip compressed data, was "imessagedb-1.2.5.tar", max compression
```

## Comparing `imessagedb-1.2.4.tar` & `imessagedb-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1070 2023-05-18 01:02:28.976375 imessagedb-1.2.4/LICENSE
--rw-r--r--   0        0        0     8458 2023-05-18 01:02:28.976375 imessagedb-1.2.4/README.md
--rw-r--r--   0        0        0     1256 2023-05-18 01:03:02.332685 imessagedb-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    10022 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8456 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3049 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2510 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23073 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/html.py
--rw-r--r--   0        0        0     5138 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/message.py
--rw-r--r--   0        0        0     5359 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-18 01:02:28.984375 imessagedb-1.2.4/src/imessagedb/text.py
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-18 01:13:42.193124 imessagedb-1.2.5/LICENSE
+-rw-r--r--   0        0        0     8458 2023-05-18 01:13:42.193124 imessagedb-1.2.5/README.md
+-rw-r--r--   0        0        0     1256 2023-05-18 01:14:18.025756 imessagedb-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    10022 2023-05-18 01:13:42.197124 imessagedb-1.2.5/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-18 01:13:42.197124 imessagedb-1.2.5/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8456 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3049 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2133 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     2510 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3301 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/default.ini
+-rw-r--r--   0        0        0      985 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     1640 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    23073 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5138 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/message.py
+-rw-r--r--   0        0        0     5359 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     4182 2023-05-18 01:13:42.201124 imessagedb-1.2.5/src/imessagedb/text.py
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.5/PKG-INFO
```

### Comparing `imessagedb-1.2.4/LICENSE` & `imessagedb-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/README.md` & `imessagedb-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/pyproject.toml` & `imessagedb-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.2.4"
+version = "1.2.5"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.2.4/src/imessagedb/__init__.py` & `imessagedb-1.2.5/src/imessagedb/__init__.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/attachment.py` & `imessagedb-1.2.5/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/attachments.py` & `imessagedb-1.2.5/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/chat.py` & `imessagedb-1.2.5/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/chats.py` & `imessagedb-1.2.5/src/imessagedb/chats.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/db.py` & `imessagedb-1.2.5/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/default.ini` & `imessagedb-1.2.5/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/handle.py` & `imessagedb-1.2.5/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/handles.py` & `imessagedb-1.2.5/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/html.py` & `imessagedb-1.2.5/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/message.py` & `imessagedb-1.2.5/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/messages.py` & `imessagedb-1.2.5/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/src/imessagedb/text.py` & `imessagedb-1.2.5/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.4/PKG-INFO` & `imessagedb-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.2.4
+Version: 1.2.5
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

