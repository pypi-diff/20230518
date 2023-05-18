# Comparing `tmp/wg-easy-api-wrapper-1.0.2.tar.gz` & `tmp/wg-easy-api-wrapper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg-easy-api-wrapper-1.0.2.tar", last modified: Wed May 17 22:28:33 2023, max compression
+gzip compressed data, was "wg-easy-api-wrapper-1.0.3.tar", last modified: Thu May 18 13:29:42 2023, max compression
```

## Comparing `wg-easy-api-wrapper-1.0.2.tar` & `wg-easy-api-wrapper-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:28:33.783729 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 22:28:26.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:28:33.787729 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 22:28:33.000000 wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:29:42.014871 wg-easy-api-wrapper-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-18 13:29:42.014871 wg-easy-api-wrapper-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-18 13:29:42.014871 wg-easy-api-wrapper-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:29:42.014871 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-18 13:29:34.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:29:42.014871 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-18 13:29:42.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-18 13:29:42.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:29:42.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 13:29:42.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 13:29:42.000000 wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper.egg-info/top_level.txt
```

### Comparing `wg-easy-api-wrapper-1.0.2/setup.cfg` & `wg-easy-api-wrapper-1.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wg-easy-api-wrapper
-version = 1.0.2
+version = 1.0.3
 author = MrShandy
 author_email = mrshandy@shandy-dev.ru
 description = Wrapper for wg-easy API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Shandeika/wg-easy-api-wrapper
 license = GPL-3.0
```

### Comparing `wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/client.py` & `wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  name: str,
                  persistent_keepalive: str,
                  public_key: str,
                  transfer_rx: int,
                  transfer_tx: int,
                  updated_at: str,
                  session: aiohttp.ClientSession,
-                 server: 'Server',):
+                 server: 'Server', ):
         self._address = address
         self._created_at = datetime.strptime(created_at, time_format)
         self._enabled = bool(enabled)
         self._uid = uid
         self._last_handshake_at = datetime.strptime(last_handshake_at, time_format) if last_handshake_at else None
         self._name = name
         self._persistent_keepalive = persistent_keepalive
```

### Comparing `wg-easy-api-wrapper-1.0.2/wg_easy_api_wrapper/server.py` & `wg-easy-api-wrapper-1.0.3/wg_easy_api_wrapper/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 import aiohttp
+
 from .client import Client
+from .errors import AlreadyLoggedInError
 
 
 class Server:
     def __init__(self, host: str, port: int, password: str, session: aiohttp.ClientSession = None):
         self.host = host
         self.port = port
         self._password = password
-        self._session = session
-        self.clients = []
+        self._session = aiohttp.ClientSession() if session is None else session
+
+    async def is_logged_in(self):
+        session = await self.get_session()
+        json_response = await session.json()
+        return json_response["authenticated"]
 
     def url_builder(self, path: str) -> str:
         return f"http://{self.host}:{self.port}{path}"
 
-    def __enter__(self):
-        if self._session is None:
-            self._session = aiohttp.ClientSession()
+    async def __aenter__(self):
+        await self.login()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self._session.close()
+    async def __aexit__(self, exc_type, exc, exc_tb):
+        if await self.is_logged_in():
+            await self.logout()
+        await self._session.close()
+        if exc:
+            raise exc
 
     async def login(self):
-        # POST to /api/session
+        if await self.is_logged_in():
+            raise AlreadyLoggedInError("You are already logged in")
         await self._session.post(self.url_builder("/api/session"), json={"password": self._password})
         session = await self.get_session()
         return session
 
     async def logout(self) -> None:
-        # DELETE to /api/session
+        if not await self.is_logged_in():
+            raise AlreadyLoggedInError("You are not logged in")
         await self._session.delete(self.url_builder("/api/session"))
 
     async def get_session(self):
         # GET to /api/session
         answer = await self._session.get(self.url_builder("/api/session"))
         return answer
 
@@ -46,11 +57,7 @@
         await self._session.delete(self.url_builder("/api/wireguard/client/{}".format(uid)))
 
     async def create_client(self, name: str):
         await self._session.post(
             self.url_builder("/api/wireguard/client"),
             json={"name": name},
         )
-
-
-
-
```

