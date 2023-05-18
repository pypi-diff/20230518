# Comparing `tmp/aioairzone-cloud-0.0.3.tar.gz` & `tmp/aioairzone-cloud-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.0.3.tar", last modified: Thu May 18 08:21:47 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.0.4.tar", last modified: Thu May 18 16:30:20 2023, max compression
```

## Comparing `aioairzone-cloud-0.0.3.tar` & `aioairzone-cloud-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.3/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.3/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.3/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    12864 2022-04-27 17:54:29.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4225 2022-04-06 19:26:33.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2890 2022-04-06 19:36:15.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      624 2022-04-06 08:18:59.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1168 2022-04-06 10:44:53.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3775 2022-04-06 08:42:41.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    17976 2022-04-06 19:27:54.000000 aioairzone-cloud-0.0.3/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-18 08:21:47.000000 aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-18 08:20:12.000000 aioairzone-cloud-0.0.3/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.3/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-18 08:21:47.528369 aioairzone-cloud-0.0.3/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.4/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.4/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.4/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    13337 2023-05-18 16:26:53.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4225 2022-04-06 19:26:33.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2890 2022-04-06 19:36:15.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      731 2023-05-18 16:12:10.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1168 2022-04-06 10:44:53.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3775 2022-04-06 08:42:41.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    17976 2022-04-06 19:27:54.000000 aioairzone-cloud-0.0.4/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-18 16:30:20.000000 aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-18 16:27:43.000000 aioairzone-cloud-0.0.4/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.4/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-18 16:30:20.793392 aioairzone-cloud-0.0.4/setup.cfg
```

### Comparing `aioairzone-cloud-0.0.3/LICENSE` & `aioairzone-cloud-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/PKG-INFO` & `aioairzone-cloud-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/cloudapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Airzone Cloud API."""
 from __future__ import annotations
 
 import logging
 import urllib.parse
 from typing import Any, cast
 
-from aiohttp import ClientConnectorError, ClientSession
+from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aiohttp.client_reqrep import ClientResponse
 
 from .common import ConnectionOptions
 from .const import (
     API_AUTH_LOGIN,
     API_AUTH_REFRESH_TOKEN,
     API_AZ_SYSTEM,
@@ -35,15 +35,21 @@
     AZD_WEBSERVERS,
     AZD_ZONES,
     HEADER_AUTHORIZATION,
     HEADER_BEARER,
     HTTP_CALL_TIMEOUT,
 )
 from .device import Device
-from .exceptions import LoginError, TokenRefreshError
+from .exceptions import (
+    AirzoneCloudError,
+    APIError,
+    LoginError,
+    TokenRefreshError,
+    TooManyRequests,
+)
 from .installation import Installation
 from .system import System
 from .webserver import WebServer
 from .zone import Zone
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -67,27 +73,41 @@
         self.zones: list[Zone] = []
 
     async def api_request(
         self, method: str, path: str, json: Any | None = None
     ) -> dict[str, Any]:
         """Airzone Cloud API request."""
         _LOGGER.debug("aiohttp request: /%s (params=%s)", path, json)
+
         headers: dict[str, str] = {}
         if self.token:
             headers[HEADER_AUTHORIZATION] = f"{HEADER_BEARER} {self.token}"
-        resp: ClientResponse = await self.aiohttp_session.request(
-            method,
-            f"{API_URL}/{path}",
-            headers=headers,
-            json=json,
-            raise_for_status=True,
-            timeout=HTTP_CALL_TIMEOUT,
-        )
+
+        try:
+            resp: ClientResponse = await self.aiohttp_session.request(
+                method,
+                f"{API_URL}/{path}",
+                headers=headers,
+                json=json,
+                raise_for_status=True,
+                timeout=HTTP_CALL_TIMEOUT,
+            )
+        except ClientResponseError as err:
+            if path.endswith(API_AUTH_LOGIN):
+                raise LoginError from err
+
+            if err.status == 400:
+                raise APIError from err
+            if err.status == 429:
+                raise TooManyRequests from err
+            raise AirzoneCloudError from err
+
         resp_json = await resp.json(content_type=None)
         _LOGGER.debug("aiohttp response: %s", resp_json)
+
         return cast(dict, resp_json)
 
     async def api_get_device_config(self, device: Device) -> dict[str, Any]:
         """Request API device config data."""
         dev_id = urllib.parse.quote(device.get_id())
 
         params = {
```

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/common.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/const.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/device.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,7 +20,11 @@
 
 class InvalidParam(AirzoneCloudError):
     """Exception raised when invalid param is requested."""
 
 
 class ParamUpdateFailure(AirzoneCloudError):
     """Exception raised when parameter isn't updated."""
+
+
+class TooManyRequests(AirzoneCloudError):
+    """Exception raised when max API requests are exceeded."""
```

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.0.4/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.3/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.0.4/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.3/pyproject.toml` & `aioairzone-cloud-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.0.3"
+version = "0.0.4"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

