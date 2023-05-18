# Comparing `tmp/imessagedb-1.2.7.tar.gz` & `tmp/imessagedb-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessagedb-1.2.7.tar", max compression
+gzip compressed data, was "imessagedb-1.2.8.tar", max compression
```

## Comparing `imessagedb-1.2.7.tar` & `imessagedb-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rwxr-xr-x   0        0        0     1070 2023-05-18 02:04:41.005016 imessagedb-1.2.7/LICENSE
--rw-r--r--   0        0        0     8458 2023-05-18 02:04:41.005016 imessagedb-1.2.7/README.md
--rw-r--r--   0        0        0     1309 2023-05-18 02:05:16.137377 imessagedb-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     9342 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/__main__.py
--rw-r--r--   0        0        0     8456 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/attachment.py
--rw-r--r--   0        0        0     3049 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/attachments.py
--rw-r--r--   0        0        0     2133 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/chat.py
--rw-r--r--   0        0        0     2510 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/chats.py
--rw-r--r--   0        0        0     3301 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/db.py
--rw-r--r--   0        0        0     3357 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/default.ini
--rw-r--r--   0        0        0      985 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/handle.py
--rw-r--r--   0        0        0     1640 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/handles.py
--rw-r--r--   0        0        0    23073 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/html.py
--rw-r--r--   0        0        0     5138 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/message.py
--rw-r--r--   0        0        0     5359 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/messages.py
--rw-r--r--   0        0        0     4182 2023-05-18 02:04:41.013016 imessagedb-1.2.7/src/imessagedb/text.py
--rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-18 02:57:53.956294 imessagedb-1.2.8/LICENSE
+-rw-r--r--   0        0        0     8458 2023-05-18 02:57:53.956294 imessagedb-1.2.8/README.md
+-rw-r--r--   0        0        0     1309 2023-05-18 02:58:25.356546 imessagedb-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     9342 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/__main__.py
+-rw-r--r--   0        0        0     8476 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/attachment.py
+-rw-r--r--   0        0        0     3055 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/attachments.py
+-rw-r--r--   0        0        0     2133 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/chat.py
+-rw-r--r--   0        0        0     2518 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/chats.py
+-rw-r--r--   0        0        0     3301 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/db.py
+-rw-r--r--   0        0        0     3357 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/default.ini
+-rw-r--r--   0        0        0      985 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/handle.py
+-rw-r--r--   0        0        0     1640 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/handles.py
+-rw-r--r--   0        0        0    23179 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/html.py
+-rw-r--r--   0        0        0     4975 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/message.py
+-rw-r--r--   0        0        0     4896 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/messages.py
+-rw-r--r--   0        0        0     4182 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/text.py
+-rw-r--r--   0        0        0      538 2023-05-18 02:57:53.960294 imessagedb-1.2.8/src/imessagedb/utils.py
+-rw-r--r--   0        0        0     9164 1970-01-01 00:00:00.000000 imessagedb-1.2.8/PKG-INFO
```

### Comparing `imessagedb-1.2.7/LICENSE` & `imessagedb-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/README.md` & `imessagedb-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/pyproject.toml` & `imessagedb-1.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imessagedb"
-version = "1.2.7"
+version = "1.2.8"
 description = "Reads and displays the Apple iMessage database"
 authors = ["xev <git@schore.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imessagedb-1.2.7/src/imessagedb/__init__.py` & `imessagedb-1.2.8/src/imessagedb/__init__.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/src/imessagedb/attachment.py` & `imessagedb-1.2.8/src/imessagedb/attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             except Exception as exp:
                 print(f"Failed to copy {self._destination_filename}: {exp}")
                 return
         else:
             # If the file already exists, do nothing
             return
 
-    def convert_heic_image(self, heic_location, png_location) -> None:
+    def convert_heic_image(self, heic_location: str, png_location: str) -> None:
         """ Convert a HEIC image to a PNG so it can be viewed in the browser """
         # Don't do the expensive conversion if we've already converted it
         if self._force or not os.path.exists(png_location):
             try:
                 print(f"Converting {os.path.basename(png_location)}")
                 heic_image = heic2png.HEIC2PNG(heic_location)
                 heic_image.save(png_location)
@@ -199,15 +199,15 @@
             except Exception as exp:
                 print(f'Failed to convert {heic_location} to {png_location}: {exp}')
                 return
         else:
             # If the file exists already, don't convert it
             return
 
-    def convert_audio_video(self, original, converted) -> None:
+    def convert_audio_video(self, original: str, converted: str) -> None:
         """ Convert an audio or video file from an undisplayable source to something the browser can display"""
         if self._force or not os.path.exists(converted):
             try:
                 print(f"Converting {os.path.basename(converted)}")
                 stream = ffmpeg.input(original)
                 stream = ffmpeg.output(stream, converted)
                 stream = ffmpeg.overwrite_output(stream)
```

### Comparing `imessagedb-1.2.7/src/imessagedb/attachments.py` & `imessagedb-1.2.8/src/imessagedb/attachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 self.message_join[message_id] = [attachment_id]
             i = self._database.connection.fetchone()
 
         return
 
     @property
     def attachment_list(self) -> dict:
-        """ Return the list of all attachments """
+        """ Return the dictionary of all attachments """
         return self._attachment_list
 
     @property
     def message_join(self) -> dict:
         """ Return the mapping of messages to attachments """
         return self._message_join
```

### Comparing `imessagedb-1.2.7/src/imessagedb/chat.py` & `imessagedb-1.2.8/src/imessagedb/chat.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/src/imessagedb/chats.py` & `imessagedb-1.2.8/src/imessagedb/chats.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         for i in sorted(self.chat_list):
             string_array.append(str(self.chat_list[i]))
         return '\n'.join(string_array)
 
     def __len__(self) -> int:
         return len(self._chat_list)
 
-    def _get_chats(self):
+    def _get_chats(self) -> None:
         self._database.connection.execute('select rowid, chat_identifier, display_name from chat')
         rows = self._database.connection.fetchall()
         for row in rows:
             rowid = row[0]
             chat_identifier = row[1]
             display_name = row[2]
             new_chat = Chat(self._database, rowid, chat_identifier, display_name)
```

### Comparing `imessagedb-1.2.7/src/imessagedb/db.py` & `imessagedb-1.2.8/src/imessagedb/db.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/src/imessagedb/default.ini` & `imessagedb-1.2.8/src/imessagedb/default.ini`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/src/imessagedb/handle.py` & `imessagedb-1.2.8/src/imessagedb/handle.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/src/imessagedb/handles.py` & `imessagedb-1.2.8/src/imessagedb/handles.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/src/imessagedb/html.py` & `imessagedb-1.2.8/src/imessagedb/html.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 from datetime import datetime
 import re
+import imessagedb
+from imessagedb.message import Message
+from imessagedb.messages import Messages
 from alive_progress import alive_bar
 
 
-def _generate_thread_row(message):
+def _generate_thread_row(message: Message) -> str:
     if message.is_from_me:
         style = 'me'
     else:
         style = 'them'
 
     text = message.text
-    # row_string = f'    <tr><td class="blank></td><td class="reply_text_{style}" > {text} </td ></tr>\n'
     row_string = f'{" ":16s}<tr>\n' \
                  f'{" ":18s}<td class="reply_text_thread">\n' \
                  f'{" ":20s}<a href="#{message.rowid}">\n' \
                  f'{" ":22s}<button class="reply_text_{style}"> {text}</button>\n' \
                  f'{" ":20s}</a>\n' \
                  f'{" ":18s}</td>\n' \
                  f'{" ":16s}</tr>\n'
     return row_string
 
 
-def _generate_thread_table(message_list, style):
+def _generate_thread_table(message_list: list, style: str) -> str:
     table_string = f'{" ":14s}<table class="thread_table_{style}">\n'
     for message in message_list:
         table_string = f'{table_string}{_generate_thread_row(message)}'
     table_string = f'{table_string}' \
                    f'{" ":14s}</table>\n' \
                    f'{" ":14s}<p>\n'
     return table_string
 
 
-def _replace_url_to_link(value):
+url_pattern = re.compile(r"((https?):((//)|(\\\\))+[\w\d:#@%/;$()~_?\+-=\\\.&]*)", re.MULTILINE | re.UNICODE)
+mailto_pattern = re.compile(r"([\w\-\.]+@(\w[\w\-]+\.)+[\w\-]+)", re.MULTILINE | re.UNICODE)
+
+
+def _replace_url_to_link(value: str) -> str:
     """ From https://gist.github.com/guillaumepiot/4539986 """
 
     # Replace url to link
-    urls = re.compile(r"((https?):((//)|(\\\\))+[\w\d:#@%/;$()~_?\+-=\\\.&]*)", re.MULTILINE | re.UNICODE)
-    value = urls.sub(r'<a href="\1" target="_blank">\1</a>', value)
+    value = url_pattern.sub(r'<a href="\1" target="_blank">\1</a>', value)
     # Replace email to mailto
-    urls = re.compile(r"([\w\-\.]+@(\w[\w\-]+\.)+[\w\-]+)", re.MULTILINE | re.UNICODE)
-    value = urls.sub(r'<a href="mailto:\1">\1</a>', value)
+    value = mailto_pattern.sub(r'<a href="mailto:\1">\1</a>', value)
     return value
 
 
 class HTMLOutput:
     """ Creates an HTML file (or string) from a Messages list
 
     ...
@@ -83,15 +87,15 @@
 
     me html name color = Blue
     them html name color = Purple :
                 The color of the name
 
     """
 
-    def __init__(self, database, me: str, person: str, message_list,
+    def __init__(self, database, me: str, person: str, message_list: Messages,
                  inline=False, output_file=None) -> None:
         """
             Parameters
             ----------
             database : imessagedb.DB
                 An instance of a connected database
 
@@ -155,15 +159,15 @@
 
     def _print_and_save(self, message: str, array: list) -> None:
         """ Save to the output file while it is processing """
         array.append(message)
         if self._output_file:
             print(message, end="", file=self._output_file)
 
-    def _generate_table(self, message_list) -> str:
+    def _generate_table(self, message_list: Messages) -> str:
         table_array = []
         self._print_and_save(f'{" ":2s}<table class="main_table">\n', table_array)
 
         previous_day = ''
 
         message_count = 0
         with alive_bar(len(message_list), title="Generating HTML", stats="({rate}, eta: {eta})") as bar:
@@ -185,15 +189,15 @@
                     bar()
                 else:
                     bar(skipped=True)
 
         self._print_and_save(f'{" ":2s}</table>\n', table_array)
         return ''.join(table_array)
 
-    def _generate_row(self, message) -> str:
+    def _generate_row(self, message: Message) -> str:
         # Specify if the message is from me, or the other person
         if message.is_from_me:
             who = self._me
             style = 'me'
         else:
             who = self._person
             style = 'them'
@@ -213,15 +217,15 @@
                 # sort the threads by the date sent
                 for i in sorted(thread_list.values(), key=lambda x: x.date):
                     if i == message: # stop at the current message
                         break
                     print_thread.append(i)
                 thread_table = _generate_thread_table(print_thread, style)
 
-        # Generate the attatchment string
+        # Generate the attachment string
         attachments_string = ""
         if message.attachments:
             for attachment_key in message.attachments:
                 if attachment_key not in self._attachment_list.attachment_list:
                     attachments_string = f'{attachments_string} <span class="missing"> Attachment missing </span> '
                     continue
 
@@ -301,15 +305,15 @@
         edited_string = ""
         edit_table = ""
         text_cell_edit_row = ""
 
         if len(message.edits) > 0:
             edit_table = f'{" ":14s}<div class="edits_{style}">\n'
             for i in range(0, len(message.edits)):
-                edit_table = f'{edit_table}{" ":16s}"{message.edits[i]} <p>\n'
+                edit_table = f'{edit_table}{" ":16s}"{message.edits[i]["text"]} <p>\n'
             edit_table = f'{edit_table}{" ":14s}</div>\n'
             edited_string = f'<sub><button class="edited_button"' \
                             f' onclick="ToggleDisplay(\'{message.rowid}editTable\')"> Edited </button></sub>'
             text_cell_edit_row = f'{" ":10s}<tr id={message.rowid}editTable class="edits">\n' \
                                  f'{" ":12s}<td>\n' \
                                  f'{edit_table} ' \
                                  f'{" ":12s}</td>\n ' \
@@ -547,23 +551,23 @@
     border-radius: 6px;
     border-radius: 50px;
     font-size: 60%
 ''' + ''' }
 
 .reply_text_me {''' + f'''
     border: 2px solid;
-    background: {me_html_background_color};
+    background: {me_thread_background_color};
     border-radius: 6px;
     border-radius: 50px;
     font-size: 60%
 ''' + ''' }
 
 .reply_text_them {''' + f'''
     border: 2px solid;
-    background: {them_html_background_color};
+    background: {them_thread_background_color};
     border-radius: 6px;
     border-radius: 50px;
     font-size: 60%
 ''' + ''' }
 
 td.blank {''' + f'''
     border: none;
```

### Comparing `imessagedb-1.2.7/src/imessagedb/message.py` & `imessagedb-1.2.8/src/imessagedb/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import plistlib
-import datetime
+from datetime import datetime
 
-from . import attachments
+from imessagedb.utils import *
 import imessagedb
 
 
-def _date_from_webkit(webkit_timestamp: float) -> datetime.datetime:
-    # From https://www.epochconverter.com/webkit
-    epoch_start = datetime.datetime(1601,1,1)
-    delta = datetime.timedelta(microseconds=int(webkit_timestamp*1000000))
-    return epoch_start + delta
-
-
 def _convert_attributed_body(encoded: bytes) -> str:
     # This general logic was copied from
     # https://github.com/my-other-github-account/imessage_tools/blob/master/imessage_tools.py, however
     # I needed to make some improvements
 
     text = encoded.split(b'NSNumber')[0]
     text = text.split(b'NSString')[1]
@@ -29,16 +22,17 @@
         text = text.split(b'\x86')[0]
     return text.decode('utf-8', errors='replace')
 
 
 class Message:
     """ Class for holding information about a message """
 
-    def __init__(self, database, rowid, guid, date, is_from_me, handle_id, attributed_body, message_summary_info, text,
-                 reply_to_guid, thread_originator_guid, thread_originator_part, chat_id, message_attachments):
+    def __init__(self, database, rowid: int, guid: str, date: str, is_from_me: bool, handle_id: int,
+                 attributed_body: bytes, message_summary_info: bytes, text: str, reply_to_guid: str,
+                 thread_originator_guid: str, thread_originator_part: str, chat_id: int, message_attachments: list):
         """
                 Parameters
                 ----------
                 database : imessagedb.DB
                     An instance of a connected database
 
                 rowid, guid, date, is_from_me, handle_id, attributed_body, message_summary_info, text,
@@ -73,16 +67,16 @@
             self._text = _convert_attributed_body(self._attributed_body)
 
         # Edits are stored in message_summary_info
         try:
             plist = plistlib.loads(self._message_summary_info)
             if 'ec' in plist:
                 for row in plist['ec']['0']:
-                    self._edits.append(_convert_attributed_body(row['t']))
-                    # row['d'] = _date_from_webkit(row['d'])
+                    self._edits.append({'text': _convert_attributed_body(row['t']),
+                                        'date': convert_from_database_date(row['d'])})
         except plistlib.InvalidFileException as exp:
             pass
 
     def __repr__(self) -> str:
         return_string = f'RowID: {self._rowid}' \
                         f' GUID: {self._guid}' \
                         f' Date: {self._date}' \
@@ -93,23 +87,23 @@
                         f' Reply Message: {self._reply_to_guid}' \
                         f' Thread Part: {self._thread_originator_part}' \
                         f' Chat ID: {self._chat_id}' \
                         f' Attachments: {self._attachments}'
         return str(return_string)
 
     @property
-    def rowid(self) -> str:
+    def rowid(self) -> int:
         return self._rowid
 
     @property
     def guid(self) -> str:
         return self._guid
 
     @property
-    def date(self) -> datetime.datetime:
+    def date(self) -> str:
         return self._date
 
     @property
     def is_from_me(self) -> bool:
         return self._is_from_me
 
     @property
@@ -141,13 +135,13 @@
         return self._thread_originator_guid
 
     @property
     def chat_id(self) -> str:
         return self._chat_id
 
     @property
-    def attachments(self) -> attachments.Attachments:
+    def attachments(self) -> list:
         return self._attachments
 
     @property
     def thread(self) -> dict:
         return self._thread
```

### Comparing `imessagedb-1.2.7/src/imessagedb/messages.py` & `imessagedb-1.2.8/src/imessagedb/messages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-from datetime import datetime
+from imessagedb.utils import *
 from alive_progress import alive_bar
 from imessagedb.message import Message
 
 
-mac_epoch_start = int(datetime(2001, 1, 1, 0, 0, 0).strftime('%s'))
-
-
-def _convert_to_database_date(date_string):
-    date_ = datetime.strptime(date_string, '%Y-%m-%d %H:%M:%S')
-    epoch_date = int(date_.strftime('%s'))
-    diff = epoch_date - mac_epoch_start
-    return diff * 1000000000
-
-
-def _convert_from_database_date(date_value):
-    date_ = date_value / 1000000000
-    epoch_date = date_ + mac_epoch_start
-    return datetime.fromtimestamp(epoch_date)
-
-
 class Messages:
     """ All messages in a conversation or conversations with a particular person """
     def __init__(self, database, person: str, numbers: list) -> None:
         """
                 Parameters
                 ----------
                 database : imessagedb.DB
@@ -43,18 +27,18 @@
 
         numbers_string = "','".join(self._numbers)
         time_rules = []
         time_where_clause = ""
         start_time = self._database.control.get('start time', fallback=None)
         end_time = self._database.control.get('end time', fallback=None)
         if start_time:
-            database_start_date = _convert_to_database_date(start_time)
+            database_start_date = convert_to_database_date(start_time)
             time_rules.append(f"message.date >= {database_start_date}")
         if end_time:
-            database_end_date = _convert_to_database_date(end_time)
+            database_end_date = convert_to_database_date(end_time)
             time_rules.append(f"message.date <= {database_end_date}")
         if len(time_rules) > 0:
             time_where_clause = f" and {' AND '.join(time_rules)}"
 
         where_clause = "rowid in (" \
                        " select message_id from chat_message_join where chat_id in (" \
                        "  select chat_id from chat_handle_join where handle_id in (" \
```

### Comparing `imessagedb-1.2.7/src/imessagedb/text.py` & `imessagedb-1.2.8/src/imessagedb/text.py`

 * *Files identical despite different names*

### Comparing `imessagedb-1.2.7/PKG-INFO` & `imessagedb-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imessagedb
-Version: 1.2.7
+Version: 1.2.8
 Summary: Reads and displays the Apple iMessage database
 License: MIT
 Author: xev
 Author-email: git@schore.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

