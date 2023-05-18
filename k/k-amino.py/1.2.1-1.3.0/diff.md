# Comparing `tmp/k-amino.py-1.2.1.tar.gz` & `tmp/k-amino.py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.2.1.tar", last modified: Sat Apr 15 11:16:34 2023, max compression
+gzip compressed data, was "k-amino.py-1.3.0.tar", last modified: Thu May 18 08:00:40 2023, max compression
```

## Comparing `k-amino.py-1.2.1.tar` & `k-amino.py-1.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.507357 k-amino.py-1.2.1/
--rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     2143 2023-04-15 11:16:34.508470 k-amino.py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.384998 k-amino.py-1.2.1/k_amino/
--rw-rw-rw-   0        0        0      872 2023-04-15 11:11:31.000000 k-amino.py-1.2.1/k_amino/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.427845 k-amino.py-1.2.1/k_amino/k_async/
--rw-rw-rw-   0        0        0      122 2023-04-09 03:38:43.000000 k-amino.py-1.2.1/k_amino/k_async/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.2.1/k_amino/k_async/acm.py
--rw-rw-rw-   0        0        0     2392 2023-04-15 05:50:54.000000 k-amino.py-1.2.1/k_amino/k_async/bot.py
--rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.2.1/k_amino/k_async/client.py
--rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.2.1/k_amino/k_async/local.py
--rw-rw-rw-   0        0        0    27434 2023-04-15 11:12:16.000000 k-amino.py-1.2.1/k_amino/k_async/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.466628 k-amino.py-1.2.1/k_amino/k_async/websocket_async/
--rw-rw-rw-   0        0        0      801 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/__init__.py
--rw-rw-rw-   0        0        0    13388 2023-04-14 11:31:01.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_abnf.py
--rw-rw-rw-   0        0        0    20115 2023-04-15 11:13:22.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_app.py
--rw-rw-rw-   0        0        0     2118 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_cookiejar.py
--rw-rw-rw-   0        0        0    20129 2023-04-15 10:09:33.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_core.py
--rw-rw-rw-   0        0        0     2105 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_exceptions.py
--rw-rw-rw-   0        0        0     6073 2023-04-14 11:59:23.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_handshake.py
--rw-rw-rw-   0        0        0    11803 2023-04-14 12:04:01.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_http.py
--rw-rw-rw-   0        0        0     2027 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_logging.py
--rw-rw-rw-   0        0        0     4922 2023-04-14 12:08:35.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_socket.py
--rw-rw-rw-   0        0        0     1122 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_ssl_compat.py
--rw-rw-rw-   0        0        0     4797 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_url.py
--rw-rw-rw-   0        0        0     3516 2023-04-14 11:23:07.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_utils.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 03:38:42.000000 k-amino.py-1.2.1/k_amino/k_async/websocket_async/_wsdump.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.483954 k-amino.py-1.2.1/k_amino/k_sync/
--rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.2.1/k_amino/k_sync/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.2.1/k_amino/k_sync/acm.py
--rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.2.1/k_amino/k_sync/bot.py
--rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.2.1/k_amino/k_sync/client.py
--rw-rw-rw-   0        0        0    45202 2023-04-15 06:24:52.000000 k-amino.py-1.2.1/k_amino/k_sync/local.py
--rw-rw-rw-   0        0        0    24349 2023-04-15 06:31:22.000000 k-amino.py-1.2.1/k_amino/k_sync/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.504349 k-amino.py-1.2.1/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-04-14 13:36:56.000000 k-amino.py-1.2.1/k_amino/lib/async_sessions.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-04-15 05:49:07.000000 k-amino.py-1.2.1/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.2.1/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0     1688 2023-04-09 07:16:48.000000 k-amino.py-1.2.1/k_amino/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:16:34.406671 k-amino.py-1.2.1/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2023-04-15 11:16:34.000000 k-amino.py-1.2.1/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 11:16:33.000000 k-amino.py-1.2.1/k_amino.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 11:16:34.512576 k-amino.py-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.613183 k-amino.py-1.3.0/
+-rw-rw-rw-   0        0        0      586 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-05-18 08:00:40.613183 k-amino.py-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.491336 k-amino.py-1.3.0/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-05-18 07:58:35.000000 k-amino.py-1.3.0/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.536282 k-amino.py-1.3.0/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     4438 2023-05-11 06:13:50.000000 k-amino.py-1.3.0/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     2392 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    31693 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    47044 2023-05-12 21:17:23.000000 k-amino.py-1.3.0/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    27434 2023-05-18 07:57:43.000000 k-amino.py-1.3.0/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.575287 k-amino.py-1.3.0/k_amino/k_async/websocket_async/
+-rw-rw-rw-   0        0        0      801 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/__init__.py
+-rw-rw-rw-   0        0        0    13388 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_abnf.py
+-rw-rw-rw-   0        0        0    20115 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_app.py
+-rw-rw-rw-   0        0        0     2118 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_cookiejar.py
+-rw-rw-rw-   0        0        0    20129 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_core.py
+-rw-rw-rw-   0        0        0     2105 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_exceptions.py
+-rw-rw-rw-   0        0        0     6073 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_handshake.py
+-rw-rw-rw-   0        0        0    11803 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_http.py
+-rw-rw-rw-   0        0        0     2027 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_logging.py
+-rw-rw-rw-   0        0        0     4922 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_socket.py
+-rw-rw-rw-   0        0        0     1122 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_ssl_compat.py
+-rw-rw-rw-   0        0        0     4797 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_url.py
+-rw-rw-rw-   0        0        0     3516 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_utils.py
+-rw-rw-rw-   0        0        0     6909 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_async/websocket_async/_wsdump.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.592239 k-amino.py-1.3.0/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     4256 2023-05-11 06:14:07.000000 k-amino.py-1.3.0/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-05-11 06:16:04.000000 k-amino.py-1.3.0/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    30339 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45934 2023-05-18 08:00:07.000000 k-amino.py-1.3.0/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    24349 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.610190 k-amino.py-1.3.0/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1688 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:00:40.516329 k-amino.py-1.3.0/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-05-18 08:00:40.000000 k-amino.py-1.3.0/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 08:00:39.000000 k-amino.py-1.3.0/k_amino.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 08:00:40.617174 k-amino.py-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-05-02 17:43:46.000000 k-amino.py-1.3.0/setup.py
```

### Comparing `k-amino.py-1.2.1/LICENSE` & `k-amino.py-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/PKG-INFO` & `k-amino.py-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.2.1
+Version: 1.3.0
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.2.1/README.md` & `k-amino.py-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/__init__.py` & `k-amino.py-1.3.0/k_amino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .k_async.acm import AsyncAcm
 from .k_async.client import AsyncClient
 from .k_async.local import AsyncSubClient
 # from .k_async.sockets import *
 from .k_async.bot import AsyncBot
 
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
 
 
 __newest__ = loads(get("https://pypi.python.org/pypi/k-amino.py/json").text)["info"]["version"]
 
 if __version__ != __newest__:
     print(f"\033[1;31;38mk_amino New Version!: {__newest__} (You are using {__version__})\033[1;36;33m\nDiscord server: \"https://discord.gg/zd8gyFJquT\"\033[1;0m")
 else:
```

### Comparing `k-amino.py-1.2.1/k_amino/k_async/acm.py` & `k-amino.py-1.3.0/k_amino/k_async/acm.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 
         if rank not in ["transfer-agent", "leader", "curator"]:
             raise TypeError(rank)
 
         req = await self.postRequest(f"/x{self.comId}/s/user-profile/{userId}/{rank}")
         return Json(req)
 
+    """
+    async def set_push_settings(self, activities: bool = None, broadcasts: bool = None, cid: int = 0):
+        return await self.http.post('user-profile/push', dict(
+            pushEnabled=bool(activities or broadcasts),
+            pushExtensions=dict(
+                **dict(communityBroadcastsEnabled=broadcasts) if broadcasts else {},
+                **dict(communityActivitiesEnabled=activities) if activities else {},
+                #systemEnabled=enable
+            )
+        ), cid=cid) 
+    """
     async def accept_join_request(self, userId: str):
         req = await self.postRequest(
             f"/x{self.comId}/s/community/membership-request/{userId}/accept"
         )
         return Json(req)
 
     async def reject_join_request(self, userId: str):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `k-amino.py-1.2.1/k_amino/k_async/bot.py` & `k-amino.py-1.3.0/k_amino/k_async/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/client.py` & `k-amino.py-1.3.0/k_amino/k_async/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/local.py` & `k-amino.py-1.3.0/k_amino/k_async/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Union, BinaryIO
 from uuid import UUID
 
 from ..lib.objects import *
 from ..lib.async_sessions import AsyncSession as Session
 from .acm import AsyncAcm as Acm
 
-
 class AsyncSubClient(Acm, Session):
     def __init__(self, comId: str, proxies: dict = None, acm: bool = False):
         self.proxies = proxies
         self.comId = comId
 
         if acm:
             Acm.__init__(self, comId=self.comId, proxies=self.proxies)
@@ -123,22 +122,36 @@
 
     async def get_online_users(self, start: int = 0, size: int = 25):
         req = await self.getRequest(
             f"/x{self.comId}/s/live-layer?topic=ndtopic:x{self.comId}:online-members&start={start}&size={size}"
         )
         return UserProfileList(req["userProfileList"]).UserProfileList
 
-    async def get_public_chats(
-        self, filterType: str = "recommended", start: int = 0, size: int = 50
-    ):
-        req = await self.getRequest(
-            f"/x{self.comId}/s/chat/thread?type=public-all&filterType={filterType}&start={start}&size={size}"
-        )
+    async def get_public_chats(self, filterType: str = "recommended", start: int = 0, size: int = 50):
+        req = await self.getRequest(f"/x{self.comId}/s/chat/thread?type=public-all&filterType={filterType}&start={start}&size={size}")
         return ThreadList(req["threadList"]).ThreadList
 
+    async def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
+        data = {
+            "type": 0,
+            "content": message,
+            "extensions": {
+                "linkSnippetList": [{
+                    "link": link,
+                    "mediaType": 100,
+                    "mediaUploadValue": b64encode(image.read()).decode(),
+                    "mediaUploadValueContentType": "image/png"
+                }]
+            },
+            "clientRefId": int(timestamp() / 10 % 100000000),
+            "timestamp": int(timestamp() * 1000),
+            "attachedObject": None
+        }
+        return Json(await self.postRequest(f"/x{self.comId}/s/chat/thread/{chatId}/message", data))
+
     async def send_message(
         self,
         chatId: str,
         message: str = None,
         messageType: int = 0,
         file: BinaryIO = None,
         fileType: str = None,
```

### Comparing `k-amino.py-1.2.1/k_amino/k_async/sockets.py` & `k-amino.py-1.3.0/k_amino/k_async/sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,15 +672,15 @@
         if first_time:
             loop, th = self.start_async()
             loop = self.submit_async(self.reboot_socket(), loop)
 
     async def reboot_socket(self):
         self.run_reboot = True
         while self.run_reboot:
-            await asyncio.sleep(120)
+            await asyncio.sleep(300)
             await self.close()
             await self.launch(False)
 
     def start_async(self):
         loop = asyncio.new_event_loop()
         th = threading.Thread(target=loop.run_forever)
         th.start()
```

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/__init__.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/__init__.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_abnf.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_abnf.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_app.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_app.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_cookiejar.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_cookiejar.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_core.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_core.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_exceptions.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_exceptions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_handshake.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_handshake.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_http.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_http.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_logging.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_logging.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_socket.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_socket.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_ssl_compat.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_url.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_url.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_utils.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_utils.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_async/websocket_async/_wsdump.py` & `k-amino.py-1.3.0/k_amino/k_async/websocket_async/_wsdump.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_sync/bot.py` & `k-amino.py-1.3.0/k_amino/k_sync/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_sync/client.py` & `k-amino.py-1.3.0/k_amino/k_sync/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/k_sync/local.py` & `k-amino.py-1.3.0/k_amino/k_sync/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,32 @@
         self, filterType: str = "recommended", start: int = 0, size: int = 50
     ):
         req = self.getRequest(
             f"/x{self.comId}/s/chat/thread?type=public-all&filterType={filterType}&start={start}&size={size}"
         )
         return ThreadList(req["threadList"]).ThreadList
 
+    def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
+        data = {
+            "type": 0,
+            "content": message,
+            "extensions": {
+                "linkSnippetList": [{
+                    "link": link,
+                    "mediaType": 100,
+                    "mediaUploadValue": b64encode(image.read()).decode(),
+                    "mediaUploadValueContentType": "image/png"
+                }]
+            },
+            "clientRefId": int(timestamp() / 10 % 100000000),
+            "timestamp": int(timestamp() * 1000),
+            "attachedObject": None
+        }
+        return Json(self.postRequest(f"/x{self.comId}/s/chat/thread/{chatId}/message", data))
+
     def send_message(
         self,
         chatId: str,
         message: str = None,
         messageType: int = 0,
         file: BinaryIO = None,
         fileType: str = None,
```

### Comparing `k-amino.py-1.2.1/k_amino/k_sync/sockets.py` & `k-amino.py-1.3.0/k_amino/k_sync/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/lib/async_sessions.py` & `k-amino.py-1.3.0/k_amino/lib/async_sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/lib/exception.py` & `k-amino.py-1.3.0/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/lib/headers.py` & `k-amino.py-1.3.0/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/lib/objects.py` & `k-amino.py-1.3.0/k_amino/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/lib/sessions.py` & `k-amino.py-1.3.0/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino/lib/util.py` & `k-amino.py-1.3.0/k_amino/lib/util.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/k_amino.py.egg-info/PKG-INFO` & `k-amino.py-1.3.0/k_amino.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.2.1
+Version: 1.3.0
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.2.1/k_amino.py.egg-info/SOURCES.txt` & `k-amino.py-1.3.0/k_amino.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.2.1/setup.py` & `k-amino.py-1.3.0/setup.py`

 * *Files identical despite different names*

