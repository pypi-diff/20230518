# Comparing `tmp/spothinta-0.0.2.tar.gz` & `tmp/spothinta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spothinta-0.0.2.tar", max compression
+gzip compressed data, was "spothinta-0.1.0.tar", max compression
```

## Comparing `spothinta-0.0.2.tar` & `spothinta-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-05-18 11:55:47.282059 spothinta-0.0.2/LICENSE
--rw-r--r--   0        0        0     5123 2023-05-18 11:55:47.282059 spothinta-0.0.2/README.md
--rw-r--r--   0        0        0     3642 2023-05-18 11:56:12.890859 spothinta-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      363 2023-05-18 11:55:47.282059 spothinta-0.0.2/spothinta/__init__.py
--rw-r--r--   0        0        0      106 2023-05-18 11:55:47.282059 spothinta-0.0.2/spothinta/const.py
--rw-r--r--   0        0        0      303 2023-05-18 11:55:47.282059 spothinta-0.0.2/spothinta/exceptions.py
--rw-r--r--   0        0        0     5844 2023-05-18 11:55:47.282059 spothinta-0.0.2/spothinta/models.py
--rw-r--r--   0        0        0        0 2023-05-18 11:55:47.282059 spothinta-0.0.2/spothinta/py.typed
--rw-r--r--   0        0        0     4183 2023-05-18 11:55:47.282059 spothinta-0.0.2/spothinta/spothinta.py
--rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 spothinta-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-18 18:50:45.683146 spothinta-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5123 2023-05-18 18:50:45.687147 spothinta-0.1.0/README.md
+-rw-r--r--   0        0        0     3639 2023-05-18 18:50:59.811289 spothinta-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/const.py
+-rw-r--r--   0        0        0      303 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/exceptions.py
+-rw-r--r--   0        0        0     5844 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/models.py
+-rw-r--r--   0        0        0        0 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/py.typed
+-rw-r--r--   0        0        0     4348 2023-05-18 18:50:45.687147 spothinta-0.1.0/spothinta/spothinta.py
+-rw-r--r--   0        0        0     6237 1970-01-01 00:00:00.000000 spothinta-0.1.0/PKG-INFO
```

### Comparing `spothinta-0.0.2/LICENSE` & `spothinta-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spothinta-0.0.2/README.md` & `spothinta-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spothinta-0.0.2/pyproject.toml` & `spothinta-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spothinta"
-version = "0.0.2"
+version = "0.1.0"
 description = "Asynchronous Python client providing energy prices from spot-hinta.fi"
 authors = [
   "Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>",
   "Klaas Schoute <hello@student-techlife.com>"
 ]
 maintainers = ["Sebastian Lövdahl <sebastian.lovdahl@hibox.fi>"]
 license = "MIT"
@@ -22,15 +22,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
     { include = "spothinta" }
 ]
 
 [tool.poetry.scripts]
-example = "examples.energy:__main__"
+example = "examples.energy:start"
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `spothinta-0.0.2/spothinta/models.py` & `spothinta-0.1.0/spothinta/models.py`

 * *Files identical despite different names*

### Comparing `spothinta-0.0.2/spothinta/spothinta.py` & `spothinta-0.1.0/spothinta/spothinta.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,31 @@
 from typing import Any, cast
 
 import async_timeout
 from aiohttp.client import ClientError, ClientSession
 from aiohttp.hdrs import METH_GET
 from yarl import URL
 
-from .const import API_HOST
-from .exceptions import (
-    SpotHintaConnectionError,
-    SpotHintaError,
-    SpotHintaNoDataError,
-)
+from .const import API_HOST, Region
+from .exceptions import SpotHintaConnectionError, SpotHintaError, SpotHintaNoDataError
 from .models import Electricity
 
 
 @dataclass
 class SpotHinta:
     """Main class for handling data fetching from spot-hinta.fi."""
 
     request_timeout: float = 10.0
     session: ClientSession | None = None
 
     _close_session: bool = False
 
     async def _request(
         self,
-        *,
+        uri: str,
         method: str = METH_GET,
         params: dict[str, Any] | None = None,
     ) -> Any:
         """Handle a request to the API of spot-hinta.fi.
 
         Args:
         ----
@@ -56,15 +52,15 @@
                 the API.
         """
         version = metadata.version(__package__)
 
         url = URL.build(
             scheme="https",
             host=API_HOST,
-            path="/TodayAndDayForward",
+            path=uri,
         )
 
         headers = {
             "Accept": "application/json",
             "User-Agent": f"PythonSpotHinta/{version}",
         }
 
@@ -100,29 +96,36 @@
             raise SpotHintaError(
                 msg,
                 {"Content-Type": content_type, "response": text},
             )
 
         return cast(dict[str, Any], await response.json())
 
-    async def energy_prices(self) -> Electricity:
-        """Get energy prices for a given period.
+    async def energy_prices(self, region: Region = Region.FI) -> Electricity:
+        """Get energy prices for today and tomorrow for a region.
 
-        Returns
+        Args:
+        ----
+            region: The region to get prices for.
+
+        Returns:
         -------
             A Python dictionary with the response from spot-hinta.fi.
 
-        Raises
+        Raises:
         ------
-            SpotHintaNoDataError: No energy prices found for this period.
+            SpotHintaNoDataError: No energy prices found.
         """
-        data = await self._request()
+        data = await self._request(
+            uri="/TodayAndDayForward",
+            params={"region": region.name},
+        )
 
         if len(data) == 0:
-            msg = "No energy prices found for this period."
+            msg = "No energy prices found."
             raise SpotHintaNoDataError(msg)
         return Electricity.from_dict(data)
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
```

### Comparing `spothinta-0.0.2/PKG-INFO` & `spothinta-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spothinta
-Version: 0.0.2
+Version: 0.1.0
 Summary: Asynchronous Python client providing energy prices from spot-hinta.fi
 License: MIT
 Keywords: energy,spothinta,prices,api,async,client
 Author: Sebastian Lövdahl
 Author-email: sebastian.lovdahl@hibox.fi
 Maintainer: Sebastian Lövdahl
 Maintainer-email: sebastian.lovdahl@hibox.fi
```

