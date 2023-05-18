# Comparing `tmp/imessagedb-1.0.1.tar.gz` & `tmp/imessagedb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.0.1.tar", max compression
+gzip compressed data, was "imessagedb-1.2.0.tar", max compression
```

## Comparing `imessagedb-1.0.1.tar` & `imessagedb-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1070 2023-05-11 14:57:19.657437 imessagedb-1.0.1/LICENSE
--rw-r--r--   0        0        0     8458 2023-05-17 19:52:20.244611 imessagedb-1.0.1/README.md
--rw-r--r--   0        0        0      613 2023-05-17 21:03:03.364829 imessagedb-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10022 2023-05-17 18:29:02.215520 imessagedb-1.0.1/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-17 17:24:37.620303 imessagedb-1.0.1/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8456 2023-05-16 02:23:28.247675 imessagedb-1.0.1/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3049 2023-05-16 02:08:18.779667 imessagedb-1.0.1/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-16 02:10:14.635038 imessagedb-1.0.1/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2443 2023-05-16 02:10:26.298470 imessagedb-1.0.1/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-17 20:18:21.035523 imessagedb-1.0.1/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-11 14:57:19.757639 imessagedb-1.0.1/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-16 02:10:41.131442 imessagedb-1.0.1/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-16 02:12:14.545279 imessagedb-1.0.1/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23073 2023-05-17 17:46:25.080601 imessagedb-1.0.1/src/imessagedb/html.py
--rw-r--r--   0        0        0     5138 2023-05-17 16:50:30.769562 imessagedb-1.0.1/src/imessagedb/message.py
--rw-r--r--   0        0        0     5359 2023-05-17 16:50:30.771703 imessagedb-1.0.1/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-16 02:13:57.551857 imessagedb-1.0.1/src/imessagedb/text.py
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-11 14:57:19.657437 imessagedb-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8458 2023-05-17 19:52:20.244611 imessagedb-1.2.0/README.md
+-rw-r--r--   0        0        0     1256 2023-05-18 00:25:26.525914 imessagedb-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10022 2023-05-17 18:29:02.215520 imessagedb-1.2.0/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-17 17:24:37.620303 imessagedb-1.2.0/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8456 2023-05-16 02:23:28.247675 imessagedb-1.2.0/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3049 2023-05-16 02:08:18.779667 imessagedb-1.2.0/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2133 2023-05-16 02:10:14.635038 imessagedb-1.2.0/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     2510 2023-05-17 21:45:47.568234 imessagedb-1.2.0/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3301 2023-05-17 20:18:21.035523 imessagedb-1.2.0/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-11 14:57:19.757639 imessagedb-1.2.0/src/imessagedb/default.ini
+-rw-r--r--   0        0        0      985 2023-05-16 02:10:41.131442 imessagedb-1.2.0/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     1640 2023-05-16 02:12:14.545279 imessagedb-1.2.0/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    23073 2023-05-17 17:46:25.080601 imessagedb-1.2.0/src/imessagedb/html.py
+-rw-r--r--   0        0        0     5138 2023-05-17 16:50:30.769562 imessagedb-1.2.0/src/imessagedb/message.py
+-rw-r--r--   0        0        0     5359 2023-05-17 16:50:30.771703 imessagedb-1.2.0/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     4182 2023-05-16 02:13:57.551857 imessagedb-1.2.0/src/imessagedb/text.py
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.0/PKG-INFO
```

### Comparing `imessagedb-1.0.1/LICENSE` & `imessagedb-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/README.md` & `imessagedb-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/__init__.py` & `imessagedb-1.2.0/src/imessagedb/__init__.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/attachment.py` & `imessagedb-1.2.0/src/imessagedb/attachment.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/attachments.py` & `imessagedb-1.2.0/src/imessagedb/attachments.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/chat.py` & `imessagedb-1.2.0/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/chats.py` & `imessagedb-1.2.0/src/imessagedb/chats.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
     def __repr__(self) -> str:
         string_array = []
         for i in sorted(self.chat_list):
             string_array.append(str(self.chat_list[i]))
         return '\n'.join(string_array)
 
+    def __len__(self) -> int:
+        return len(self._chat_list)
+
     def _get_chats(self):
         self._database.connection.execute('select rowid, chat_identifier, display_name from chat')
         rows = self._database.connection.fetchall()
         for row in rows:
             rowid = row[0]
             chat_identifier = row[1]
             display_name = row[2]
```

### Comparing `imessagedb-1.0.1/src/imessagedb/db.py` & `imessagedb-1.2.0/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/default.ini` & `imessagedb-1.2.0/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/handle.py` & `imessagedb-1.2.0/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/handles.py` & `imessagedb-1.2.0/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/html.py` & `imessagedb-1.2.0/src/imessagedb/html.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/message.py` & `imessagedb-1.2.0/src/imessagedb/message.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/messages.py` & `imessagedb-1.2.0/src/imessagedb/messages.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/src/imessagedb/text.py` & `imessagedb-1.2.0/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.0.1/PKG-INFO` & `imessagedb-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.0.1
+Version: 1.2.0
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

