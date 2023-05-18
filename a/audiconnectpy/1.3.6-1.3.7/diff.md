# Comparing `tmp/audiconnectpy-1.3.6.tar.gz` & `tmp/audiconnectpy-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.6.tar", last modified: Wed May 17 11:48:11 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.7.tar", last modified: Thu May 18 12:35:08 2023, max compression
```

## Comparing `audiconnectpy-1.3.6.tar` & `audiconnectpy-1.3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:48:11.931547 audiconnectpy-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-17 11:48:11.931547 audiconnectpy-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:48:11.931547 audiconnectpy-1.3.6/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28101 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:48:11.931547 audiconnectpy-1.3.6/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-17 11:48:11.000000 audiconnectpy-1.3.6/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-17 11:48:11.000000 audiconnectpy-1.3.6/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:48:11.000000 audiconnectpy-1.3.6/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:48:11.000000 audiconnectpy-1.3.6/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 11:48:11.000000 audiconnectpy-1.3.6/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:48:11.931547 audiconnectpy-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-17 11:48:11.000000 audiconnectpy-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:48:11.931547 audiconnectpy-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 11:48:02.000000 audiconnectpy-1.3.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29017 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32808 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.6/LICENSE` & `audiconnectpy-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.6/PKG-INFO` & `audiconnectpy-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.6
+Version: 1.3.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.6/README.md` & `audiconnectpy-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.6/audiconnectpy/api.py` & `audiconnectpy-1.3.7/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.6/audiconnectpy/auth.py` & `audiconnectpy-1.3.7/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.6/audiconnectpy/helpers.py` & `audiconnectpy-1.3.7/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.6/audiconnectpy/models.py` & `audiconnectpy-1.3.7/audiconnectpy/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,103 +267,120 @@
     """Preheater class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
+        if not isinstance(self.data, ExtendedDict):
+            _LOGGER.warning("Preheater format is incorrect %s", self.data)  # type: ignore
         return self.data.getr("statusResponse.climatisationStateReport") is not None
 
     @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
-        report = self.data.getr("statusResponse.climatisationStateReport", {})
-        attrs = {
-            "preheater_state": report,
-            "preheater_active": report.get("climatisationState"),
-            "preheater_duration": report.get("climatisationDuration"),
-            "preheater_remaining": report.get("remainingClimateTime"),
-        }
+        attrs: dict[str, Any] = {}
+        if isinstance(self.data, ExtendedDict):
+            report: ExtendedDict = self.data.getr(
+                "statusResponse.climatisationStateReport", {}
+            )
+            attrs = {
+                "preheater_state": report,
+                "preheater_active": report.get("climatisationState"),
+                "preheater_duration": report.get("climatisationDuration"),
+                "preheater_remaining": report.get("remainingClimateTime"),
+            }
         return attrs
 
 
 @dataclass
 class ChargerDataResponse:
     """Charger class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
+        if not isinstance(self.data, ExtendedDict):
+            _LOGGER.warning("Charger format is incorrect %s", self.data)  # type: ignore
         return (
             self.data.getr("charger.settings") is not None
             or self.data.getr("charger.status") is not None
         )
 
     @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
-        settings = self.data.getr("charger.settings", {})
-        status = self.data.getr("charger.status", {})
-        charging = status.get("chargingStatusData", {})
-        cruising = status.get("cruisingRangeStatusData", {})
-        attrs = {
-            "max_charge_current": settings.getr("maxChargeCurrent.content"),
-            "charging_state": charging.getr("chargingState.content"),
-            "actual_charge_rate": charging.getr("actualChargeRate.content"),
-            "actual_charge_rate_unit": charging.getr("chargeRateUnit.content"),
-            "charging_power": charging.getr("chargingPower.content"),
-            "charging_mode": charging.getr("chargingMode.content"),
-            "energy_flow": charging.getr("energyFlow.content"),
-            "primary_engine_type": cruising.getr("engineTypeFirstEngine.content"),
-            "secondary_engine_type": cruising.getr("engineTypeSecondEngine.content"),
-            "hybrid_range": cruising.getr("hybridRange.content"),
-            "primary_engine_range": cruising.getr("primaryEngineRange.content"),
-            "secondary_engine_range": cruising.getr("secondaryEngineRange.content"),
-            "state_of_charge": status.getr("batteryStatusData.stateOfCharge.content"),
-            "plug_state": status.getr("plugStatusData.plugState.content"),
-            "plug_lock": status.getr("plugStatusData.lockState.content"),
-            "remaining_charging_time": status.getr(
-                "batteryStatusData.remainingChargingTime.content"
-            ),
-        }
+        attrs = {}
+        if isinstance(self.data, ExtendedDict):
+            settings = self.data.getr("charger.settings", {})
+            status = self.data.getr("charger.status", {})
+            charging = status.get("chargingStatusData", {})
+            cruising = status.get("cruisingRangeStatusData", {})
+            attrs = {
+                "max_charge_current": settings.getr("maxChargeCurrent.content"),
+                "charging_state": charging.getr("chargingState.content"),
+                "actual_charge_rate": charging.getr("actualChargeRate.content"),
+                "actual_charge_rate_unit": charging.getr("chargeRateUnit.content"),
+                "charging_power": charging.getr("chargingPower.content"),
+                "charging_mode": charging.getr("chargingMode.content"),
+                "energy_flow": charging.getr("energyFlow.content"),
+                "primary_engine_type": cruising.getr("engineTypeFirstEngine.content"),
+                "secondary_engine_type": cruising.getr(
+                    "engineTypeSecondEngine.content"
+                ),
+                "hybrid_range": cruising.getr("hybridRange.content"),
+                "primary_engine_range": cruising.getr("primaryEngineRange.content"),
+                "secondary_engine_range": cruising.getr("secondaryEngineRange.content"),
+                "state_of_charge": status.getr(
+                    "batteryStatusData.stateOfCharge.content"
+                ),
+                "plug_state": status.getr("plugStatusData.plugState.content"),
+                "plug_lock": status.getr("plugStatusData.lockState.content"),
+                "remaining_charging_time": status.getr(
+                    "batteryStatusData.remainingChargingTime.content"
+                ),
+            }
         return attrs
 
 
 @dataclass
 class ClimaterDataResponse:
     """Climater class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
+        if not isinstance(self.data, ExtendedDict):
+            _LOGGER.warning("Climater format is incorrect %s", self.data)  # type: ignore
         return (
             self.data.getr("climater.settings") is not None
             or self.data.getr("climater.status") is not None
         )
 
     @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
         attrs = {}
-        settings = self.data.getr("climater.settings")
-        status = self.data.getr("climater.status")
-        attrs = {
-            "climatisation_state": status.getr(
-                "climatisationStatusData.climatisationState.content"
-            ),
-            "outdoor_temperature": status.getr(
-                "temperatureStatusData.outdoorTemperature.content"
-            ),
-            "climatisation_heater_src": settings.getr("heaterSource.content"),
-            "climatisation_target_temp": settings.getr("targetTemperature.content"),
-        }
+        if isinstance(self.data, ExtendedDict):
+            settings = self.data.getr("climater.settings")
+            status = self.data.getr("climater.status")
+            attrs = {
+                "climatisation_state": status.getr(
+                    "climatisationStatusData.climatisationState.content"
+                ),
+                "outdoor_temperature": status.getr(
+                    "temperatureStatusData.outdoorTemperature.content"
+                ),
+                "climatisation_heater_src": settings.getr("heaterSource.content"),
+                "climatisation_target_temp": settings.getr("targetTemperature.content"),
+            }
         return attrs
 
 
 @dataclass
 class DestinationDataResponse:
     """Destination."""
```

### Comparing `audiconnectpy-1.3.6/audiconnectpy/services.py` & `audiconnectpy-1.3.7/audiconnectpy/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,35 +50,41 @@
 
     async def async_get_vehicles(self) -> Any:
         """Get all vehicles."""
         url = await self._async_get_home_region("")
         data = await self._auth.get(
             f"{url}/usermanagement/users/v1/{self.brand}/{self.country}/vehicles"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_vehicle_details(self, vin: str) -> Any:
         """Get vehicle data."""
         url = await self._async_get_home_region(vin.upper())
         accept = {
             "Accept": "application/vnd.vwg.mbb.vehicleDataDetail_v2_1_0+json, application/vnd.vwg.mbb.genericError_v1_0_2+json"
         }
         headers = await self._auth.async_get_headers(token_type="mbb", headers=accept)
         data = await self._auth.get(
             f"{url}/vehicleMgmt/vehicledata/v2/{self.brand}/{self.country}/vehicles/{vin.upper()}/",
             headers=headers,
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_vehicle(self, vin: str) -> VehicleDataResponse:
         """Get store data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_refresh_vehicle_data(self, vin: str) -> None:
         """Refresh vehicle data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.post(
             f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests"
@@ -94,44 +100,52 @@
 
     async def async_get_stored_position(self, vin: str) -> PositionDataResponse:
         """Get position data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return PositionDataResponse(data)
 
     async def async_get_destinations(self, vin: str) -> DestinationDataResponse:
         """Get destination data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/destinationfeedservice/mydestinations/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/destinations"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return DestinationDataResponse(data)
 
     async def async_get_history(self, vin: str) -> HistoryDataResponse:
         """Get history data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/dwap/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/history"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return HistoryDataResponse(data)
 
     async def async_get_vehicule_users(self, vin: str) -> UsersDataResponse:
         """Get ufers of vehicle."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(f"{url}/bs/uic/v1/{vin.upper()}/users")
         return UsersDataResponse(data)
 
     async def async_get_charger(self, vin: str) -> ChargerDataResponse:
         """Get charger data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return ChargerDataResponse(data)
 
     async def async_get_tripdata(
         self, vin: str, kind: Literal["short", "long", "cyclic"]
     ) -> tuple[TripDataResponse, TripDataResponse]:
         """Get trip data."""
         if kind not in ["short", "long", "cyclic"]:
@@ -146,14 +160,16 @@
                 "%Y-%m-%dT%H:%M:%SZ"
             ),
         }
         data = await self._auth.get(
             f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{kind}",
             params=params,
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         td_sorted = sorted(
             data.getr("tripDataList.tripData"),
             key=lambda k: k["overallMileage"],  # type: ignore[no-any-return]
             reverse=True,
         )
         td_current = td_sorted[0]
         td_reset_trip = {}
@@ -171,47 +187,57 @@
 
     async def async_get_operations_list(self, vin: str) -> Any:
         """Get operation data."""
         url = await self._async_get_home_region_setter(vin.upper())
         data = await self._auth.get(
             f"{url}/rolesrights/operationlist/v3/vehicles/{vin.upper()}"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_climater(self, vin: str) -> ClimaterDataResponse:
         """Get climater data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return ClimaterDataResponse(data)
 
     async def async_get_preheater(self, vin: str) -> PreheaterDataResponse:
         """Get Heater/Ventilation data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return PreheaterDataResponse(data)
 
     async def async_get_climater_timer(self, vin: str) -> Any:
         """Get timer."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/departuretimer/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/timer"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_capabilities(self, vin: str) -> VehicleDataResponse:
         """Get capabilities."""
         url = "https://emea.bff.cariad.digital"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(
             f"{url}/vehicle/v1/vehicles/{vin.upper()}/capabilities", headers=headers
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_get_vehicle_information(self) -> Any:
         """Get vehicle information."""
         headers = await self._auth.async_get_headers(
             token_type="audi",
             headers={
@@ -235,42 +261,52 @@
 
     async def async_get_honkflash(self, vin: str) -> Any:
         """Get Honk & Flash status."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/rhf/v1/{self.brand}/{self.country}/configuration"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_personal_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/personalData", headers=headers)
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_real_car_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/realCarData", headers=headers)
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_mbb_status(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/mbbStatusData", headers=headers)
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_identity_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/identityData", headers=headers)
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     # async def async_get_users(self, vin: str) -> Any:
     #     """Get users."""
     #     url = "https://userinformationservice.apps.emea.vwapps.io/iaa"
     #     headers = await self._auth.async_get_headers(token_type="idk")
     #     data = await self._auth.get(f"{url}/uic/v1/vin/{vin.upper()}/users", headers=headers)
@@ -278,38 +314,46 @@
 
     async def async_get_fences(self, vin: str) -> Any:
         """Get fences."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingAlerts"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_fences_config(self, vin: str) -> Any:
         """Get fences configuration."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingConfiguration"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_speed_alert(self, vin: str) -> Any:
         """Get speed alert."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlerts"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_get_speed_config(self, vin: str) -> Any:
         """Get speed alert configuration."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlertConfiguration"
         )
+        if not isinstance(data, ExtendedDict):
+            _LOGGER.warning("Format is incorrect %s", data)
         return data
 
     async def async_lock(self, vin: str, lock: bool) -> None:
         """Set lock."""
         # OpenHab "lock","unlock"
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
```

### Comparing `audiconnectpy-1.3.6/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.7/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.6
+Version: 1.3.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.6/pyproject.toml` & `audiconnectpy-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.6/setup.py` & `audiconnectpy-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.6",
+    version="1.3.7",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

