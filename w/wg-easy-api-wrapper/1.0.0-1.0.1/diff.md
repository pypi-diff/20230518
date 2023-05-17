# Comparing `tmp/wg-easy-api-wrapper-1.0.0.tar.gz` & `tmp/wg-easy-api-wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg-easy-api-wrapper-1.0.0.tar", last modified: Wed May 17 21:29:21 2023, max compression
+gzip compressed data, was "wg-easy-api-wrapper-1.0.1.tar", last modified: Wed May 17 22:08:52 2023, max compression
```

## Comparing `wg-easy-api-wrapper-1.0.0.tar` & `wg-easy-api-wrapper-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 21:29:21.098160 wg-easy-api-wrapper-1.0.0/
--rw-rw-rw-   0        0        0      259 2023-05-17 21:29:21.097624 wg-easy-api-wrapper-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-17 21:29:21.099169 wg-easy-api-wrapper-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      416 2023-05-17 21:08:04.000000 wg-easy-api-wrapper-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:29:21.082408 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper/
--rw-rw-rw-   0        0        0       56 2023-05-17 21:01:47.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0     4653 2023-05-17 21:22:40.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper/client.py
--rw-rw-rw-   0        0        0     1808 2023-05-17 20:55:12.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper/server.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:29:21.093871 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0      259 2023-05-17 21:29:20.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-17 21:29:21.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:29:20.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-17 21:29:20.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-17 21:29:20.000000 wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-17 22:08:52.370329 wg-easy-api-wrapper-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-17 22:08:43.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:08:52.366329 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 22:08:52.000000 wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper.egg-info/top_level.txt
```

### Comparing `wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper/client.py` & `wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-from datetime import datetime
-from typing import TYPE_CHECKING
-
-import aiohttp
-
-time_format = "%Y-%m-%dT%H:%M:%S.%fZ"
-
-if TYPE_CHECKING:
-    from .server import Server
-
-
-class Client:
-    def __init__(self,
-                 address: str,
-                 created_at: str,
-                 enabled: bool,
-                 uid: str,
-                 last_handshake_at: str,
-                 name: str,
-                 persistent_keepalive: str,
-                 public_key: str,
-                 transfer_rx: int,
-                 transfer_tx: int,
-                 updated_at: str,
-                 session: aiohttp.ClientSession,
-                 server: 'Server',):
-        # вывод всех входящих аргументов
-        print(address, created_at, enabled, uid, last_handshake_at, name, persistent_keepalive, public_key, transfer_rx, transfer_tx, updated_at)
-        self._address = address
-        self._created_at = datetime.strptime(created_at, time_format)
-        self._enabled = bool(enabled)
-        self._uid = uid
-        self._last_handshake_at = datetime.strptime(last_handshake_at, time_format) if last_handshake_at else None
-        self._name = name
-        self._persistent_keepalive = persistent_keepalive
-        self._public_key = public_key
-        self._transfer_rx = transfer_rx
-        self._transfer_tx = transfer_tx
-        self._updated_at = datetime.strptime(updated_at, time_format)
-        self._session = session
-        self._server = server
-
-    @classmethod
-    def from_json(cls, json, session: aiohttp.ClientSession, server: 'Server'):
-        return cls(
-            address=json["address"],
-            created_at=json["createdAt"],
-            enabled=bool(json["enabled"]),
-            uid=json["id"],
-            last_handshake_at=json["latestHandshakeAt"],
-            name=json["name"],
-            persistent_keepalive=json["persistentKeepalive"],
-            public_key=json["publicKey"],
-            transfer_rx=json["transferRx"],
-            transfer_tx=json["transferTx"],
-            updated_at=json["updatedAt"],
-            session=session,
-            server=server,
-        )
-
-    @property
-    def name(self):
-        return self._name
-
-    @name.setter
-    async def name(self, value):
-        await self._session.put(
-            self._server.url_builder("/api/wireguard/client/{}/name".format(self._uid)),
-            json={"name": value}
-        )
-        self._name = value
-
-    @property
-    def address(self):
-        return self._address
-
-    @address.setter
-    async def address(self, value):
-        await self._session.put(
-            self._server.url_builder("/api/wireguard/client/{}/address".format(self._uid)),
-            json={"address": value}
-        )
-        self._address = value
-
-    @property
-    def created_at(self):
-        return self._created_at
-
-    @property
-    def last_handshake_at(self):
-        return self._last_handshake_at
-
-    @property
-    def updated_at(self):
-        return self._updated_at
-
-    @property
-    def enabled(self):
-        return self._enabled
-
-    @property
-    def uid(self):
-        return self._uid
-
-    @property
-    def persistent_keepalive(self):
-        return self._persistent_keepalive
-
-    @property
-    def public_key(self):
-        return self._public_key
-
-    @property
-    def transfer_rx(self):
-        return self._transfer_rx
-
-    @property
-    def transfer_tx(self):
-        return self._transfer_tx
-
-    async def enable(self):
-        if self._enabled:
-            raise ValueError("Client is already enabled")
-        await self._session.put(
-            self._server.url_builder("/api/wireguard/client/{}/enable".format(self._uid)),
-            json={"enable": True}
-        )
-        self._enabled = True
-
-    async def disable(self):
-        if not self._enabled:
-            raise ValueError("Client is already disabled")
-        await self._session.post(
-            self._server.url_builder("/api/wireguard/client/{}/disable".format(self._uid)),
-        )
-        self._enabled = False
-
-    async def get_qr_code(self):
-        return await self._session.get(
-            self._server.url_builder("/api/wireguard/client/{}/qrcode.svg".format(self._uid))
-        )
-
-    async def get_configuration(self):
-        config_file = await self._session.get(
-            self._server.url_builder("/api/wireguard/client/{}/configuration".format(self._uid))
-        )
-        # вернуть как текст
-        return await config_file.text()
+from datetime import datetime
+from typing import TYPE_CHECKING
+
+import aiohttp
+
+time_format = "%Y-%m-%dT%H:%M:%S.%fZ"
+
+if TYPE_CHECKING:
+    from .server import Server
+
+
+class Client:
+    def __init__(self,
+                 address: str,
+                 created_at: str,
+                 enabled: bool,
+                 uid: str,
+                 last_handshake_at: str,
+                 name: str,
+                 persistent_keepalive: str,
+                 public_key: str,
+                 transfer_rx: int,
+                 transfer_tx: int,
+                 updated_at: str,
+                 session: aiohttp.ClientSession,
+                 server: 'Server',):
+        # вывод всех входящих аргументов
+        print(address, created_at, enabled, uid, last_handshake_at, name, persistent_keepalive, public_key, transfer_rx, transfer_tx, updated_at)
+        self._address = address
+        self._created_at = datetime.strptime(created_at, time_format)
+        self._enabled = bool(enabled)
+        self._uid = uid
+        self._last_handshake_at = datetime.strptime(last_handshake_at, time_format) if last_handshake_at else None
+        self._name = name
+        self._persistent_keepalive = persistent_keepalive
+        self._public_key = public_key
+        self._transfer_rx = transfer_rx
+        self._transfer_tx = transfer_tx
+        self._updated_at = datetime.strptime(updated_at, time_format)
+        self._session = session
+        self._server = server
+
+    @classmethod
+    def from_json(cls, json, session: aiohttp.ClientSession, server: 'Server'):
+        return cls(
+            address=json["address"],
+            created_at=json["createdAt"],
+            enabled=bool(json["enabled"]),
+            uid=json["id"],
+            last_handshake_at=json["latestHandshakeAt"],
+            name=json["name"],
+            persistent_keepalive=json["persistentKeepalive"],
+            public_key=json["publicKey"],
+            transfer_rx=json["transferRx"],
+            transfer_tx=json["transferTx"],
+            updated_at=json["updatedAt"],
+            session=session,
+            server=server,
+        )
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    async def name(self, value):
+        await self._session.put(
+            self._server.url_builder("/api/wireguard/client/{}/name".format(self._uid)),
+            json={"name": value}
+        )
+        self._name = value
+
+    @property
+    def address(self):
+        return self._address
+
+    @address.setter
+    async def address(self, value):
+        await self._session.put(
+            self._server.url_builder("/api/wireguard/client/{}/address".format(self._uid)),
+            json={"address": value}
+        )
+        self._address = value
+
+    @property
+    def created_at(self):
+        return self._created_at
+
+    @property
+    def last_handshake_at(self):
+        return self._last_handshake_at
+
+    @property
+    def updated_at(self):
+        return self._updated_at
+
+    @property
+    def enabled(self):
+        return self._enabled
+
+    @property
+    def uid(self):
+        return self._uid
+
+    @property
+    def persistent_keepalive(self):
+        return self._persistent_keepalive
+
+    @property
+    def public_key(self):
+        return self._public_key
+
+    @property
+    def transfer_rx(self):
+        return self._transfer_rx
+
+    @property
+    def transfer_tx(self):
+        return self._transfer_tx
+
+    async def enable(self):
+        if self._enabled:
+            raise ValueError("Client is already enabled")
+        await self._session.put(
+            self._server.url_builder("/api/wireguard/client/{}/enable".format(self._uid)),
+            json={"enable": True}
+        )
+        self._enabled = True
+
+    async def disable(self):
+        if not self._enabled:
+            raise ValueError("Client is already disabled")
+        await self._session.post(
+            self._server.url_builder("/api/wireguard/client/{}/disable".format(self._uid)),
+        )
+        self._enabled = False
+
+    async def get_qr_code(self):
+        return await self._session.get(
+            self._server.url_builder("/api/wireguard/client/{}/qrcode.svg".format(self._uid))
+        )
+
+    async def get_configuration(self):
+        config_file = await self._session.get(
+            self._server.url_builder("/api/wireguard/client/{}/configuration".format(self._uid))
+        )
+        # вернуть как текст
+        return await config_file.text()
```

### Comparing `wg-easy-api-wrapper-1.0.0/wg_easy_api_wrapper/server.py` & `wg-easy-api-wrapper-1.0.1/wg_easy_api_wrapper/server.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import aiohttp
-from .client import Client
-
-
-class Server:
-    def __init__(self, host: str, port: int, password: str, session: aiohttp.ClientSession = None):
-        self.host = host
-        self.port = port
-        self._password = password
-        self._session = session
-        self.clients = []
-
-    def url_builder(self, path: str) -> str:
-        return f"http://{self.host}:{self.port}{path}"
-
-    def __enter__(self):
-        if self._session is None:
-            self._session = aiohttp.ClientSession()
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self._session.close()
-
-    async def login(self):
-        # POST to /api/session
-        await self._session.post(self.url_builder("/api/session"), json={"password": self._password})
-        session = await self.get_session()
-        return session
-
-    async def logout(self) -> None:
-        # DELETE to /api/session
-        await self._session.delete(self.url_builder("/api/session"))
-
-    async def get_session(self):
-        # GET to /api/session
-        answer = await self._session.get(self.url_builder("/api/session"))
-        return answer
-
-    async def get_clients(self):
-        # GET to /api/clients
-        answer = await self._session.get(self.url_builder("/api/wireguard/client"))
-        return [Client.from_json(client, self._session, self) for client in await answer.json()]
-
-    async def remove_client(self, uid: str):
-        # DELETE to /api/clients/{list_id}
-        await self._session.delete(self.url_builder("/api/wireguard/client/{}".format(uid)))
-
-    async def create_client(self, name: str):
-        await self._session.post(
-            self.url_builder("/api/wireguard/client"),
-            json={"name": name},
-        )
-
-
-
-
+import aiohttp
+from .client import Client
+
+
+class Server:
+    def __init__(self, host: str, port: int, password: str, session: aiohttp.ClientSession = None):
+        self.host = host
+        self.port = port
+        self._password = password
+        self._session = session
+        self.clients = []
+
+    def url_builder(self, path: str) -> str:
+        return f"http://{self.host}:{self.port}{path}"
+
+    def __enter__(self):
+        if self._session is None:
+            self._session = aiohttp.ClientSession()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._session.close()
+
+    async def login(self):
+        # POST to /api/session
+        await self._session.post(self.url_builder("/api/session"), json={"password": self._password})
+        session = await self.get_session()
+        return session
+
+    async def logout(self) -> None:
+        # DELETE to /api/session
+        await self._session.delete(self.url_builder("/api/session"))
+
+    async def get_session(self):
+        # GET to /api/session
+        answer = await self._session.get(self.url_builder("/api/session"))
+        return answer
+
+    async def get_clients(self):
+        # GET to /api/clients
+        answer = await self._session.get(self.url_builder("/api/wireguard/client"))
+        return [Client.from_json(client, self._session, self) for client in await answer.json()]
+
+    async def remove_client(self, uid: str):
+        # DELETE to /api/clients/{list_id}
+        await self._session.delete(self.url_builder("/api/wireguard/client/{}".format(uid)))
+
+    async def create_client(self, name: str):
+        await self._session.post(
+            self.url_builder("/api/wireguard/client"),
+            json={"name": name},
+        )
+
+
+
+
```

