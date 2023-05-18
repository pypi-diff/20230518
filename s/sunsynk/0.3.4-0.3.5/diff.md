# Comparing `tmp/sunsynk-0.3.4.tar.gz` & `tmp/sunsynk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.4.tar", last modified: Fri May  5 11:04:19 2023, max compression
+gzip compressed data, was "sunsynk-0.3.5.tar", last modified: Thu May 18 10:27:12 2023, max compression
```

## Comparing `sunsynk-0.3.4.tar` & `sunsynk-0.3.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.860590 sunsynk-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 11:04:11.000000 sunsynk-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 11:04:11.000000 sunsynk-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-05 11:04:19.860590 sunsynk-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-05 11:04:11.000000 sunsynk-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 11:04:19.860590 sunsynk-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:04:11.000000 sunsynk-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.856590 sunsynk-0.3.4/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12100 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8030 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.856590 sunsynk-0.3.4/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.856590 sunsynk-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass-addon-sunsynk-dev.zip
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.860590 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.860590 sunsynk-0.3.4/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_pysunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 10:27:02.000000 sunsynk-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 10:27:02.000000 sunsynk-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-18 10:27:12.956032 sunsynk-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-18 10:27:02.000000 sunsynk-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 10:27:12.956032 sunsynk-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 10:27:02.000000 sunsynk-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11686 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8030 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-18 10:27:02.000000 sunsynk-0.3.5/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:27:12.000000 sunsynk-0.3.5/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass-addon-sunsynk-dev.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:12.952032 sunsynk-0.3.5/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_pysunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-18 10:27:02.000000 sunsynk-0.3.5/tests/sunsynk/test_usunsynk.py
```

### Comparing `sunsynk-0.3.4/LICENSE` & `sunsynk-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/PKG-INFO` & `sunsynk-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.4/README.md` & `sunsynk-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/setup.cfg` & `sunsynk-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk/definitions.py` & `sunsynk-0.3.5/sunsynk/definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,119 +1,124 @@
 """Sunsynk 5kW&8kW hybrid inverter sensor definitions."""
 from sunsynk import AMPS, CELSIUS, KWH, VOLT, WATT
 from sunsynk.rwsensors import (
     NumberRWSensor,
     SelectRWSensor,
+    SwitchRWSensor,
     SystemTimeRWSensor,
     TimeRWSensor,
 )
 from sunsynk.sensors import (
+    BinarySensor,
     FaultSensor,
     InverterStateSensor,
     MathSensor,
     SDStatusSensor,
     Sensor,
     SensorDefinitions,
     SerialSensor,
     TempSensor,
 )
 
-SENSORS = SensorDefinitions()
+SENSORS: SensorDefinitions = SensorDefinitions()
 
 ##########
 # Battery
 ##########
 SENSORS += (
     TempSensor(182, "Battery temperature", CELSIUS, 0.1),
     Sensor(183, "Battery voltage", VOLT, 0.01),
     Sensor(184, "Battery SOC", "%"),
     Sensor(190, "Battery power", WATT, -1),
     Sensor(191, "Battery current", AMPS, -0.01),
 )
 
-#################
-# Inverter Power
-#################
+###########
+# Inverter
+###########
 SENSORS += (
     Sensor(175, "Inverter power", WATT, -1),
     Sensor(154, "Inverter voltage", VOLT, 0.1),
+    Sensor(164, "Inverter current", AMPS, 0.01),
     Sensor(193, "Inverter frequency", "Hz", 0.01),
 )
 
-#############
-# Grid Power
-#############
+#######
+# Grid
+#######
 SENSORS += (
     Sensor(79, "Grid frequency", "Hz", 0.01),
     Sensor(169, "Grid power", WATT, -1),  # L1(167) + L2(168)
     Sensor(167, "Grid LD power", WATT, -1),  # L1 seems to be LD
     Sensor(168, "Grid L2 power", WATT, -1),
     Sensor(150, "Grid voltage", VOLT, 0.1),
     MathSensor((160, 161), "Grid current", AMPS, factors=(0.01, 0.01)),
     Sensor(172, "Grid CT power", WATT, -1),
 )
-# LD power?
 
-#############
-# Load Power
-#############
+#######
+# Load
+#######
 SENSORS += (
     Sensor(178, "Load power", WATT, -1),  # L1(176) + L2(177)
     Sensor(176, "Load L1 power", WATT, -1),
     Sensor(177, "Load L2 power", WATT, -1),
 )
 
-################
-# Solar Power 1
-################
+#############
+# Solar PV 1
+#############
 SENSORS += (
     Sensor(186, "PV1 power", WATT, -1),
     Sensor(109, "PV1 voltage", VOLT, 0.1),
     Sensor(110, "PV1 current", AMPS, 0.1),
 )
 
-################
-# Solar Power 2
-################
+#############
+# Solar PV 2
+#############
 SENSORS += (
     Sensor(187, "PV2 power", WATT, -1),
     Sensor(111, "PV2 voltage", VOLT, 0.1),
     Sensor(112, "PV2 current", AMPS, 0.1),
 )
 
 ###################
 # Power on Outputs
 ###################
 SENSORS += (
     Sensor(166, "AUX power", WATT, -1),
-    # https://github.com/kellerza/sunsynk/issues/75
-    #  https://powerforum.co.za/topic/8646-my-sunsynk-8kw-data-collection-setup/?do=findComment&comment=147591
+    # Essential power
+    # - https://powerforum.co.za/topic/8646-my-sunsynk-8kw-data-collection-setup/?do=findComment&comment=147591
+    # Essential 1 power
+    # - dev & normal version, see https://github.com/kellerza/sunsynk/issues/134
+    # Essential 2 power
+    # - early-2023 see https://github.com/kellerza/sunsynk/issues/75
+    MathSensor((175, 169, 166), "Essential power", WATT, factors=(1, 1, -1)),
+    MathSensor((175, 167, 166), "Essential 1 power", WATT, factors=(1, 1, -1)),
     MathSensor(
-        (175, 169, 166), "Essential power", WATT, factors=(1, 1, -1), absolute=True
+        (175, 169, 166), "Essential 2 power", WATT, factors=(1, 1, -1), absolute=True
     ),
-    # MathSensor((175, 167, 166), "Essential power", WATT, factors=(1, 1, -1)),
     MathSensor(
         (172, 167), "Non-Essential power", WATT, factors=(1, -1), no_negative=True
     ),
 )
 
-###################
+#########
 # Energy
-###################
+#########
 SENSORS += (
     Sensor(60, "Day Active Energy", KWH, -0.1),
     Sensor(70, "Day Battery Charge", KWH, 0.1),
     Sensor(71, "Day Battery Discharge", KWH, 0.1),
-    Sensor(77, "Day Grid Export", KWH, 0.1),
     Sensor(76, "Day Grid Import", KWH, 0.1),
-    # Sensor(200, "Day Load Power", KWH, 0.01),
+    Sensor(77, "Day Grid Export", KWH, 0.1),
     Sensor(84, "Day Load Energy", KWH, 0.1),
     Sensor(108, "Day PV Energy", KWH, 0.1),
     Sensor(61, "Day Reactive Energy", "kVarh", -0.1),
-    # Sensor((201, 202), "History Load Power", KWH, 0.1),
     Sensor(67, "Month Grid Energy", KWH, 0.1),
     Sensor(66, "Month Load Energy", KWH, 0.1),
     Sensor(65, "Month PV Energy", KWH, 0.1),
     Sensor((63, 64), "Total Active Energy", KWH, 0.1),  # signed?
     Sensor((72, 73), "Total Battery Charge", KWH, 0.1),
     Sensor((74, 75), "Total Battery Discharge", KWH, 0.1),
     Sensor((81, 82), "Total Grid Export", KWH, 0.1),
@@ -135,23 +140,27 @@
     Sensor(0, "Device Type"),
     FaultSensor((103, 104, 105, 106), "Fault"),
     InverterStateSensor(59, "Overall state"),
     SDStatusSensor(92, "SD Status", ""),  # type: ignore
     TempSensor(90, "DC transformer temperature", CELSIUS, 0.1),
     TempSensor(95, "Environment temperature", CELSIUS, 0.1),
     TempSensor(91, "Radiator temperature", CELSIUS, 0.1),
-    Sensor(194, "Grid Connected Status"),
+    Sensor(194, "Grid Connected Status"),  # Remove in the future?
+    BinarySensor(194, "Grid Connected"),
     SystemTimeRWSensor((22, 23, 24), "Date Time", unit=""),
 )
 ###########
 # Settings
 ###########
 SENSORS += (
     Sensor(200, "Control Mode"),
     Sensor(232, "Grid Charge enabled", "", -1),
+    SelectRWSensor(
+        235, "Generator input", "", options={0: "Disable", 1: "Output", 2: "Input"}
+    ),
     Sensor(312, "Battery charging voltage", VOLT, 0.01),
     Sensor(603, "Bat1 SOC", "%"),
     Sensor(611, "Bat1 Cycle"),
 )
 
 # Battery capacity (if managed by BMS)
 BATTERY_LOW_CAP = NumberRWSensor(219, "Battery Low Capacity", "%", max=50)
@@ -200,22 +209,22 @@
     BATTERY_RESTART_VOLT,
     BATTERY_LOW_VOLT,
 )
 
 #################
 # System program
 #################
-SENSORS += SelectRWSensor(
-    243, "Priority Mode", options={0: "Battery first", 1: "Load first"}
-)
-
-SENSORS += SelectRWSensor(
-    244,
-    "Load Limit",
-    options={0: "Allow Export", 1: "Essentials", 2: "Zero Export"},
+SENSORS += (
+    SelectRWSensor(243, "Priority Mode", options={0: "Battery first", 1: "Load first"}),
+    SelectRWSensor(
+        244,
+        "Load Limit",
+        options={0: "Allow Export", 1: "Essentials", 2: "Zero Export"},
+    ),
+    SwitchRWSensor(248, "Use Timer", on=1, bitmask=1),
 )
 
 PROG1_TIME = TimeRWSensor(250, "Prog1 Time")
 PROG2_TIME = TimeRWSensor(251, "Prog2 Time", min=PROG1_TIME)
 PROG3_TIME = TimeRWSensor(252, "Prog3 Time", min=PROG2_TIME)
 PROG4_TIME = TimeRWSensor(253, "Prog4 Time", min=PROG3_TIME)
 PROG5_TIME = TimeRWSensor(254, "Prog5 Time", min=PROG4_TIME)
@@ -301,43 +310,35 @@
 SENSORS += NumberRWSensor(210, "Battery Max Charge current", AMPS, min=0, max=185)
 SENSORS += NumberRWSensor(211, "Battery Max Discharge current", AMPS, min=0, max=185)
 
 
 #############
 # Deprecated
 #############
-def _deprecated() -> None:
-    """Populate the deprecated sensors."""
-    dep_map: dict[str, Sensor] = {
-        "aux_power": Sensor(166, "AUX load", WATT, -1),
-        "battery_temperature": TempSensor(182, "Temp Battery", CELSIUS, 0.1),
-        "dc_transformer_temperature": TempSensor(
-            90, "Temp DC transformer", CELSIUS, 0.1
-        ),
-        "environment_temperature": TempSensor(95, "Temp Environment", CELSIUS, 0.1),
-        "grid_charge_battery_current": Sensor(230, "Battery Grid Charge", AMPS, -1),
-        "grid_ct_power": Sensor(172, "Grid CT load", WATT, -1),
-        "grid_l2_power": Sensor(168, "Grid L2 load", WATT, -1),
-        "grid_ld_power": Sensor(167, "Grid L1 load", WATT, -1),
-        "grid_power": Sensor(169, "Grid load", WATT, -1),
-        "inverter_power": Sensor(175, "Inverter Output", WATT, -1),
-        "radiator_temperature": TempSensor(91, "Temp Radiator", CELSIUS, 0.1),
-        "day_active_energy": Sensor(60, "Day Active Power", KWH, -0.1),
-        "day_reactive_energy": Sensor(61, "Day Reactive Power", "kVarh", -0.1),
-        "total_active_energy": Sensor((63, 64), "Total Active Power", KWH, 0.1),
-        "month_pv_energy": Sensor(65, "Month PV Power", KWH),
-        "month_load_energy": Sensor(66, "Month Load Power", KWH),
-        "month_grid_energy": Sensor(67, "Month Grid Power", KWH),
-        "year_pv_energy": Sensor((68, 69), "Year PV Power", KWH, 0.1),
-        "day_load_energy": Sensor(84, "Day Load Power", KWH, 0.1),
-        "total_load_energy": Sensor((85, 86), "Total Load Power", KWH, 0.1),
-        "year_load_energy": Sensor((87, 88), "Year Load Power", KWH, 0.1),
-        "total_pv_energy": Sensor((96, 97), "Total PV Power", KWH, 0.1),
-        "battery_equalization_voltage": Sensor(201, "Equalization voltage", VOLT, 0.01),
-        "battery_absorption_voltage": Sensor(202, "Absorption voltage", VOLT, 0.01),
+SENSORS.deprecated.update(
+    {
+        "aux_load": "aux_power",
+        "temp_battery": "battery_temperature",
+        "temp_dc_transformer": "dc_transformer_temperature",
+        "temp_environment": "environment_temperature",
+        "battery_grid_charge": "grid_charge_battery_current",
+        "grid_ct_load": "grid_ct_power",
+        "grid_l1_load": "grid_ld_power",
+        "grid_l2_load": "grid_l2_power",
+        "grid_load": "grid_power",
+        "inverter_output": "inverter_power",
+        "temp_radiator": "radiator_temperature",
+        "day_active_power": "day_active_energy",
+        "day_reactive_power": "day_reactive_energy",
+        "total_active_power": "total_active_energy",
+        "month_pv_power": "month_pv_energy",
+        "month_load_power": "month_load_energy",
+        "month_grid_power": "month_grid_energy",
+        "year_pv_power": "year_pv_energy",
+        "day_load_power": "day_load_energy",
+        "total_load_power": "total_load_energy",
+        "year_load_power": "year_load_energy",
+        "total_pv_power": "total_pv_energy",
+        "equalization_voltage": "battery_equalization_voltage",
+        "absorption_voltage": "battery_absorption_voltage",
     }
-
-    for newname, sen in dep_map.items():
-        SENSORS.deprecated[sen.id] = SENSORS.all[newname]
-
-
-_deprecated()
+)
```

### Comparing `sunsynk-0.3.4/sunsynk/definitions3ph.py` & `sunsynk-0.3.5/sunsynk/definitions3ph.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk/pysunsynk.py` & `sunsynk-0.3.5/sunsynk/pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk/rwsensors.py` & `sunsynk-0.3.5/sunsynk/rwsensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk/sensors.py` & `sunsynk-0.3.5/sunsynk/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Sensor classes represent modbus registers for an inverter."""
 from __future__ import annotations
 
 import logging
-from typing import Union
+from typing import Optional, Union
 
 import attrs
 
 from sunsynk.helpers import (
     NumType,
     RegType,
     ValType,
@@ -15,15 +15,15 @@
     signed,
     slug,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@attrs.define(slots=True)
+@attrs.define(slots=True, eq=False)
 class Sensor:
     """Sunsynk sensor."""
 
     # pylint: disable=too-many-instance-attributes
     address: RegType = attrs.field(converter=ensure_tuple)
     name: str = attrs.field()
     unit: str = attrs.field(default="")
@@ -60,20 +60,38 @@
     def __eq__(self, other: object) -> bool:
         """Sensor equality is based on the ID only."""
         if not isinstance(other, Sensor):
             raise TypeError(str(type(other)))
         return self.id == other.id
 
 
+@attrs.define(slots=True, eq=False)
+class BinarySensor(Sensor):
+    """Binary sensor."""
+
+    off: Optional[int] = attrs.field(default=None)
+    on: Optional[int] = attrs.field(default=None)  # pylint: disable=invalid-name
+
+    def reg_to_value(self, regs: RegType) -> ValType:
+        """Reg to value for binary."""
+        res = super().reg_to_value(regs)
+        if self.on is not None:
+            return res == self.on
+        if self.off is not None:
+            return res != self.off
+        return bool(res)
+
+
 @attrs.define(slots=True)
 class SensorDefinitions:
     """Definitions."""
 
     all: dict[str, Sensor] = attrs.field(factory=dict)
-    deprecated: dict[str, Sensor] = attrs.field(factory=dict)
+    deprecated: dict[str, str] = attrs.field(factory=dict)
+    """map of 'old_name': 'new_name'"""
 
     @property
     def serial(self) -> Sensor:
         """Get the serial sensor."""
         return self.all["serial"]
 
     @property
```

### Comparing `sunsynk-0.3.4/sunsynk/state.py` & `sunsynk-0.3.5/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk/sunsynk.py` & `sunsynk-0.3.5/sunsynk/sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk/usunsynk.py` & `sunsynk-0.3.5/sunsynk/usunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/sunsynk.egg-info/PKG-INFO` & `sunsynk-0.3.5/sunsynk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.4/sunsynk.egg-info/SOURCES.txt` & `sunsynk-0.3.5/sunsynk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/conftest.py` & `sunsynk-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.3.5/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/hass-addon-sunsynk.zip` & `sunsynk-0.3.5/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_filter.py` & `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_filter.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_run.py` & `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_run.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_sensors.py` & `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_state.py` & `sunsynk-0.3.5/tests/hass_addon_sunsynk_multi/test_state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_helpers.py` & `sunsynk-0.3.5/tests/sunsynk/test_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 """Test helpers."""
 from sunsynk.helpers import (
     SSTime,
+    as_num,
     ensure_tuple,
     int_round,
     patch_bitmask,
     signed,
-    simple_eval,
 )
 from sunsynk.sensors import Sensor
 
 
-def test_int_round() -> None:
-    res1 = int_round(1.0)
-    assert isinstance(res1, int)
-    assert res1 == 1
+def test_as_num(caplog) -> None:
+    assert as_num(None) == 0
+    assert as_num(1.0) == 1.0
+    assert as_num(1) == 1
+    assert as_num("1") == 1
+    assert as_num("1.5") == 1.5
+    caplog.clear()
+    assert as_num("1.0x") == 0
+    assert "could not convert string to float: '1.0x'" in caplog.text
 
 
 def test_ensure_tuple() -> None:
     assert ensure_tuple(1) == (1,)
     assert ensure_tuple((1,)) == (1,)
     assert ensure_tuple((1, 5)) == (1, 5)
     assert ensure_tuple("a") == ("a",)
 
 
+def test_int_round() -> None:
+    res1 = int_round(1.0)
+    assert isinstance(res1, int)
+    assert res1 == 1
+
+
 def test_signed() -> None:
     assert signed(0x7FFF) == 0x7FFF
     assert signed(0xFFFF) == 0
 
 
 def test_signeds() -> None:
     """Signed sensors have a -1 factor"""
@@ -74,25 +85,7 @@
 def test_patch_bitmask() -> None:
     assert patch_bitmask(2, 1, 1) == 3
     assert patch_bitmask(1, 2, 2) == 3
 
     assert patch_bitmask(0xFFF, 0, 1) == 0xFFE
     assert patch_bitmask(0xFFFF, 0, 1) == 0xFFFE
     assert patch_bitmask(0xFFF, 0, 2) == 0xFFD
-
-
-def test_math() -> None:
-    for expr, res in (
-        ("2^4", 6),
-        ("2**4", 16),
-        ("1 + 2*3**(4^5) / (6 + -7)", -5.0),
-        ("7 + 9 * (2 << 2)", 79),
-        ("6 // 2 + 0.0", 3.0),
-        ("2+3", 5),
-        ("6+4/2*2", 10.0),
-        ("3+2.45/8", 3.30625),
-        ("3**3*3/3+3", 30.0),
-        ("abs(-1)", 1),
-        ("pow(2,0)", 1),
-    ):
-        result = simple_eval(expr)
-        assert result == res
```

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_pysunsynk.py` & `sunsynk-0.3.5/tests/sunsynk/test_pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_register.py` & `sunsynk-0.3.5/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.3.5/tests/sunsynk/test_rwsensors.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 
     long = NumberRWSensor((1, 2), "long", max=0xFFFFF)
     reg55 = (55, 1)
     res55 = (1 << 16) + 55
     assert long.reg_to_value(reg55) == res55
     assert long.value_to_reg(res55, state.get) == reg55
 
+    with pytest.raises(NotImplementedError):
+        s.address = tuple()
+        s.value_to_reg(123, state.get)
+
 
 def test_select_rw(caplog, state) -> None:
     s = SelectRWSensor(1, "", options={1: "one", 2: "two"})
 
     assert s.reg_to_value((2,)) == "two"
     assert s.value_to_reg("two", state.get) == (2,)
     assert s.reg_to_value((5,)) is None
@@ -130,14 +134,17 @@
     state.track(s)
 
     tim = "2023-03-01 12:34:56"
     res = s.value_to_reg(tim, state.get)
     assert res == (5891, 268, 8760)
     assert s.reg_to_value(res) == tim
 
+    with pytest.raises(ValueError):
+        s.value_to_reg("2023-03-01 12:34", state.get)
+
 
 def test_time_rw(state) -> None:
     s = TimeRWSensor(60, "two", factor=0.1)
     state.track(s)
 
     state.update(
         {
@@ -206,7 +213,19 @@
 #     update_sensors([s], {60: 10})
 #     assert s.value == 1
 
 
 def test_bad_sensor(caplog) -> None:
     NumberRWSensor((60, 1), "two", factor=0.1, bitmask=1)
     assert "single register" in caplog.text
+
+
+def test_sensor_hash():
+    ss = {Sensor(0, "S 1"), Sensor(0, "S 1")}
+    assert len(ss) == 1
+    ss = {Sensor(0, "S 1"), Sensor(0, "S 2")}
+    assert len(ss) == 2
+
+    s = RWSensor((0, 1), "rwswitch")
+    m = SelectRWSensor((0, 1), "switch")
+    ss = {s, m}
+    assert len(ss) == 2
```

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_sensors.py` & `sunsynk-0.3.5/tests/sunsynk/test_sensors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 """Sunsynk sensor tests."""
 import logging
 from typing import Sequence
 
 import pytest
 
 from sunsynk.definitions import AMPS, CELSIUS, SENSORS, VOLT, WATT
-from sunsynk.rwsensors import RWSensor, SelectRWSensor
 from sunsynk.sensors import (
+    BinarySensor,
     FaultSensor,
     InverterStateSensor,
     MathSensor,
     SDStatusSensor,
     Sensor,
     SerialSensor,
     TempSensor,
 )
 from sunsynk.state import group_sensors
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def test_binary_sensor() -> None:
+    b = BinarySensor(111, "B 1")
+    assert b.reg_to_value((0,)) is False
+    assert b.reg_to_value((1,)) is True
+    assert b.reg_to_value((2,)) is True
+    assert b.reg_to_value((255,)) is True
+
+    b = BinarySensor(111, "B 1", on=1)
+    assert b.reg_to_value((0,)) is False
+    assert b.reg_to_value((1,)) is True
+    assert b.reg_to_value((2,)) is False
+    assert b.reg_to_value((255,)) is False
+
+    b = BinarySensor(111, "B 1", off=2)
+    assert b.reg_to_value((0,)) is True
+    assert b.reg_to_value((1,)) is True
+    assert b.reg_to_value((2,)) is False
+    assert b.reg_to_value((255,)) is True
+
+
 def test_sen():
     s = Sensor(0, "S 1")
     a = [s]
     assert a[0] == s
     assert s.id == "s_1"
 
     # Test __hash__
@@ -45,21 +65,17 @@
     ss = {Sensor(0, "S 1"), Sensor(0, "S 1")}
     assert len(ss) == 1
     ss = {Sensor(0, "S 1"), Sensor(0, "S 2")}
     assert len(ss) == 2
 
     s = Sensor(0, "S 1")
     m = MathSensor((0, 1), "math1", factors=(1, 1))
-    ss = {s, m}
-    assert len(ss) == 2
-
-    s = RWSensor((0, 1), "rwswitch")
-    m = SelectRWSensor((0, 1), "switch")
-    ss = {s, m}
-    assert len(ss) == 2
+    b = BinarySensor((0,), "b1")
+    ss = {s, m, b}
+    assert len(ss) == 3
 
 
 def test_group() -> None:
     sen = [
         Sensor(10, "10"),
         Sensor(11, "11"),
         Sensor(12, "12"),
@@ -103,16 +119,20 @@
     return [sum(b - a for a, b in zip(g[:-1], g[1:])) for g in groups]
 
 
 def test_ids() -> None:
     for name, sen in SENSORS.all.items():
         assert name == sen.id
 
-        if sen.factor and sen.factor < 0 and len(sen.address) > 1:
-            assert False, "only single signed supported"
+        try:
+            if sen.factor and sen.factor < 0 and len(sen.address) > 1:
+                assert False, "only single signed supported"
+        except TypeError:
+            _LOGGER.error("Sensor %s, factor=%s", name, sen.factor)
+            raise
 
         if sen.id in SENSORS.deprecated:
             continue
         assert sen.unit != AMPS or sen.name.endswith(" current")
         assert sen.unit != WATT or sen.name.endswith(" power")
         assert sen.unit != VOLT or sen.name.endswith(" voltage")
         assert sen.unit != CELSIUS or sen.name.endswith(" temperature")
@@ -157,15 +177,15 @@
 def test_update_func() -> None:
     s = SerialSensor(1, "", "")
     regs = (0x4148, 0x3738)
     assert s.reg_to_value(regs) == "AH78"
 
 
 # def test_update_float(caplog) -> None:
-#     s = TempSensor(60, "two", factor=0.1)
+#     s = TempSensor(60, "two", factors=0.1)
 #     rmap = register_map(60, [1001])
 #     update_sensors([s], rmap)
 
 #     assert s.value == 0.1
 
 #     s.reg_value = (None,)
 #     s.update_value()
```

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.3.5/tests/sunsynk/test_sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.4/tests/sunsynk/test_usunsynk.py` & `sunsynk-0.3.5/tests/sunsynk/test_usunsynk.py`

 * *Files identical despite different names*

