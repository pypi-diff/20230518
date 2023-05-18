# Comparing `tmp/pymino-1.1.7.8.tar.gz` & `tmp/pymino-1.1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.5\dist\.tmp-m24dzwfv\pymino-1.1.7.8.tar", last modified: Wed May 17 23:56:22 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.5\dist\.tmp-1exk1t1p\pymino-1.1.7.9.tar", last modified: Thu May 18 00:42:46 2023, max compression
```

## Comparing `pymino-1.1.7.8.tar` & `pymino-1.1.7.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.560728 pymino-1.1.7.8/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.8/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-17 23:56:22.561224 pymino-1.1.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.508648 pymino-1.1.7.8/pymino/
--rw-rw-rw-   0        0        0      676 2023-05-17 23:32:47.000000 pymino-1.1.7.8/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-05-17 23:36:26.000000 pymino-1.1.7.8/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.8/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.537931 pymino-1.1.7.8/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.8/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.8/pymino/ext/account.py
--rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.8/pymino/ext/community.py
--rw-rw-rw-   0        0        0    44878 2023-05-17 23:55:35.000000 pymino-1.1.7.8/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.8/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.554280 pymino-1.1.7.8/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.8/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.8/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14506 2023-05-17 03:04:03.000000 pymino-1.1.7.8/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    49421 2023-05-17 03:04:26.000000 pymino-1.1.7.8/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2653 2023-05-17 23:34:15.000000 pymino-1.1.7.8/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.7.8/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.8/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.8/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.7.8/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.7.8/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.559736 pymino-1.1.7.8/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.8/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.8/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.8/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.8/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-17 23:56:22.526999 pymino-1.1.7.8/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 23:56:22.000000 pymino-1.1.7.8/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-17 23:56:22.568168 pymino-1.1.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:42:46.852457 pymino-1.1.7.9/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.9/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-18 00:42:46.852953 pymino-1.1.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 00:42:46.809305 pymino-1.1.7.9/pymino/
+-rw-rw-rw-   0        0        0      676 2023-05-18 00:42:04.000000 pymino-1.1.7.9/pymino/__init__.py
+-rw-rw-rw-   0        0        0    26133 2023-05-17 23:36:26.000000 pymino-1.1.7.9/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.9/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:42:46.834105 pymino-1.1.7.9/pymino/ext/
+-rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.9/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.9/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   271483 2023-05-18 00:27:35.000000 pymino-1.1.7.9/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    45041 2023-05-18 00:39:45.000000 pymino-1.1.7.9/pymino/ext/context.py
+-rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.9/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:42:46.846530 pymino-1.1.7.9/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.9/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.9/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14506 2023-05-17 03:04:03.000000 pymino-1.1.7.9/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    49421 2023-05-17 03:04:26.000000 pymino-1.1.7.9/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     2653 2023-05-17 23:34:15.000000 pymino-1.1.7.9/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.7.9/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.9/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.9/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.7.9/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.7.9/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:42:46.851465 pymino-1.1.7.9/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.9/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.9/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.9/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.9/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-18 00:42:46.826169 pymino-1.1.7.9/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-18 00:42:46.000000 pymino-1.1.7.9/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-18 00:42:46.000000 pymino-1.1.7.9/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 00:42:46.000000 pymino-1.1.7.9/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-18 00:42:46.000000 pymino-1.1.7.9/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 00:42:46.000000 pymino-1.1.7.9/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-18 00:42:46.854937 pymino-1.1.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-05-18 00:06:54.000000 pymino-1.1.7.9/setup.py
```

### Comparing `pymino-1.1.7.8/LICENSE` & `pymino-1.1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/PKG-INFO` & `pymino-1.1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.8
+Version: 1.1.7.9
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.8 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.9 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.8/README.md` & `pymino-1.1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/__init__.py` & `pymino-1.1.7.9/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.7.8'
+__version__ = '1.1.7.9'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .client import Client as Client
 
 from requests import get
 from colorama import Fore, Style
```

### Comparing `pymino-1.1.7.8/pymino/bot.py` & `pymino-1.1.7.9/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/client.py` & `pymino-1.1.7.9/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/account.py` & `pymino-1.1.7.9/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/community.py` & `pymino-1.1.7.9/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -4192,14 +4192,15 @@
         return ApiResponse(self.session.handler(
             method = "POST",
             url = "/g/s/media/upload",
             data = media,
             content_type = content_type
             )).mediaValue
 
+
     @community
     def join_chat(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Joins a chat.
 
         :param chatId: The ID of the chat to join.
         :type chatId: str
@@ -4228,14 +4229,15 @@
         ...     print("Failed to join chat.")
         """
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}"
             ))
 
+
     @community
     def leave_chat(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Leaves a chat.
 
         :param chatId: The ID of the chat to leave.
         :type chatId: str
@@ -4264,14 +4266,15 @@
         ...     print("Failed to leave chat.")
         """
         return ApiResponse(self.session.handler(
             method = "DELETE",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}"
             ))
 
+
     @community
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True, comId: Union[str, int] = None) -> ApiResponse:
         """
         Kicks a user from a chat.
 
         :param userId: The ID of the user to kick from the chat.
         :type userId: str
@@ -4304,14 +4307,15 @@
         ...     print("Failed to kick user.")
         """
         return ApiResponse(self.session.handler(
             method = "DELETE",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={1 if allowRejoin else 0}"
             ))
 
+
     @community
     def delete_chat(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Deletes a chat.
 
         :param chatId: The ID of the chat to delete.
         :type chatId: str
@@ -4340,14 +4344,15 @@
         ...     print("Failed to delete chat.")
         """
         return ApiResponse(self.session.handler(
             method = "DELETE",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}"
             ))
 
+
     @community
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """
         Deletes a message in a chat.
 
         :param chatId: The ID of the chat that contains the message.
         :type chatId: str
@@ -4391,14 +4396,15 @@
             "timestamp": int(time() * 1000)
             }
             )) if asStaff else ApiResponse(self.session.handler(
             method = "DELETE",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/message/{messageId}"
             ))
 
+
     @community
     def transfer_host(self, chatId: str, userId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Requests to transfer chat organizer privileges to another user.
 
         :param chatId: The ID of the chat where the transfer request will be made.
         :type chatId: str
@@ -4431,14 +4437,15 @@
         return ApiResponse(self.session.handler(
             method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/transfer-organizer",
             data = {
                 "uidList": [userId],
                 "timestamp": int(time() * 1000)
                 }))
 
+
     @community
     def accept_host(self, chatId: str, requestId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Accepts a request to transfer chat organizer privileges to the current user.
 
         :param chatId: The ID of the chat where the transfer request was made.
         :type chatId: str
@@ -4469,14 +4476,15 @@
         ...     print("Failed to accept transfer request.")
         """
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept"
             ))
 
+
     @community
     def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """
         Subscribes to an influencer's content.
 
         :param userId: The ID of the influencer to subscribe to.
         :type userId: str
@@ -4515,14 +4523,15 @@
                 "paymentContext": {
                     "transactionId": transactionId,
                     "isAutoRenew": autoRenew
                 },
                 "timestamp": int(time() * 1000)
                 }))
 
+
     @community
     def thank_props(self, chatId: str, userId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Sends a thank-you message to a user who has been tipped in a chat.
 
         :param chatId: The ID of the chat where the user was tipped.
         :type chatId: str
@@ -4553,14 +4562,15 @@
         ...     print("Failed to send thank-you message.")
         """
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank"
             ))
 
+
     @community
     def send_active(
         self,
         tz: int = -timezone // 1000,
         start: int = None,
         end: int = None,
         timers: list = None,
@@ -4618,14 +4628,15 @@
 
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/community/stats/user-active-time",
             data=data
             ))
 
+
     @community
     def send_coins(
         self,
         coins: int,
         blogId: str = None,
         chatId: str = None,
         wikiId: str = None,
@@ -4666,21 +4677,18 @@
         >>> response = client.community.send_coins(coins=100, chatId="0000-0000-0000-0000")
         ... if response.statuscode == 0:
         ...     print("Coins sent successfully!")
         ... else:
         ...     print("Failed to send coins.")
         """
         return ApiResponse(self.session.handler(
-            method="POST", url=f'/x{self.community_id if comId is None else comId}/s/{"blog" if blogId else "chat/thread" if chatId else "item"}/{blogId or chatId or wikiId}/tipping',
-            data={
-                "coins": coins,
-                "tippingContext": {"transactionId": transactionId or (str(uuid4()))},
-                "timestamp": int(time() * 1000)
-            }
-        ))
+            method="POST",
+            url=f'/x{self.community_id if comId is None else comId}/s/{"blog" if blogId else "chat/thread" if chatId else "item"}/{blogId or chatId or wikiId}/tipping',
+            data={"coins": coins, "tippingContext": {"transactionId": transactionId or (str(uuid4()))}, "timestamp": int(time() * 1000)}
+            ))
 
 
     @community
     def send_chat_props(self, coins: int, chatId: str, transactionId: str = None, comId: Union[str, int] = None) -> ApiResponse:
         """Refer to `send_coins` for documentation."""
         return self.send_coins(coins=coins, chatId=chatId, transactionId=transactionId, comId=comId)
 
@@ -4695,15 +4703,15 @@
     def start_chat(
         self,
         userIds: Union[str, List[str]],
         title: Optional[str] = None,
         message: Optional[str] = None,
         content: Optional[str] = None,
         comId: Optional[Union[str, int]] = None
-    ) -> ApiResponse:
+    ) -> CThread:
         """
         Creates a new chat with the given users.
 
         :param userIds: A single user ID or a list of user IDs to invite to the chat.
         :type userIds: Union[str, List[str]]
         :param title: The title of the chat. Defaults to `None`.
         :type title: Optional[str]
@@ -4714,15 +4722,15 @@
         :param comId: The ID of the community where the chat will be created. If not provided, the current community ID is used.
         :type comId: Optional[Union[str, int]]
         :return: An `ApiResponse` object containing information about the request status.
         :rtype: ApiResponse
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
-        `ApiResponse`:
+        `ApiResponse`: TODO: Update this to reflect the new return type.
 
         - `message`: A message indicating whether the chat was successfully created.
         - `statuscode`: The status code of the API response.
         - `duration`: The duration of the API request.
         - `timestamp`: The timestamp of the API request.
 
         **Example usage:**
@@ -4731,26 +4739,28 @@
 
         >>> response = client.community.start_chat(userIds=["0000-0000-0000-0000", "1111-1111-1111-1111"], title="New chat", message="Join my chat!", content="Hello, world!")
         ... if response.statuscode == 0:
         ...     print("Chat created successfully!")
         ... else:
         ...     print("Failed to create chat.")
         """
-        return ApiResponse(self.session.handler(
-            method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/chat/thread",
+        return CThread(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread",
             data = {
             "title": title,
             "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
             "initialMessageContent": message,
             "content": content,
             "type": 0,
             "publishToGlobal": 0,
             "timestamp": int(time() * 1000)
             }))
 
+
     @community
     def invite_chat(self, chatId: str, userIds: Union[str, List[str]], comId: Union[str, int] = None) -> ApiResponse:
         """
         Invites one or more users to join a chat.
 
         :param chatId: The ID of the chat to invite users to.
         :type chatId: str
@@ -4779,15 +4789,16 @@
         >>> response = client.community.invite_chat(chatId="0000-0000-0000-0000", userIds="0101-0101-0101-0101")
         ... if response.statuscode == 0:
         ...     print("Invitation sent successfully!")
         ... else:
         ...     print("Failed to send invitation.")
         """
         return ApiResponse(self.session.handler(
-            method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/invite",
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/invite",
             data = {
             "uids": userIds if isinstance(userIds, list) else [userIds],
             "timestamp": int(time() * 1000)
             }))
 
 
     @community
```

### Comparing `pymino-1.1.7.8/pymino/ext/context.py` & `pymino-1.1.7.9/pymino/ext/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1293,9 +1293,13 @@
                     "member_remove_your_cohost",
                 }:
                     return self._events[event](data)
                 else:
                     return self._events[event](context)
 
             if event == "text_message":
-                self._add_cache(data.chatId, data.author.userId, data.content)
+                if not self.command_exists(
+                    command_name=data.content[len(self.command_prefix):].split(" ")[0]
+                    ):
+                    self._add_cache(data.chatId, data.author.userId, data.content)
+
                 return self._handle_command(data=data, context=context)
```

### Comparing `pymino-1.1.7.8/pymino/ext/dispatcher.py` & `pymino-1.1.7.9/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/enums.py` & `pymino-1.1.7.9/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/exceptions.py` & `pymino-1.1.7.9/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/general.py` & `pymino-1.1.7.9/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/handlers.py` & `pymino-1.1.7.9/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/messages.py` & `pymino-1.1.7.9/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/threads.py` & `pymino-1.1.7.9/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/userprofile.py` & `pymino-1.1.7.9/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/entities/wsevents.py` & `pymino-1.1.7.9/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/socket.py` & `pymino-1.1.7.9/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/utilities/commands.py` & `pymino-1.1.7.9/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/utilities/generate.py` & `pymino-1.1.7.9/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino/ext/utilities/request_handler.py` & `pymino-1.1.7.9/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/pymino.egg-info/PKG-INFO` & `pymino-1.1.7.9/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.8
+Version: 1.1.7.9
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
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.8 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.9 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.8/pymino.egg-info/SOURCES.txt` & `pymino-1.1.7.9/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.8/setup.cfg` & `pymino-1.1.7.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e37 2e38 0d0a 6175  on = 1.1.7.8..au
+00000020: 6f6e 203d 2031 2e31 2e37 2e39 0d0a 6175  on = 1.1.7.9..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.7.8/setup.py` & `pymino-1.1.7.9/setup.py`

 * *Files identical despite different names*

