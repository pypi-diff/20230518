# Comparing `tmp/pymino-1.1.7.7.tar.gz` & `tmp/pymino-1.1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.5\dist\.tmp-2nezukqd\pymino-1.1.7.7.tar", last modified: Wed May 17 05:06:22 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.5\dist\.tmp-m24dzwfv\pymino-1.1.7.8.tar", last modified: Wed May 17 23:56:22 2023, max compression
```

## Comparing `pymino-1.1.7.7.tar` & `pymino-1.1.7.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 05:06:22.677955 pymino-1.1.7.7/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.7/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-17 05:06:22.678451 pymino-1.1.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 05:06:22.630835 pymino-1.1.7.7/pymino/
--rw-rw-rw-   0        0        0      676 2023-05-17 05:05:47.000000 pymino-1.1.7.7/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.7/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.7/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:06:22.653651 pymino-1.1.7.7/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.7/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.7/pymino/ext/account.py
--rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.7/pymino/ext/community.py
--rw-rw-rw-   0        0        0    44955 2023-05-17 05:05:31.000000 pymino-1.1.7.7/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.7/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:06:22.671010 pymino-1.1.7.7/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.7/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.7/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14506 2023-05-17 03:04:03.000000 pymino-1.1.7.7/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    49421 2023-05-17 03:04:26.000000 pymino-1.1.7.7/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.7/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.7.7/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.7/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.7/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.7.7/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.7.7/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:06:22.675970 pymino-1.1.7.7/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.7/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.7/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.7/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.7/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:06:22.643731 pymino-1.1.7.7/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-17 05:06:22.000000 pymino-1.1.7.7/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-17 05:06:22.000000 pymino-1.1.7.7/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 05:06:22.000000 pymino-1.1.7.7/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-17 05:06:22.000000 pymino-1.1.7.7/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 05:06:22.000000 pymino-1.1.7.7/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-17 05:06:22.680434 pymino-1.1.7.7/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.560728 pymino-1.1.7.8/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.8/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-17 23:56:22.561224 pymino-1.1.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.508648 pymino-1.1.7.8/pymino/
+-rw-rw-rw-   0        0        0      676 2023-05-17 23:32:47.000000 pymino-1.1.7.8/pymino/__init__.py
+-rw-rw-rw-   0        0        0    26133 2023-05-17 23:36:26.000000 pymino-1.1.7.8/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.8/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.537931 pymino-1.1.7.8/pymino/ext/
+-rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.8/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.8/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.8/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    44878 2023-05-17 23:55:35.000000 pymino-1.1.7.8/pymino/ext/context.py
+-rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.8/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.554280 pymino-1.1.7.8/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.8/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.8/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14506 2023-05-17 03:04:03.000000 pymino-1.1.7.8/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    49421 2023-05-17 03:04:26.000000 pymino-1.1.7.8/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     2653 2023-05-17 23:34:15.000000 pymino-1.1.7.8/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.7.8/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.8/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.8/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.7.8/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.7.8/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.559736 pymino-1.1.7.8/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.8/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.8/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.8/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.8/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.526999 pymino-1.1.7.8/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-17 23:56:22.568168 pymino-1.1.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.8/setup.py
```

### Comparing `pymino-1.1.7.7/LICENSE` & `pymino-1.1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/PKG-INFO` & `pymino-1.1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.7
+Version: 1.1.7.8
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.7/README.md` & `pymino-1.1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/__init__.py` & `pymino-1.1.7.8/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.7.7'
+__version__ = '1.1.7.8'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .client import Client as Client
 
 from requests import get
 from colorama import Fore, Style
```

### Comparing `pymino-1.1.7.7/pymino/bot.py` & `pymino-1.1.7.8/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/client.py` & `pymino-1.1.7.8/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/account.py` & `pymino-1.1.7.8/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/community.py` & `pymino-1.1.7.8/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/context.py` & `pymino-1.1.7.8/pymino/ext/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,26 +147,28 @@
             else:
                 ctx.send(content="You have been verified!", delete_after=TIMEOUT)
         ```
         """
         start = time()
         cache = Cache("cache")
         
-        while True:
+        while time() - start < timeout:
             cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
-            if time() - start >= timeout:
-                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
-                return None
-            if cached_message is not None and cached_message != message:
-                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
-                return None
+
             if cached_message == message:
                 cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
                 return self.message
-    
+
+            if all([cached_message is not None, cached_message != message]):
+                cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+                return None
+
+        cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
+        return None
+
     @_run
     def send(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
         `send` - This sends a message.
 
         `**Parameters**``
         - `content` - The message you want to send.
@@ -187,15 +189,15 @@
             extensions = {
             "mentionedArray": [
             {"uid": self.message.author.userId}
             ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
             ] if isinstance(mentioned, list) else None
             })
 
-        Thread(target=self._delete, args=(message, delete_after)) if delete_after else None
+        Thread(target=self._delete, args=(message, delete_after)).start() if delete_after else None
 
         return message
 
     @_run
     def reply(self, content: str, delete_after: int= None, mentioned: Union[str, List[str]]= None) -> CMessage:
         """
         `reply` - This replies to the message.
@@ -220,15 +222,15 @@
             extensions = {
             "mentionedArray": [
             {"uid": self.message.author.userId}
             ] if isinstance(mentioned, str) else [{"uid": i} for i in mentioned
             ] if isinstance(mentioned, list) else None
             })
         
-        Thread(target=self._delete, args=(message, delete_after)) if delete_after else None
+        Thread(target=self._delete, args=(message, delete_after)).start() if delete_after else None
         
         return message
 
     def prepare_mentions(self, mentioned: dict) -> list:
         """
         `prepare_mentions` - This prepares the mentions for the message.
         
@@ -1276,28 +1278,24 @@
         self,
         event: str,
         data: Union[Message, OnlineMembers, NNotification, Context]
         ) -> Union[Context, None]:
         """
         `_handle_event` is a function that handles events.
         """
-        context = self.context(data, self.request)
-
-        if event == "text_message":
-            self._add_cache(data.chatId, data.author.userId, data.content)
-        
-        if event in self._events:
-            self._remove_cache(data.chatId, data.author.userId)
-            if event == "user_online":
-                return self._events[event](data)
-
-            if event in {
-                "member_set_you_host",
-                "member_set_you_cohost",
-                "member_remove_your_cohost",
-            }:
-                return self._events[event](data)
+        with suppress(KeyError):
+            context = self.context(data, self.request)
 
-            return self._events[event](context)
+            if event in self._events:
+                if event in {
+                    "user_online",
+                    "member_set_you_host",
+                    "member_set_you_cohost",
+                    "member_remove_your_cohost",
+                }:
+                    return self._events[event](data)
+                else:
+                    return self._events[event](context)
 
-        with suppress(KeyError):
-            return self._handle_command(data=data, context=context)
+            if event == "text_message":
+                self._add_cache(data.chatId, data.author.userId, data.content)
+                return self._handle_command(data=data, context=context)
```

### Comparing `pymino-1.1.7.7/pymino/ext/dispatcher.py` & `pymino-1.1.7.8/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/enums.py` & `pymino-1.1.7.8/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/exceptions.py` & `pymino-1.1.7.8/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/general.py` & `pymino-1.1.7.8/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/handlers.py` & `pymino-1.1.7.8/pymino/ext/entities/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,19 +58,22 @@
     """Parses the user ID from a session ID."""
     decoded_sid = urlsafe_b64decode(f"{sid}==")
     decoded_json: dict = loads(decoded_sid[1:-20].decode())
     return decoded_json["2"]
 
 def cache_login(email: str, device: str, sid: str):
     """Cache the login credentials for the current user."""
-    cache = Cache("cache")
-    cache[email] = {"device": device, "sid": sid}
+    with suppress(Exception):
+        cache = Cache("cache")
+        cache[email] = {"device": device, "sid": sid}
 
 def fetch_cache(email: str) -> tuple:
     """Fetch the login credentials for the current user."""
-    cache = Cache("cache")
-    return cache[email]["sid"], cache[email]["device"]
+    with suppress(Exception):
+        cache = Cache("cache")
+        return cache[email]["sid"], cache[email]["device"]
 
 def cache_exists(email: str) -> bool:
     """Check if the cache exists for the current user."""
-    cache = Cache("cache")
-    return email in cache
+    with suppress(Exception):
+        cache = Cache("cache")
+        return email in cache
```

### Comparing `pymino-1.1.7.7/pymino/ext/entities/messages.py` & `pymino-1.1.7.8/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/threads.py` & `pymino-1.1.7.8/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/userprofile.py` & `pymino-1.1.7.8/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/entities/wsevents.py` & `pymino-1.1.7.8/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/socket.py` & `pymino-1.1.7.8/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/utilities/commands.py` & `pymino-1.1.7.8/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/utilities/generate.py` & `pymino-1.1.7.8/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino/ext/utilities/request_handler.py` & `pymino-1.1.7.8/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/pymino.egg-info/PKG-INFO` & `pymino-1.1.7.8/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.7
+Version: 1.1.7.8
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.7 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.8 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.7/pymino.egg-info/SOURCES.txt` & `pymino-1.1.7.8/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.7/setup.cfg` & `pymino-1.1.7.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e37 2e37 0d0a 6175  on = 1.1.7.7..au
+00000020: 6f6e 203d 2031 2e31 2e37 2e38 0d0a 6175  on = 1.1.7.8..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.7.7/setup.py` & `pymino-1.1.7.8/setup.py`

 * *Files identical despite different names*

