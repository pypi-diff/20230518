# Comparing `tmp/govee_led_wez-0.0.8.tar.gz` & `tmp/govee_led_wez-0.0.9.tar.gz`

## Comparing `govee_led_wez-0.0.8.tar` & `govee_led_wez-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/Makefile
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/ble.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/setup.cfg
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/__init__.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/ble.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/color.py
--rw-r--r--   0        0        0    31997 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/govee.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/http.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/kelvin_rgb.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/govee_led_wez/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/tests/test_stuff.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/LICENSE
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/README.md
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 govee_led_wez-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/Makefile
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/ble.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/__init__.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/ble.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/color.py
+-rw-r--r--   0        0        0    31997 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/govee.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/http.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/kelvin_rgb.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/govee_led_wez/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/tests/test_stuff.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/README.md
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 govee_led_wez-0.0.9/PKG-INFO
```

### Comparing `govee_led_wez-0.0.8/ble.py` & `govee_led_wez-0.0.9/ble.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import logging
 from uuid import UUID
 from typing import Union, List
 from bleak import BleakScanner, BleakClient, AdvertisementData, BLEDevice
 from govee_led_wez import GoveeController, GoveeColor
 
 GOVEE_MFR = [34817, 34818]
 
@@ -48,8 +49,11 @@
         await asyncio.sleep(2)
         await controller.set_color_temperature(lamp, 2000)
         # await power(DESK_STRIP, False)
 
     finally:
         await controller.async_stop()
 
+logging.basicConfig()#level=logging.DEBUG)
+logging.getLogger("govee_led_wez").setLevel(logging.DEBUG)
+
 asyncio.run(main())
```

### Comparing `govee_led_wez-0.0.8/setup.cfg` & `govee_led_wez-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/.github/workflows/python-app.yml` & `govee_led_wez-0.0.9/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/.github/workflows/python-publish.yml` & `govee_led_wez-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/govee_led_wez/ble.py` & `govee_led_wez-0.0.9/govee_led_wez/ble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import time
 from typing import Optional
 from uuid import UUID
 
 from bleak import AdvertisementData, BleakClient, BLEDevice
+from bleak_retry_connector import establish_connection
 
 from .color import GoveeColor
 from .models import BleColorMode, ModelInfo
 
 GOVEE_MFR = [34817, 34818]
 GOVEE_SVC = UUID("00010203-0405-0607-0809-0a0b0c0d1910")
 GOVEE_CHR = UUID("00010203-0405-0607-0809-0a0b0c0d2b11")
@@ -44,25 +45,29 @@
         _LOGGER.debug("Attempt to connect to %s", self.device)
 
         def disconnected(client: BleakClient):
             if self.client == client:
                 self.client = None
                 self.last_use = None
 
-        client = BleakClient(self.device, disconnected_callback=disconnected)
-
-        await client.connect()
+        client = await establish_connection(
+            BleakClient,
+            self.device,
+            name=self.device.address,
+            disconnected_callback=disconnected,
+        )
         self.client = client
         self.last_use = time.monotonic()
         return client
 
     async def write_gatt_char(self, data: bytes):
         """Write a packet to the control characteristic.
         Will attempt to obtain a client implicitly"""
         client = await self.connect()
+        _LOGGER.debug("calling write_gatt_char %s %s", self.device, data)
         await client.write_gatt_char(GOVEE_CHR, data)
 
     async def disconnect(self):
         """Disconnect the ble client, if connected"""
         if self.client:
             _LOGGER.debug("Disconnecting client from %s", self.device)
             await self.client.disconnect()
```

### Comparing `govee_led_wez-0.0.8/govee_led_wez/color.py` & `govee_led_wez-0.0.9/govee_led_wez/color.py`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/govee_led_wez/govee.py` & `govee_led_wez-0.0.9/govee_led_wez/govee.py`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/govee_led_wez/http.py` & `govee_led_wez-0.0.9/govee_led_wez/http.py`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/govee_led_wez/kelvin_rgb.py` & `govee_led_wez-0.0.9/govee_led_wez/kelvin_rgb.py`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/govee_led_wez/models.py` & `govee_led_wez-0.0.9/govee_led_wez/models.py`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/tests/test_stuff.py` & `govee_led_wez-0.0.9/tests/test_stuff.py`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/.gitignore` & `govee_led_wez-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/LICENSE` & `govee_led_wez-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/README.md` & `govee_led_wez-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `govee_led_wez-0.0.8/pyproject.toml` & `govee_led_wez-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "govee_led_wez"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Wez Furlong", email="wez@wezfurlong.org" },
 ]
 description = "Control Govee LED lights"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -12,14 +12,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "certifi>=2021.10.8",
   "aiohttp>=3.7.1",
   "bleak>=0.19.0",
+  "bleak-retry-connector>=2.8.7",
 ]
 
 [tool.pylint]
 max-line-length = 88
 disable = [
   "missing-module-docstring",
   "too-few-public-methods",
```

### Comparing `govee_led_wez-0.0.8/PKG-INFO` & `govee_led_wez-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: govee_led_wez
-Version: 0.0.8
+Version: 0.0.9
 Summary: Control Govee LED lights
 Project-URL: Homepage, https://github.com/wez/govee-py
 Project-URL: Bug Tracker, https://github.com/wez/govee-py/issues
 Author-email: Wez Furlong <wez@wezfurlong.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: aiohttp>=3.7.1
+Requires-Dist: bleak-retry-connector>=2.8.7
 Requires-Dist: bleak>=0.19.0
 Requires-Dist: certifi>=2021.10.8
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
```

