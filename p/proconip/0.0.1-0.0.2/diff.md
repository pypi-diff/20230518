# Comparing `tmp/proconip-0.0.1.tar.gz` & `tmp/proconip-0.0.2.tar.gz`

## Comparing `proconip-0.0.1.tar` & `proconip-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-0.0.1/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-0.0.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proconip-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-0.0.1/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-0.0.1/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-0.0.1/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-0.0.1/src/proconip/__init__.py
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 proconip-0.0.1/src/proconip/definitions.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 proconip-0.0.1/src/proconip/get_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-0.0.1/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-0.0.1/tests/requirements.txt
--rw-r--r--   0        0        0    12004 2020-02-02 00:00:00.000000 proconip-0.0.1/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-0.0.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-0.0.1/LICENSE
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 proconip-0.0.1/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 proconip-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-0.0.2/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-0.0.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proconip-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-0.0.2/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-0.0.2/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-0.0.2/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-0.0.2/src/proconip/__init__.py
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 proconip-0.0.2/src/proconip/api.py
+-rw-r--r--   0        0        0    21899 2020-02-02 00:00:00.000000 proconip-0.0.2/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-0.0.2/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-0.0.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 proconip-0.0.2/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 proconip-0.0.2/PKG-INFO
```

### Comparing `proconip-0.0.1/CODE_OF_CONDUCT.md` & `proconip-0.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/CONTRIBUTING.md` & `proconip-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/.github/workflows/pylint.yml` & `proconip-0.0.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/.github/workflows/python-publish.yml` & `proconip-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/.github/workflows/unittest.yml` & `proconip-0.0.2/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/src/proconip/definitions.py` & `proconip-0.0.2/src/proconip/definitions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,80 @@
 """Defines data structures for use with and used by the GetState.csv and usercfg.cgi APIs."""
 import dataclasses
 
 
+API_PATH_GET_STATE = "/GetState.csv"
+API_PATH_USRCFG = "/usrcfg.cgi"
+
+
+CATEGORY_TIME = "time"
+CATEGORY_ANALOG = "analog"
+CATEGORY_ELECTRODE = "electrode"
+CATEGORY_TEMPERATURE = "temperature"
+CATEGORY_RELAY = "relay"
+CATEGORY_DIGITAL_INPUT = "digital_input"
+CATEGORY_EXTERNAL_RELAY = "external_relay"
+CATEGORY_CANISTER = "canister"
+CATEGORY_CONSUMPTION = "consumption"
+
+
+RESET_ROOT_CAUSE = {
+    0: "n.a.",
+    1: "External reset",
+    2: "PowerUp reset",
+    4: "Brown out reset",
+    8: "Watchdog reset",
+    16: "SW reset",
+}
+
+NTP_FAULT_STATE = {
+    0: "n.a.",
+    1: "Logfile (GUI warning, green)",
+    2: "Warning (GUI warning, yellow)",
+    4: "Error (GUI warning, red)",
+    65536: "NTP available",
+}
+
+
 @dataclasses.dataclass
 class ConfigObject:
     """Configuration to be used with classes that interact with the pool controller."""
+
     def __init__(
         self,
         base_url: str,
         username: str,
         password: str,
     ):
         self.base_url = base_url
         self.username = username
         self.password = password
 
-
-CATEGORY_TIME = "time"
-CATEGORY_ANALOG = "analog"
-CATEGORY_ELECTRODE = "electrode"
-CATEGORY_TEMPERATURE = "temperature"
-CATEGORY_RELAY = "relay"
-CATEGORY_DIGITAL_INPUT = "digital_input"
-CATEGORY_EXTERNAL_RELAY = "external_relay"
-CATEGORY_CANISTER = "canister"
-CATEGORY_CONSUMPTION = "consumption"
+    @staticmethod
+    def from_dict(data: dict[str, str]):
+        """Set attributes from a dictionary."""
+        if "base_url" not in data:
+            raise ValueError("base_url is required")
+        if "username" not in data:
+            raise ValueError("username is required")
+        if "password" not in data:
+            raise ValueError("password is required")
+        return ConfigObject(data["base_url"], data["username"], data["password"])
+
+    def to_dict(self):
+        """Return a dictionary representation of the object."""
+        return {
+            "base_url": self.base_url,
+            "username": self.username,
+            "password": self.password,
+        }
 
 
 # pylint: disable=R0902
+@dataclasses.dataclass
 class DataObject:
     """Represents a single data unit combining the lines 2, 3, 4 and 5 from raw data."""
 
     _column: int
     _category: str
     _category_id: int
     _name: str
@@ -151,33 +194,55 @@
 
     @property
     def category_id(self) -> int:
         """Category ID of the data object (counts from 0 for each category)."""
         return self._category_id
 
 
-RESET_ROOT_CAUSE = {
-    0: "n.a.",
-    1: "External reset",
-    2: "PowerUp reset",
-    4: "Brown out reset",
-    8: "Watchdog reset",
-    16: "SW reset",
-}
+@dataclasses.dataclass
+class Relay(DataObject):
+    """Represents a relay."""
 
-NTP_FAULT_STATE = {
-    0: "n.a.",
-    1: "Logfile (GUI warning, green)",
-    2: "Warning (GUI warning, yellow)",
-    4: "Error (GUI warning, red)",
-    65536: "NTP available",
-}
+    def __init__(self, data_object: DataObject):
+        super().__init__(
+            data_object.column,
+            data_object.name,
+            data_object.unit,
+            data_object.offset,
+            data_object.gain,
+            data_object.value)
+
+    def __str__(self):
+        return f"{self._name}: {self._display_value}"
+
+    def is_on(self) -> bool:
+        """Returns whether the relay is on."""
+        return int(self._value) & 1 == 1
+
+    def is_off(self) -> bool:
+        """Returns whether the relay is off."""
+        return not self.is_on()
+
+    def is_manual_mode(self) -> bool:
+        """Returns whether the relay is in manual mode."""
+        return int(self._value) & 2 == 2
+
+    def is_auto_mode(self) -> bool:
+        """Returns whether the relay is in manual mode."""
+        return not self.is_manual_mode()
+
+    def get_bit_mask(self) -> int:
+        """Returns the bit mask of the relay."""
+        if self._category == CATEGORY_EXTERNAL_RELAY:
+            return 1 << (self._category_id + 8)
+        return 1 << self._category_id
 
 
 # pylint: disable=R0904
+@dataclasses.dataclass
 class GetStateData:
     """Structured representation of the data returned by the GetState.csv API."""
 
     _time: str
     _version: str
     _cpu_time: int
     _reset_root_cause: int
@@ -426,24 +491,34 @@
         return self._temperature_objects
 
     @property
     def relay_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the relay category."""
         return self._relay_objects
 
+    def relays(self) -> list[Relay]:
+        """Returns relays as a list of Relay object instances."""
+        return [Relay(relay_object) for relay_object in self._relay_objects]
+
     @property
     def digital_input_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the digital input category."""
         return self._digital_objects
 
     @property
     def external_relay_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the external relay category."""
         return self._external_relay_objects
 
+    def external_relays(self) -> list[Relay]:
+        """Returns external relays as a list of Relay object instances."""
+        return [
+            Relay(external_relay_object) for external_relay_object in self._external_relay_objects
+        ]
+
     @property
     def canister_objects(self) -> list[DataObject]:
         """Returns a list of DataObjects of the canister category."""
         return self._canister_objects
 
     @property
     def consumption_objects(self) -> list[DataObject]:
@@ -505,7 +580,26 @@
         """Returns the DataObject of the pH minus dosage relay."""
         return self.aggregated_relay_objects[self._ph_minus_dosage_relay_id]
 
     @property
     def ph_plus_dosage_relay(self) -> DataObject:
         """Returns the DataObject of the pH plus dosage relay."""
         return self.aggregated_relay_objects[self._ph_plus_dosage_relay_id]
+
+    def get_relay(self, relay_id: int) -> Relay:
+        """Returns the Relay instance for the given id."""
+        return Relay(self.aggregated_relay_objects[relay_id])
+
+    def determine_overall_relay_bit_state(self) -> [int, int]:
+        """Determine the overall relay bit state from the current state."""
+        relays = self.relays()
+        bit_state = [255, 0]
+        if self.is_relay_extension_enabled():
+            relays.extend(self.external_relays())
+            bit_state[0] = 65535
+        for relay in relays:
+            relay_bit_mask = relay.get_bit_mask()
+            if relay.is_on():
+                bit_state[1] |= relay_bit_mask
+            else:
+                bit_state[0] &= ~relay_bit_mask
+        return bit_state
```

### Comparing `proconip-0.0.1/tests/helper.py` & `proconip-0.0.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/tests/test_definitions.py` & `proconip-0.0.2/tests/test_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Testing data structures and helper classes from definitions module."""
+
 import unittest
 
 from proconip.definitions import (
     ConfigObject,
     GetStateData,
     CATEGORY_ANALOG,
     CATEGORY_ELECTRODE,
     CATEGORY_TEMPERATURE,
     CATEGORY_RELAY,
     CATEGORY_DIGITAL_INPUT,
     CATEGORY_EXTERNAL_RELAY,
     CATEGORY_CANISTER,
     CATEGORY_CONSUMPTION,
 )
+
 from .helper import (
     BASE_URL,
     GET_STATE_CSV,
     USERNAME,
     PASSWORD,
 )
```

### Comparing `proconip-0.0.1/.gitignore` & `proconip-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/LICENSE` & `proconip-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-0.0.1/pyproject.toml` & `proconip-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-0.0.1/PKG-INFO` & `proconip-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,89 @@
-Metadata-Version: 2.1
-Name: proconip
-Version: 0.0.1
-Summary: Library for basic interaction with the Procon.IP pool controller unit.
-Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
-Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
-Author-email: Yannic Labonte <yannic.labonte@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Python package for the ProCon.IP Pool Controller
 
+[![Pylint](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml)
+[![Unittest](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml)
+
+[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;width: 144px !important;" >](https://www.buymeacoffee.com/ylabonte)
+
 ## Overview
 
 * [Introduction (_What is this library for?_)](#introduction)
+* [Installation](#installation)
+* [Usage](#usage)
 * [A brief description of the ProCon.IP pool controller](#a-brief-description-of-the-proconip-pool-controller)
 * [Disclaimer](#disclaimer)
 
+
 ---
 
 ## Introduction
 
-The name of this library refers to the [ProCon.IP pool controller](#what-is-procon-ip).
+The name of this library refers to the [ProCon.IP pool controller](#a-brief-description-of-the-proconip-pool-controller).
 It is somehow a port of my [procon-ip](https://github.com/ylabonte/procon-ip) 
 TypeScript library (available as [NPM Package](https://www.npmjs.com/package/procon-ip)). 
 As the TypeScript library was a byproduct of my ioBroker adapter for the pool 
 controller unit, this library is primary intended for the implementation of a 
 Home Assistant integration.
 
 Documentation might follow. Until this please take a look at the sources. I
 tried to keep it simple and readable. An IDE with proper auto-completion should
 help understand and use the library without further documentation.
 
 Feel free to ask questions by using github's issues system, so others can take
 advantage, contribute and are able to find the answer if they have a similar 
 question. Thanks! :)
 
+## Installation
+
+This library is available on [PyPI](https://pypi.org/project/proconip/). So you 
+can easily install it with pip:
+```bash
+pip install proconip
+```
+or
+```bash
+python -m pip install proconip
+```
+In both cases you can add `--upgrade` to update to the latest version.
+
+## Usage
+
+```python
+import asyncio
+import aiohttp
+from proconip.definitions import ConfigObject
+from proconip.api import GetState
+
+
+async def testrun():
+    client_session = aiohttp.ClientSession()
+    config = ConfigObject("http://192.168.2.3", "admin", "admin")
+    controller = GetState(client_session, config)
+    data = await controller.structured()
+    print(data.redox_electrode.display_value)
+    print(data.ph_electrode.display_value)
+    print(data.temperature_objects[0].display_value)
+    await client_session.close()
+
+
+asyncio.run(testrun())
+
+```
+
 ## A brief description of the ProCon.IP pool controller
 
 ![Picture from pooldigital.de](https://www.pooldigital.de/shop/media/image/66/47/a5/ProConIP1_720x600.png)
 
 The ProCon.IP pool controller is a low budget network attached control unit for
 home swimming pools. With its software switched relays, it can control
 multiple pumps (for the pool filter and different dosage aspects) either
 simply planned per time schedule or depending on a reading/value from one of
 its many input channels for measurements (eg. i/o flow sensors, Dallas 1-Wire
-termometers, redox and pH electrodes). At least there is also the option to
+thermometers, redox and pH electrodes). At least there is also the option to
 switch these relays on demand, which makes them also applicable for switching
 lights (or anything else you want) on/off.
 Not all of its functionality is reachable via API. In fact there is one
 documented API for reading (polling) values as CSV (`/GetState.csv`). In my
 memories there was another one for switching the relays on/off and on with
 timer. But I cannot find the second one anymore. So not even pretty, but
 functional: The ProCon.IP has two native web interfaces, which can be
```

